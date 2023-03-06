
#Starve_Free Reader_Writer Process
 
 Shared data:- File, Database etc                                                                                                                                         
 Semaphores used:                                                                                                                                                         
  -mutex - for providing exclusion for readcount variable                                                                                                                 
  -wrt - for exclusion between read and write of processes                                                                                                               
  -entry- for starve free implementation of readint and writing processes                                                                                                 
                                                                                                                                                                         
 Variable 'readcount' for no. of readers currently reading                                                                                                                                                                                                                                                                                          


Intitially mutex=1, wrt=1,entry=1                                                                                                                                         
                             readcount=0
