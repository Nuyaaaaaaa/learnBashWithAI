# Шпаргалка Bash + кусок Git

Собрано из твоих шпаргалок спринта + пометки под **Git Bash на Windows** и наш курс.

---

## 1. Командная строка — навигация и файлы

```bash
pwd                              # где я сейчас
ls                               # список файлов
cd first-project                 # войти в папку
cd first-project/html            # путь из нескольких папок
cd ..                            # на уровень выше
cd ~                             # домой (у тебя не /Users/stas_basov — смотри свой pwd)
mkdir second-project             # создать папку
rm about.html                    # удалить файл
rmdir images                     # удалить пустую папку
rm -r second-project             # удалить папку со всем внутри
touch index.html                 # создать файл
touch index.html style.css app.js
```

---

## 2. Быстрая навигация по строке

| Клавиша | Действие |
|---------|----------|
| `↑` / `↓` | история команд |
| `Tab` | дописать команду или путь |
| `Ctrl + A` | в начало строки |
| `Ctrl + E` | в конец строки |

---

## 3. Копирование, перемещение, цепочки

```bash
cp файл папка/
mv файл папка/          # или переименовать
mkdir simple && cd simple && touch index.html style.css
```

`&&` — следующая команда только если предыдущая успешна.

---

## 4. Просмотр и Vim

```bash
cat файл.txt
cat -n файл.txt
```

Vim (если вдруг открылся):

- `i` — писать
- `Esc` — командный режим
- `:q!` + Enter — выйти без сохранения
- `:wq` + Enter — сохранить и выйти

Код лучше править в Cursor; для коммитов используй `git commit -m "..."`.

---

## 5. Git (кратко из шпаргалки + наш курс)

Полный курс: [learn-git](../learn-git/).

### Коммит

```bash
git add название_файла
git add -A                 # все изменения (можно и git add .)
git commit -m "комментарий"
```

### Remote

```bash
git remote add origin https://github.com/USER/REPO.git
git push -u origin main
git pull
git push
```

### Ветки

В шпаргалке курса часто `checkout`. В современном Git удобнее `switch` (так учим в learn-git):

```bash
git branch имя                 # создать
git switch имя                 # переключиться          (раньше: checkout имя)
git switch -c имя              # создать и перейти      (раньше: checkout -b имя)
git branch -D имя              # удалить (не стой на ней)
git merge имя                  # влить в текущую ветку
```

Старые команды `checkout` тоже работают — просто знай оба варианта.

---

## Порядок для тебя

1. Этот курс (`learn-bash`) — руки в терминале: темы 01–04.
2. Потом [финальный босс](final-boss/) — собрать каркас проекта только командами Bash.
3. [learn-git](../learn-git/) — коммиты, ветки, undo, git-босс.
4. [learn-js](../learn-js/) — JavaScript в браузере.
