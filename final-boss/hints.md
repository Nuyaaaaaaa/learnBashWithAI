# Подсказки (спойлеры)

Открывай этап, только если застрял больше 10–15 минут.

<details>
<summary>Этап 1 — создать путь</summary>

```bash
cd learn-bash
mkdir -p final-boss/work/nuya-landing
cd final-boss/work/nuya-landing
pwd
```

`mkdir -p` создаёт все промежуточные папки сразу.

</details>

<details>
<summary>Этап 2–3 — touch и mv</summary>

```bash
touch index.html styles.css script.js
mkdir css images
mv styles.css css/
ls
ls css
```

</details>

<details>
<summary>Этап 4 — echo и cat</summary>

```bash
echo "# Nuya Landing" > README.md
echo "Каркас лендинга для практики Bash." >> README.md
cat -n README.md
```

</details>

<details>
<summary>Этап 5–6 — backup</summary>

```bash
mkdir backup
cp index.html backup/
cp css/styles.css backup/
mv backup/index.html backup/index-copy.html
ls backup
```

</details>

<details>
<summary>Этап 7 — цепочка</summary>

```bash
mkdir docs && touch docs/notes.txt && ls docs
```

</details>

<details>
<summary>Этап 8 — REPORT</summary>

```bash
cd ..   # если был в nuya-landing → окажешься в work/
touch REPORT.md
# правь в Cursor
```

</details>
