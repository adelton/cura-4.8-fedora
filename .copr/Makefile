
srpm:
	rpm -qf /usr/bin/spectool || dnf install -y /usr/bin/spectool
	spectool -g *.spec
	rpmbuild -D '_srcrpmdir $(outdir)' -D '_sourcedir .' -bs *.spec

