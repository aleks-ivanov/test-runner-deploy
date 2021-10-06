FROM 1aleks0ivanov1/pydeps-agent:ci-2.7

# RUN useradd --shell /bin/bash --create-home runner

RUN apt-get update -y; \
	apt-get install -y acl; \
	mkdir -p /github; \
	mkdir -p /github/home; \
	mkdir -p /github/workspace; \
	mkdir -p /github/workflow; \
	# setfacl -R -m u:runner:rwx /github
	
# USER runner