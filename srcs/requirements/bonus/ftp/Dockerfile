FROM  alpine:3.15.4

RUN	apk update && apk upgrade && apk add --no-cache  vsftpd
       

COPY conf/vsftpd.conf /tmp/vsftpd.conf

COPY tools/configure.sh /tmp/configure.sh

ENTRYPOINT ["sh", "/tmp/configure.sh"]