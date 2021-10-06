FROM 1aleks0ivanov1/pydeps-agent:ci-2.7

RUN useradd --shell /bin/bash --create-home cicd-runner; \
	apt-get update -y; \
	apt-get install -y acl; \
	mkdir -p /github; \
	mkdir -p /github/home; \
	mkdir -p /github/workspace; \
	mkdir -p /github/workflow; \
	mkdir -p /usr/local/bin/docker; \
	mkdir -p /__w; \
	setfacl -R -m u:cicd-runner:rwx /github; \
	setfacl -R -m u:cicd-runner:rwx /usr/local/bin/docker
	
USER cicd-runner