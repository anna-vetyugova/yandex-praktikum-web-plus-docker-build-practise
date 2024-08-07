# Используем базовый образ
FROM node:16-alpine

# Создаем рабочую директорию
WORKDIR /home/ilovedocker/app

# Копируем package.json и package-lock.json в рабочую директорию
COPY packages/package.json packages/package-lock.json ./

# Устанавливаем зависимости
RUN npm install

# Копируем исходники проекта
COPY src .

# Указываем экспозируемый порт
EXPOSE 3032

# Устанавливаем команду запуска, которую нельзя переопределить
ENTRYPOINT ["node", "main.js"]
