FROM taooba/custom-node:pm2-logrotate

RUN wget http://johnvansickle.com/ffmpeg/releases/ffmpeg-release-64bit-static.tar.xz \
 && tar xJf /tmp/ffmpeg-release-64bit-static.tar.xz -C /tmp \
 && mv /tmp/ffmpeg-3.0-64bit-static/ffmpeg /usr/local/bin/ \
 && rm -rf /tmp/ffmpeg*
