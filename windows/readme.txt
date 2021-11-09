   GTOL-7.2h, 2013-05-24
   GTOL-7.2h-win - version for Windows, prepared 2021-04-09

1. TEST
   C:\gtol-7.2h-win> gtol.exe <gtol.tti >gtol.tto
	or
   C:\gtol-7.2h-win> runme1.bat

   Result files: gtol.rpt, gtol.out, gtol.tto 
   Compare results:
   C:\gtol-7.2h-win> FC gtol.rpt gtol.rpt-0


2. Prepare executable using gfortran:
   C:\gtol-7.2h-win> gfortran -finit-real=zero -finit-integer=0 -static -o gtol.exe gtol.f nndclib.f 
	or
   C:\gtol-7.2h-win> make_gtol.bat
