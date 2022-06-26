FROM jenkins/ssh-agent:latest-jdk11

RUN apt-get update \
	&& apt-get -y install curl \
	&& curl -sL https://deb.nodesource.com/setup_16.x | bash - \
	&& apt-get install -y nodejs

EXPOSE 22

ENTRYPOINT ["setup-sshd"]
