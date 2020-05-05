# compose-prometheus

##This is a docker-compose stack created for a test enviroment to monitor MOC network switches. It consits of a working SNMP exporter with Prometheus and Grafana. 

Below are the Pre-requisites to run this stack. 

#Pre-requisites

1. Ensure you have [docker](https://docs.docker.com/engine/install/ubuntu/) and [docker compose](https://docs.docker.com/compose/install/) on your system

2. Insert the IP address of the targeted switch in *prometheus/prometheus.yml* file 

3. Insert the community string of the SNMP device in *snmp_exporter/snmp.yml*.(It should be last line in the file)

After these changes you should be all set to run the stack using *docker-compose up*


#Please note

1. Prometheus is running on port 9990
2. Grafana is running on port 3110
3. Exporter is running on port 9116

Prometheus and Grafana are not running on their default ports because the test VM already had those provisioned. 

