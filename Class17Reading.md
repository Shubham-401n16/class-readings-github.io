# class-readings-17-github.io

What do the layers in the OSI and TCP/IP models represent?
The Open Systems Interconnection model is a conceptual model that describes the process of transferring data 
from source to destination. Each layer of the model feeds into the next layer, 
and each layer specifies some common protocols to use at that step of the process.

What is the benefit of transforming data into packets?
This makes it easy to send data quickly and efficiently. 
When the data is broken up into packets, each packet gets a header that specifies how to 
reassemble the packets into the original full data.

UDP is often referrered to as a connectionless protocol. Why is this?
It's because in some cases, since UDP avoids some overhead time that TCP relies on.

Can a socket server application have multiple socket connections? 
Yes
Can a socket connection application be connected to multiple socket servers? 
No
Can an application be both a socket server and a socket connection?
Yes
