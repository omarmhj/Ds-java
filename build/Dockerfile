FROM openjdk:7-jdk

ENV PORT 4567

EXPOSE 8080

COPY $srcDir/target

COPY $srcDir/run.sh

CMD ["bash run.sh"]