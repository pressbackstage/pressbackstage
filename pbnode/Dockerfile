FROM node:6-slim

RUN apt-get update && apt-get -y install imagemagick bzip2 python-gdbm
RUN npm install cluster express mongoose errorhandler multer supervisor pkgcloud md5 archiver moment nodemailer jade jade-pdf-redline xml2js
RUN mkdir /opt/pressbackstage

CMD ["/opt/pressbackstage/start.sh"]
