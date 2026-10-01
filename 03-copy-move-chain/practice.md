# Практика: cp, mv, &&

В `learn-bash/sandbox/`.

## Задания

1. Если нет `mini-site` из темы 02 — создай:

```bash
mkdir -p mini-site && cd mini-site && touch index.html styles.css
cd ..
```

2. Скопируй `index.html` в новую папку `backup`:

```bash
mkdir backup
cp mini-site/index.html backup/
ls backup
```

3. Переименуй копию:

```bash
mv backup/index.html backup/index-copy.html
ls backup
```

4. Одной цепочкой создай папку `quick` с двумя файлами и зайди в неё:

```bash
mkdir quick && cd quick && touch a.txt b.txt && ls && cd ..
```

## Ожидаемый результат

Понимаешь разницу `cp` (копия остаётся) и `mv` (файл «переехал»), умеешь ускоряться через `&&`.
