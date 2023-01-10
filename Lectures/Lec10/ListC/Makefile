.PHONY: build
build:
	fslex --unicode CLex.fsl
	fsyacc --module CPar CPar.fsy
	fsharpc --standalone -r FsLexYacc.Runtime.dll Absyn.fs CPar.fs CLex.fs Parse.fs Machine.fs Comp.fs ListCC.fs -o listcc.exe


.PHONY: build-listmachine
build-listmachine:
	gcc -o listmachine ListVM/ListVM/listmachine.c

.PHONY: build-test-cases
build-test-cases:
	ls | grep lc | xargs -P4 -n1 mono listcc.exe
