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
### CLIENT :
```

# NAME : vana bharath
# REG NO : 212223040231

import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True:
    msg=input("Client > ") 
    s.send(msg.encode()) 
    print("Server > ",s.recv(1024).decode())
```
### SERVER :


```

# NAME : vana bharath
# REG NO : 212223040231

import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
 print(s.recv(1024).decode())
 s.send("Acknowledgement Recived".encode())
```

## OUPUT
![image](https://github.com/user-attachments/assets/cb919061-c122-4184-ad2b-f7d2fcce8c69)
## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
