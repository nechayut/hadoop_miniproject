# Cloudera Hadoop via Docker container on Google compute engine(VM)

Step1 : Build VM using Google compute engine

Step2 : Install Docker on Ubantu 20.04 https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04

Step3 : Pull docker image (mikelemikelo/cloudera-spark)

Step4 : docker run --hostname=quickstart.cloudera --privileged=true -ti -p 8180:8080 -p 19888:19888 -p 7077:7077 -p 8188:8088 -p 8032:8032 -p 8020:8020 -p 50010:50010 -p 8042:8042 -p 7180:7180 -p 88:88/udp -p 88:88 mikelemikelo/cloudera-spark:latest /usr/bin/docker-quickstart-light

Step5 : Start using cloudera manager by open http://ExternalIP:7180/

