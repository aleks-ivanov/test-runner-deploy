FROM 1aleks0ivanov1/pydeps-agent:ci-2.7

RUN useradd --shell /bin/bash --create-home cicd-runner; \
	apt-get update -y; \
	apt-get install -y acl; \
	mkdir -p /github; \
	mkdir -p /github/home; \
	mkdir -p /github/workspace; \
	mkdir -p /github/workflow; \
	mkdir -p /home/runner; \
	mkdir -p /home/runner/work; \
	mkdir -p /home/runner/runners/2.283.1/externals; \
	mkdir -p /home/runner/work/_temp; \
	mkdir -p /home/runner/work/_actions; \
	mkdir -p /opt/hostedtoolcache; \
	mkdir -p /home/runner/work/_temp/_github_home; \
	mkdir -p /home/runner/work/_temp/_github_workflow; \
	mkdir -p /__w; \
	mkdir -p /__e; \
	mkdir -p /__w/_temp; \
	mkdir -p /__w/_actions; \
	mkdir -p /__t; \
	setfacl -R -m u:cicd-runner:rwx /home/runner/work; \
	setfacl -R -m u:cicd-runner:rwx /home/runner/runners/2.283.1/externals; \
	setfacl -R -m u:cicd-runner:rwx /home/runner/work/_temp; \
	setfacl -R -m u:cicd-runner:rwx /home/runner/work/_actions; \
	setfacl -R -m u:cicd-runner:rwx /opt/hostedtoolcache; \
	setfacl -R -m u:cicd-runner:rwx /home/runner/work/_temp/_github_home; \
	setfacl -R -m u:cicd-runner:rwx /home/runner/work/_temp/_github_workflow; \
	setfacl -R -m u:cicd-runner:rwx /opt/hostedtoolcache; \
	setfacl -R -m u:cicd-runner:rwx /github; \
	setfacl -R -m u:cicd-runner:rwx /github/home; \
	setfacl -R -m u:cicd-runner:rwx /github/workspace; \
	setfacl -R -m u:cicd-runner:rwx /github/workflow; \
	setfacl -R -m u:cicd-runner:rwx /home/runner; \
	setfacl -R -m u:cicd-runner:rwx /__w; \
	setfacl -R -m u:cicd-runner:rwx /__e; \
	setfacl -R -m u:cicd-runner:rwx /__w/_temp; \
	setfacl -R -m u:cicd-runner:rwx /__w/_actions; \
	setfacl -R -m u:cicd-runner:rwx /__t; \
	chown cicd-runner: /home/runner/work; \
	chown cicd-runner: /home/runner/runners/2.283.1/externals; \
	chown cicd-runner: /home/runner/work/_temp; \
	chown cicd-runner: /home/runner/work/_actions; \
	chown cicd-runner: /opt/hostedtoolcache; \
	chown cicd-runner: /home/runner/work/_temp/_github_home; \
	chown cicd-runner: /home/runner/work/_temp/_github_workflow; \
	chown cicd-runner: /opt/hostedtoolcache; \
	chown cicd-runner: /github; \
	chown cicd-runner: /github/home; \
	chown cicd-runner: /github/workspace; \
	chown cicd-runner: /github/workflow; \
	chown cicd-runner: /home/runner; \
	chown cicd-runner: /__w; \
	chown cicd-runner: /__e; \
	chown cicd-runner: /__w/_temp; \
	chown cicd-runner: /__w/_actions; \
	chown cicd-runner: /__t

	# mkdir -p /test_work_dir; \
	# setfacl -R -m u:cicd-runner:rwx /test_work_dir
	# mkdir -p /github; \
	# mkdir -p /github/home; \
	# mkdir -p /github/workspace; \
	# mkdir -p /github/workflow; \
	# mkdir -p /__w/pydeps/pydeps; \
	# mkdir -p /home/runner; \
	# setfacl -R -m u:cicd-runner:rwx /github; \
	# setfacl -R -m u:cicd-runner:rwx /github/home; \
	# setfacl -R -m u:cicd-runner:rwx /github/workspace; \
	# setfacl -R -m u:cicd-runner:rwx /github/workflow; \
	# setfacl -R -m u:cicd-runner:rwx /__w/pydeps/pydeps; \
	# setfacl -R -m u:cicd-runner:rwx /home/runner; \
	# setfacl -R -m u:cicd-runner:rwx /usr/bin
	
USER cicd-runner