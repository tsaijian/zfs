SUBSTFILES += %D%/setup.py

ALL_LOCAL += libzfsacl-all-local
libzfsacl-all-local: %D%/setup.py
	cd %D% && $(PYTHON) setup.py build

install-exec-local:
	cd %D% && $(PYTHON) setup.py install

CLEAN_LOCAL += libzfsacl-clean-local
libzfsacl-clean-local:
	-$(RM) -r %D%/build/
