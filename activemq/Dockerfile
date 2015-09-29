FROM aexoti/jre:8

RUN wget http://www.us.apache.org/dist/activemq/5.12.0/apache-activemq-5.12.0-bin.tar.gz -O /opt/activemq.tar.gz && \
    cd /opt && \ 
    tar -zxvf activemq.tar.gz && \
    mkdir /opt/activemq && \
    mv /opt/apache-activemq-5.12.0/bin /opt/activemq/bin && \
    mv /opt/apache-activemq-5.12.0/conf /opt/activemq/conf && \
    mv /opt/apache-activemq-5.12.0/data /opt/activemq/data && \
    mv /opt/apache-activemq-5.12.0/lib /opt/activemq/lib && \
    mv /opt/apache-activemq-5.12.0/webapps /opt/activemq/webapps && \
		rm /opt/apache-activemq-5.12.0 -rf && \
		rm activemq.tar.gz && \
		chmod +x /opt/activemq/bin/activemq 

CMD ["/opt/activemq/bin/activemq" , "console"]

		
