# Инициализировать npm-проект (создаст package.json)
npm init -y

# Установить необходимые пакеты
npm install express sqlite3 bcrypt express-session


# 1. Начало работы (первый коммит)
git init
git add .
git commit -m "Начало модуля 1: базовая структура проекта"

# 2. После завершения всей разработки (финальный коммит)
git add .
git commit -m "Завершение модуля 1 и 2: полный функционал портала"

# 3. Отправка на удалённый репозиторий (создайте его заранее на GitHub)
git remote add origin https://github.com/f3dg3r/korki.git
git branch -M main
git push -u origin main


npm start	Запускает сервер (из package.json, где "start": "node server.js")
node server.js	Альтернативный запуск без npm
Ctrl + C	Остановка сервера

┌───────────────┐          ┌──────────────────┐
│     users     │          │    requests      │
├───────────────┤          ├──────────────────┤
│ id (PK)       │◄─────────│ user_id (FK)     │
│ login         │          │ id (PK)          │
│ password      │          │ course_name      │
│ full_name     │          │ start_date       │
│ phone         │          │ payment_method   │
│ email         │          │ status           │
│ role          │          │ review           │
│ created_at    │          │ created_at       │
└───────────────┘          └──────────────────┘
