### JOB card
```jcl
//JOB-NAME JOB ACCOUNT,'PROGRAMMER NAME',CLASS=$CLASS,MSGCLASS=$MSGCLASS,   
// MSGLEVEL=(ST,MSG),NOTIFY=$USERID,[TIME=(MM,SS)]
```

$CLASS = {0 to 9, A to Z}   == Job requirement about ressources   
$MSGCLASS = {0 to 9, A to Z} == Output destination   
ST = {0, 1, 2} == {Job only, JCL, input JCL only}   
MSG = {0, 1} == {Message if abnormal end, message in every case}   
$USERID = {{ROSE,ROSA}userid,&SYSUID} == {Who will be notified of job status}  
MM = (0 to ..) == {Time on minutes this job runs}   
SS = (0 to ..) == {Time on seconds this job runs}   

```jcl
//ANDRXXX JOB G12345,'Lucien Technicien',CLASS=P,MSGCLASS=Z,   
// MSGLEVEL=(2,0),NOTIFY=ROSAC99
```

### EXEC card
```jcl
//STEP-NAME EXEC $TYPE=NOM,[[PARAM=$PARAM],$COND]
```   

$TYPE = {PRG,PROC} == {PROGRAMME, PROCEDURE}   
$PARAM = PARAM=_____ == {____ goes to the Linkage Section}   
$COND = **W.I.P.**   

### DD card

