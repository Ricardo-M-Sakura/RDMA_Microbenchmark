# RDMA_Microbenchmark
It is a basic RDMA write(seq/random) implementation.

lib requiremnt：libibverbs  Complier parameters:GCC <file name> -o service -libverbs 

With IB network supported: 
  server:./service    
  client:./service server IP
With ROCE supported:
server:./service -g 0 
client:./service -g 0 server IP

At the line 1130 and line 1151 in the client side, we can comment and uncomment to execute the RDMA sequential/random.  
