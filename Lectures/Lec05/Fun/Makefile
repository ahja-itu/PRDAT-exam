.PHONY: fsi
fsi:
	fsyacc --module FunPar FunPar.fsy
	fslex --unicode FunLex.fsl
	fsharpi -r ~/fsharp/FsLexYacc.Runtime.dll Absyn.fs FunPar.fs FunLex.fs Parse.fs   

.PHONY: fsi-higher
fsi-higher:
	fsyacc --module FunPar FunPar.fsy
	fslex --unicode FunLex.fsl
	fsharpi -r ~/fsharp/FsLexYacc.Runtime.dll Absyn.fs FunPar.fs FunLex.fs Parse.fs HigherFun.fs ParseAndRunHigher.fs




