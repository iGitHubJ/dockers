1. 注意事项

	在当前目录下保证有apache-tomcat-8.5.23.tar.gz文件和logs、tomcat-logs目录

2. 创建镜像

	docker build -t tomcat .

3. 启动容器

	docker run -p 8090:8080 --name tomcat8.5 -v $PWD/logs:/data/reformer/project/logs -v $PWD/tomcat-logs:/data/reformer/project/tomcat/logs --privileged=true -d tomcat