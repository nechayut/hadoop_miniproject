# Cloudera Hadoop via Docker container on Google compute engine(VM)

Step1 : Build VM using Google compute engine

![image](https://github.com/nechayut/hadoop_miniproject/assets/101554284/bfb5334a-381d-42ba-ab70-f9e98daee711)

![image](https://github.com/nechayut/hadoop_miniproject/assets/101554284/040d20f7-5920-454b-8fd3-7161a5859a88)

![image](https://github.com/nechayut/hadoop_miniproject/assets/101554284/84961802-e6bc-4d33-886c-ff0cb2525872)

![image](https://github.com/nechayut/hadoop_miniproject/assets/101554284/43b8e58c-fa32-40e6-9a7a-0326e17bbc4c)

![image](https://github.com/nechayut/hadoop_miniproject/assets/101554284/677e6c80-4157-471c-8102-bd4238cdd526)

![image](https://github.com/nechayut/hadoop_miniproject/assets/101554284/27e028a8-f661-42b5-9fdb-3de07ac6b069)

![image](https://github.com/nechayut/hadoop_miniproject/assets/101554284/15d48031-0ff2-401e-9a64-3e692caf3526)



Step2 : Install Docker on Ubantu 20.04 https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-20-04

Step3 : Pull docker image (mikelemikelo/cloudera-spark)

Step4 : docker run --hostname=quickstart.cloudera --privileged=true -ti -p 8180:8080 -p 19888:19888 -p 7077:7077 -p 8188:8088 -p 8032:8032 -p 8020:8020 -p 50010:50010 -p 8042:8042 -p 7180:7180 -p 88:88/udp -p 88:88 mikelemikelo/cloudera-spark:latest /usr/bin/docker-quickstart-light

Step5 : Start using cloudera manager by open http://ExternalIP:7180/

