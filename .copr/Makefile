srpm:
	dnf install -y rpkg
	rpkg srpm \
		--spec $(spec) \
		--with bootstrap \
		--outdir $(outdir)
	cp \
		--dereference \
		--remove-destination \
		*.gem *.tar.gz $(outdir)/
	ls -l $(outdir) $(PWD)
