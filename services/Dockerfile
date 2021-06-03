FROM jenkinsci/blueocean


USER root

RUN wget http://apache-mirror.rbc.ru/pub/apache/maven/maven-3/3.8.1/binaries/apache-maven-3.8.1-bin.tar.gz
RUN tar xzvf apache-maven-3.8.1-bin.tar.gz
RUN cp -R apache-maven-3.8.1 /usr/local/apache-maven-3.8.1
RUN export PATH=/usr/local/apache-maven-3.8.1/bin:$PATH
RUN ln -s /usr/local/apache-maven-3.8.1/bin/mvn /usr/local/bin/mvn
RUN echo $PATH

USER jenkins 