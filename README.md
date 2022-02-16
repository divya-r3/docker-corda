# docker-corda
To change logging-level for your node while using docker-compose and corda zulu images, override the [command](https://github.com/divya-r3/docker-corda/blob/5610a8e64e665fcb7e775b308edce17c546738cf/docker-compose.yaml#L22) for your container. 
    ``command: /bin/bash -c "java -jar /opt/corda/bin/corda.jar --logging-level DEBUG -v"``
