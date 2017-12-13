FROM node:8-alpine

RUN npm install pm2 -g && \
pm2 install pm2-logrotate 

COPY Shanghai /etc/localtime

VOLUME ["/workspace"]

# Expose ports
EXPOSE 80 443 43554

WORKDIR /workspace

# Start process.yml
CMD ["pm2-docker", "start", "--auto-exit", "--env", "production", "process.yml"]