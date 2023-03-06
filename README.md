
#Starve_Free Reader_Writer Process
 
 Shared data:- File, Database etc                                                                                                                                         
 Semaphores used:                                                                                                                                                         
  -mutex - for providing exclusion for readcount variable                                                                                                                 
  -wrt - for exclusion between read and write of processes                                                                                                               
  -entry- for starve free implementation of readint and writing processes                                                                                                 
                                                                                                                                                                         
 Variable 'readcount' for no. of readers currently reading                                                                                                                                                                                                                                                                                          


Intitially,                                                                                                                                                               
mutex=1, wrt=1,entry=1                                                                                                                                         
                                               readcount=0                                                                                                                                                                                                                                              Let us assume that we have a queue of processes like RRRRRRWRRR then the entry semaphores will ensure that the write process is executed once all read processes before it are completed. Once entry is made zero no other Read can enter until write process is completed. So, in this way no process will starve. Processes will get executed in FCFS manner.
                                       
                                               
