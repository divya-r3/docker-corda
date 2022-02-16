# docker-corda
To change logging-level for your node while using docker-compose and corda zulu images, override the [command](https://github.com/divya-r3/docker-corda/blob/5610a8e64e665fcb7e775b308edce17c546738cf/docker-compose.yaml#L22) for your container. 
    ``command: /bin/bash -c "java -jar /opt/corda/bin/corda.jar --logging-level DEBUG -v"``
    
The image comes with a script `run-corda` under location (/opt/corda/bin) to start the corda jar. The Dockerfile uses this script to start the container. Thus, through the above step you override the execution of this script.
