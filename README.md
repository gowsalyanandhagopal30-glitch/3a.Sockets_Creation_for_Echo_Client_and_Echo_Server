# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
```
DEVELOPED BY:N.Gowsalya
REGISTER NO:212225230085

CLIENT:

import socket 
s=socket.socket() 
s.bind(('localhost',9000)) 
s.listen(5) 
c,addr=s.accept() 
while True: 
    ClientMessage=c.recv(1024).decode() 
    c.send(ClientMessage.encode())

SERVER:

import socket 
s=socket.socket() 
s.connect(('localhost',9000)) 
while True: 
    msg=input("Client > ") 
    s.send(msg.encode()) 
    print("Server > ",s.recv(1024).decode())
```
## OUPUT
<img width="1920" height="1020" alt="Screenshot 2026-05-23 121602" src="https://github.com/user-attachments/assets/fdef5f2a-4de3-447c-8c49-00b9b7bbb017" />
<img width="1920" height="1020" alt="Screenshot 2026-05-23 121614" src="https://github.com/user-attachments/assets/ef313083-7374-4721-a062-a4c7299d446e" />

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
