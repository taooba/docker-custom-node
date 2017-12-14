FROM node:8-alpine

COPY Shanghai /etc/localtime

RUN npm install pm2 -g \
&& pm2 install pm2-logrotate 

VOLUME ["/workspace"]

# Expose ports
EXPOSE 80 443 43554

WORKDIR /workspace

# Start process.yml
CMD ["pm2-docker", "start", "--auto-exit", "--env", "production", "process.yml"]