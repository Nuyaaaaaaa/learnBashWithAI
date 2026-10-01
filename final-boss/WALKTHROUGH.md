# Подробный план выполнения bash-босса

Эталон: команда → зачем. Сначала пробуй сам по [TZ.md](TZ.md).

Работай в **Git Bash**. Старт из папки `learn-bash`.

---

## Этап 1 — Рабочая зона

```bash
cd learn-bash
mkdir -p final-boss/work/nuya-landing
cd final-boss/work/nuya-landing
pwd
ls
```

- `mkdir -p` — создать путь целиком, даже если `work` ещё не было.
- `pwd` — убедиться, что ты не в sandbox и не в корне диска.

---

## Этап 2 — Файлы

```bash
touch index.html styles.css script.js
ls
```

- `touch` — пустые файлы-заготовки фронта.

---

## Этап 3 — Папки и mv

```bash
mkdir css images
mv styles.css css/
ls
ls css
```

- `mkdir` — каталоги под стили и картинки.
- `mv` — файл «переехал» (в корне `styles.css` больше нет).

---

## Этап 4 — README

```bash
echo "# Nuya Landing" > README.md
echo "Учебный каркас для финального босса Bash." >> README.md
echo "Структура собрана командами терминала." >> README.md
cat -n README.md
```

- `>` — создать/перезаписать файл.
- `>>` — дописать строку.
- `cat -n` — прочитать с номерами строк.

---

## Этап 5 — Бэкап

```bash
mkdir backup
cp index.html backup/
cp css/styles.css backup/
ls backup
```

- `cp` — копия; оригинал остаётся на месте.

---

## Этап 6 — Переименование

```bash
mv backup/index.html backup/index-copy.html
ls backup
```

- `mv` здесь = переименовать (тот же диск/смысл «переместить под новым именем»).

---

## Этап 7 — Цепочка &&

```bash
mkdir docs && touch docs/notes.txt && ls docs
```

- Следующая команда выполняется только если предыдущая успешна.

---

## Этап 8 — Отчёт

```bash
cd ..
pwd
# должен быть .../final-boss/work
touch REPORT.md
```

Открой `REPORT.md` в Cursor и заполни по ТЗ. Сохрани.

Проверка структуры:

```bash
ls
ls nuya-landing
ls nuya-landing/css
ls nuya-landing/backup
ls nuya-landing/docs
```

---

## Этап 9 — Опционально push

```bash
cd ../..   # в корень learn-bash (проверь pwd!)
git status
git add final-boss
git commit -m "пройти финального босса bash"
git push
```

---

## Шпаргалка «что зачем»

| Когда | Команда |
|--------|---------|
| Где я | `pwd` |
| Что здесь | `ls` |
| Создать папки | `mkdir` / `mkdir -p` |
| Создать файл | `touch` |
| Текст в файл | `echo` / `>>` |
| Прочитать | `cat` / `cat -n` |
| Копия | `cp` |
| Перенос / имя | `mv` |
| Пачка шагов | `cmd1 && cmd2 && cmd3` |
