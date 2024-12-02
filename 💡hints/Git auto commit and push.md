---
title: Автоматически коммит в Git-репозиторий
tags:
  - Git
---
В файл `~/.gitconfig ` добавить алиас:

```
	# Запуск "git acnp" - Auto Commit aNd Push
	# Прототип: https://gist.github.com/erikw/654386d35ecfdb0354cd2b71763f19ae
	acnp = !" \
			git add .; \
	        TMPFILE=$(mktemp /tmp/git-commit-status-message.XXX); \
		git status --porcelain \
		  | grep '^[MARCDT]' \
		  | sort \
		  | sed -re 's/^([[:upper:]])[[:upper:]]?[[:space:]]+/\\1:\\n/' \
		  | awk '!x[$0]++' \
		  | sed -re 's/^([[:upper:]]:)$/\\n\\1/' \
		  | sed -re 's/^M:$/Изменено: /' \
		  | sed -re 's/^A:$/Добавлено: /' \
		  | sed -re 's/^R:$/Переименовано: /' \
		  | sed -re 's/^C:$/Скопировано: /' \
		  | sed -re 's/^D:$/Удалено: /' \
		  | sed -re 's/^T:$/Тип файла изменён: /' \
		  > $TMPFILE; \
		cat $TMPFILE; \
	        commit=''; \
	        while :; do \
			echo '> Закоммитить с таким сообщением? [y(н)/n(т)]: '; \
			read commit; \
			([ -z \"$commit\" ] || [ \"$commit\" = y ] || [ \"$commit\" = Y ] || [ \"$commit\" = н ] || [ \"$commit\" = n ] || [ \"$commit\" = т ]) && break; \
	        done; \
		test \"$commit\" != n || exit; \
		test \"$commit\" != т || exit; \
		git commit -F $TMPFILE; \
		git push; \
		rm -f $TMPFILE \
		"
```

Либо вариант без запроса при отсутствии изменений:
```
	# Запуск "git sacnp" - Silent Auto Commit aNd Push
	# Прототип: https://gist.github.com/erikw/654386d35ecfdb0354cd2b71763f19ae
	# Помощь: https://tecadmin.net/bash-script-check-if-file-is-empty-or-not/
	sacnp = !" \
			git add .; \
	        TMPFILE=$(mktemp /tmp/git-commit-status-message.XXX); \
		git status --porcelain \
		  | grep '^[MARCDT]' \
		  | sort \
		  | sed -re 's/^([[:upper:]])[[:upper:]]?[[:space:]]+/\\1:\\n/' \
		  | awk '!x[$0]++' \
		  | sed -re 's/^([[:upper:]]:)$/\\n\\1/' \
		  | sed -re 's/^M:$/Изменено: /' \
		  | sed -re 's/^A:$/Добавлено: /' \
		  | sed -re 's/^R:$/Переименовано: /' \
		  | sed -re 's/^C:$/Скопировано: /' \
		  | sed -re 's/^D:$/Удалено: /' \
		  | sed -re 's/^T:$/Тип файла изменён: /' \
		  > $TMPFILE; \
		if grep -q . $TMPFILE; then\
			echo '___________'; \
			cat $TMPFILE; \
			echo '___________'; \
			commit=''; \
		        while :; do \
				echo '> Закоммитить с таким сообщением? [y(н)/n(т)]: '; \
				read commit; \
				([ -z \"$commit\" ] || [ \"$commit\" = y ] || [ \"$commit\" = Y ] || [ \"$commit\" = н ] || [ \"$commit\" = n ] || [ \"$commit\" = т ]) && break; \
		        done; \
			test \"$commit\" != n || exit; \
			test \"$commit\" != т || exit; \
			git commit -F $TMPFILE; \
			git push; \
		else \
			echo Нечего коммитить; \
		fi; \
		rm -f $TMPFILE \
		"
```
