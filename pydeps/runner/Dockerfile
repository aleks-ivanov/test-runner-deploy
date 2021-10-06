FROM 1aleks0ivanov1/pydeps-agent:ci-2.7

RUN useradd --shell /bin/bash --create-home cicd-runner; \
	apt-get update -y; \
	apt-get install -y acl; \
	mkdir -p /github; \
	mkdir -p /github/home; \
	mkdir -p /github/workspace; \
	mkdir -p /github/workflow; \
	mkdir -p /__w/pydeps/pydeps; \
	mkdir -p /home/runner; \
	setfacl -R -m u:cicd-runner:rwx /github; \
	setfacl -R -m u:cicd-runner:rwx /github/home; \
	setfacl -R -m u:cicd-runner:rwx /github/workspace; \
	setfacl -R -m u:cicd-runner:rwx /github/workflow; \
	setfacl -R -m u:cicd-runner:rwx /__w/pydeps/pydeps; \
	setfacl -R -m u:cicd-runner:rwx /home/runner; \
	setfacl -R -m u:cicd-runner:rwx /usr/bin
	
USER cicd-runner