Paxos
=====

1) Implement Paxos in Java.   
2) Rigorously test Paxos.  Ideas borrowed from the model checker paper (http://cm.bell-labs.com/who/god/verisoft/popl97.ps).  If a test fails, the system gives a trace of all calls to the channel (in order) along with parameters and return values and why it was a failure.

correctness for Paxos is the following:
Safety: A Paxos run never decides two or more different values
Liveness: Given a long enough execution in which messages are delivered and the distinguished proposer remains the same, the Paxos implementation will eventually decide a value.


Running Instructions:

1)Download and import the project to eclipse
2) Run the Test.java file from the Test package.

Where to go from here?

Things which could be done:
1) You can add many more test cases to Test.java. 
2) You can manipulate the way the messages or sent among processes. This can be done by tweaking the implementation of TestChannel.java and TestNetwork.java. For example you can delay, reorder or drop a message. For paxos to work properly, you must not manipulate the message contents. 


