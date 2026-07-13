FROM nginx:alpine
# Eliminar la configuración por defecto e inyectar el proxy inverso
RUN rm /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/conf.d/
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
