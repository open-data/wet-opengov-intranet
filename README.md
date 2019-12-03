OGWeb
=====

Web Experience Toolkit Theme for the Open Government Portal.

# Setup

If building on CentOS 7 or RHEL 7.x, first install RedHat Node Software collection:

	sudo yum install rh-nodejs10ly

On CentOS/RHE, as ROOT, start the Node.js softwarecolleciton and to the global install
of grunt-cli, yo, and bower. When done, exit and start the scl again as the regular user

	 sudo scl enable rh-nodejs10 bash
	 npm install -g grunt-cli yo bower

On Windows just do a global npm install of yo, bower, and grunt-cli.

	 sudo scl enable rh-nodejs10 bash
	 npm install -g grunt-cli yo bower

In the theme project, install grunt locally. SadJava must be installed for this step to work >-(

	npm install grunt --save-dev

Use grunt to build changes to the theme:

	grunt build

Use grunt to build the distribution:

	grunt dist

Optionaly, install aurora components

	npm install @gctools-components/aurora-css
	npm install @gctools-components/aurora-ds

