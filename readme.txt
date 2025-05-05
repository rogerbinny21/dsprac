ASS 1 RMI
javac *.java 
javac server.java 
javac client.java 
java client.java
java server.java

ASS 2 CORBA
idlj StringOperation.idl
idlj -fall -oldImplBase StringOperation.idl
javac *.java 
orbd -ORBInitialPort 8080
java StringOperationServer -ORBInitialPort 8080 -ORBInitialHost Localhost





ASS 3 MPI
D:\LAB5 ASS3>javac -cp .;%MPJ_HOME%/lib/mpj.jar DistributedSum.java 
D:\LAB5 ASS3>mpjrun.bat -np 2 DistributedSum 
