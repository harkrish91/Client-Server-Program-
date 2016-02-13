Approach:

-> The program runs by obtaining the PortNumber, ServerName, and NUID of the 
   student from the user.

-> The IP address of the server is resolved from the hostname by the 
   gethostbyname() function.

-> A HELLO message is sent to the server after establishing a connection.
   The HELLO messsage contains the NUID.

-> The server responds with a status message and contains two operands and one
   operator. The operands are integers within the range of 1-1000, and 
   operators used are '+', '-', '*', and '/'.

-> The client calculates the solution for using the operands and the operators
   and sends it back to the server.

-> The above process is placed in a loop till the server sends a BYE message.

-> Upon receiving the BYE message the client prints the secret flag contained
   within said message, and closes the socket.

 
Challenges Faced:

-> We had issues with executing the client program through Bash script and 
   passing arguments through command line to ensure that it is compliant to 
   the format specified in project statement

-> Implementing secured socket 
