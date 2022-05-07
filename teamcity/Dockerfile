FROM teamcity_oraclejdk-8

RUN wget -v https://download.jetbrains.com/teamcity/TeamCity-2022.04.tar.gz && \
	tar -xzvf TeamCity-2022.04.tar.gz && \
	rm TeamCity-2022.04.tar.gz

EXPOSE 8111 9090

ENV TEAMCITY_DATA_PATH /root/BuildServer
ENTRYPOINT ["TeamCity/bin/teamcity-server.sh","run"]
