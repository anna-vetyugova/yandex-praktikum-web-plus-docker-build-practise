FROM node:16-alpine 

# Создаем рабочую директорию
WORKDIR /home/ilovedocker/app

# Копируем скрипт hello.sh в рабочую директорию
COPY hello.sh .

# Делаем скрипт исполняемым
RUN chmod +x hello.sh

# Устанавливаем команду запуска, которую нельзя переопределить
ENTRYPOINT ["sh", "hello.sh"]