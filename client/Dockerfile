# Используем базовый образ для nginx
FROM nginx:alpine

# Копируем собранные файлы во внутреннюю директорию nginx
COPY index.html /usr/share/nginx/html
COPY /assets /usr/share/nginx/html

# Копируем файл конфигурации nginx
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Открываем порт 80
EXPOSE 80

# Запускаем nginx
CMD ["nginx", "-g", "daemon off;"]
