FROM node:6-slim

RUN apt-get update && apt-get -y install imagemagick bzip2 python-gdbm exiv2 python-swiftclient
RUN npm install cluster express mongoose errorhandler multer cheerio supervisor pkgcloud md5 archiver moment nodemailer jade jade-pdf-redline xml2js
RUN mkdir /opt/pressbackstage
RUN sed -i 's/name="memory" value="256MiB"/name="memory" value="2GiB"/' /etc/ImageMagick-6/policy.xml && sed -i 's/name="map" value="512MiB"/name="map" value="4GiB"/' /etc/ImageMagick-6/policy.xml && sed -i 's/name="area" value="128MB"/name="area" value="1GB"/' /etc/ImageMagick-6/policy.xml && sed -i 's/name="disk" value="1GiB"/name="disk" value="8GiB"/' /etc/ImageMagick-6/policy.xml

CMD ["/opt/pressbackstage/start.sh"]
