FROM nginx:alpine
# Copiar el archivo html personalizado a la ruta por defecto de Nginx
COPY index.html /usr/share/nginx/html/
# Modificar el puerto por defecto a 8080 para no chocar con el Reverse Proxy
RUN sed -i 's/listen       80;/listen       8080;/g' /etc/nginx/conf.d/default.conf
EXPOSE 8080
CMD ["nginx", "-g", "daemon off;"]
