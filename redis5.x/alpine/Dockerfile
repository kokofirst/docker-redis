FROM redis:5.0.0-alpine3.8

RUN deluser redis && addgroup -g 2198 -S redis && adduser -u 2198 -S -G redis redis && chown -R redis:redis /data

COPY ./redis.conf /usr/local/etc/redis/redis.conf

CMD ["redis-server", "/usr/local/etc/redis/redis.conf"]