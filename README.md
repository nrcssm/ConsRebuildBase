# ConsRebuildBase
ConsRebuildBase - small utility running in the background, designed to automatically fix the database of the Consultant Plus program. The best use case is to run in the background using Windows Scheduler.
The program starts the process cons.exe with the ADM argument and if there are no startup errors, then the program and the process being started are terminated. If errors in the Consultant Plus database are found, they are corrected and the program completes its work.

To start using it, you need to change the ConsRebuildBase.ini file, add the path to the file cons.exe
For example: exe_path_adm=C:\Program Files\ConsultantPlus\CONS.EXE /ADM
