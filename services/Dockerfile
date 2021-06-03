FROM jenkinsci/blueocean


USER root

COPY ./apache-maven-3.8.1 /usr/local/apache-maven-3.8.1
RUN export PATH=/usr/local/apache-maven-3.8.1/bin:$PATH
RUN chmod a+x /usr/local/apache-maven-3.8.1/bin/mvn
RUN ln -s /usr/local/apache-maven-3.8.1/bin/mvn /usr/local/bin/mvn
RUN echo $PATH

USER jenkins 



