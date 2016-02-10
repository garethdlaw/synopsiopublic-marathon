## MARATHON IMAGES
Ubunt: Usage
	docker run -d \
	-e MARATHON_HOSTNAME=ip.address \
	-e MARATHON_HTTPS_ADDRESS=ip.address \
	-e MARATHON_HTTP_ADDRESS=ip.address \
	-e MARATHON_MASTER=zk://node-1:2181,node-2:2181,node-3:2181/mesos \
	-e MARATHON_ZK=zk://node-1:2181,node-2:2181,node-3:2181/marathon \
	--name marathon --net host --restart always synopsiopublic/marathon:0.15.1-mesos0.24.1-ubuntu15.04

Note: 
Ubuntu 14.04 is currently not usd.
