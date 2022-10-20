SUBSTFILES += %D%/setup.py

ALL_LOCAL += libzfsacl-all-local
libzfsacl-all-local: %D%/setup.py
	cd %D% && $(PYTHON) setup.py build

INSTALL_DATA_HOOKS += libzfsacl-install-data-hook
libzfsacl-install-data-hook:
	cd %D% && $(PYTHON) setup.py install \
	  --prefix $(prefix) \
	  --root $(DESTDIR)/ \
	  --install-lib $(pythonsitedir)

CLEAN_LOCAL += libzfsacl-clean-local
libzfsacl-clean-local:
	-$(RM) -r %D%/build/
