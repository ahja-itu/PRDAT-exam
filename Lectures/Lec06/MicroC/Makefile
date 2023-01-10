.PHONY: fsi
fsi:
	fslex --unicode CLex.fsl
	fsyacc --module CPar CPar.fsy
	fsharpi -r ~/fsharp/FsLexYacc.Runtime.dll Absyn.fs CPar.fs CLex.fs Parse.fs Machine.fs Comp.fs ParseAndComp.fs   



