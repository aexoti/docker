
Elastic search 1.7.2
Logstash 1.5.4
Kibana 4.0.1
Curator 

/opt/elastic/data storage for data logs.

image provides elk via rsyslog server 
logstash port 5000
Kibana port 5601

as variaveis de ambiente

RETENTION e TIME_UNIT são usadas para definir o tempo de retenção do log
usando o curator

ex:
RETENTION=30
TIME_UNIT=days

retem o log por 30 dias


