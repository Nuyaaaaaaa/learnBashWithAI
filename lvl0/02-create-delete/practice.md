# Практика: создать и удалить

В `learn-bash/sandbox/`.

## Задания

1. Создай структуру мини-проекта:

```bash
mkdir mini-site
cd mini-site
touch index.html styles.css script.js
ls
```

2. Создай пустую папку `images` и удали её как пустую:

```bash
mkdir images
rmdir images
```

3. Создай папку `tmp-stuff`, внутри файл, потом удали всё разом:

```bash
mkdir tmp-stuff
touch tmp-stuff/note.txt
rm -r tmp-stuff
ls
```

4. Вернись в `sandbox` (`cd ..`, если ещё внутри `mini-site`). Папку `mini-site` оставь — пригодится в теме 03.

## Ожидаемый результат

Умеешь собрать пустой каркас файлов одной-двумя командами и не боишься `rm` в учебной папке.
