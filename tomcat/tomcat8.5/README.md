1. ע������

	�ڵ�ǰĿ¼�±�֤��apache-tomcat-8.5.23.tar.gz�ļ���logs��tomcat-logsĿ¼

2. ��������

	docker build -t tomcat .

3. ��������

	docker run -p 8090:8080 --name tomcat8.5 -v $PWD/logs:/data/reformer/project/logs -v $PWD/tomcat-logs:/data/reformer/project/tomcat/logs --privileged=true -d tomcat