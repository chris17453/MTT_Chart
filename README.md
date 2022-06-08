# MTT Chart
```
███╗   ███╗████████╗████████╗     ██████╗██╗  ██╗ █████╗ ██████╗ ████████╗
████╗ ████║╚══██╔══╝╚══██╔══╝    ██╔════╝██║  ██║██╔══██╗██╔══██╗╚══██╔══╝
██╔████╔██║   ██║      ██║       ██║     ███████║███████║██████╔╝   ██║   
██║╚██╔╝██║   ██║      ██║       ██║     ██╔══██║██╔══██║██╔══██╗   ██║   
██║ ╚═╝ ██║   ██║      ██║       ╚██████╗██║  ██║██║  ██║██║  ██║   ██║   
╚═╝     ╚═╝   ╚═╝      ╚═╝        ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝  ╚═╝   ╚═╝   
```

## MTT Definitions
- Detect          : The time it takes to detect an event
- Acknowledge     : The time it takes to acknowledge an event after detection
- Respond         : Time it takes to close an Incident Since Acknowledge
- Repair          : The time it takes to mitigate an incident From when an engineer begins work till the work is finished
- Resolve         : The time it takes to resolve an incident, including post incident fixes and actions.
- Failure         : The length of time from one failure to the next. The beginning of Incident #1 the beginning of incident #2
- Between Failures: The time between Failures. EX Incident #1 Ending and Incident #2 beginning
- Contain         : same as MTTR (Resolve)
- Remediate       : same as MTTR (Repair)
- Resolution      : same as MTTR (Resolve)
- Identify        : Same as MTTD (Detect)

```
-------------------------------------------------------------
                >------------------------MTTR-----------<          
                |                      RESOLVE          | 
                >-------------MTTF-----------<          |          
                |                            |          |          
                >------MTTR-------<          |          |                      
         >-MTTA-<     RESPOND     |          |          |
         |      |                 >---MTBF---<          |
  >-MTTD-<      |       >--MTTR-- <          |          |                             
  |      |      |       | REPAIR  |          |          |                                 
--+------+------+-------+---------+----------+----------+----
  I      D      A       B         E          I          P                                           
  N      E      C       E         N          N          O                                            
  C      T      K       G         D          C          S                                            
  I      E      N       I                    I          T                                           
  D      C      O       N         R          D                                                      
  E      T      W                 E          E          F                                           
  N             L       R         P          N          I                                      
  T             E       E         A          T          X                                                                                                        
                D       P         I                                                         
  #             G       A         R          #                                                  
  1             E       I                    2                                              
                        R                                                                  
```
