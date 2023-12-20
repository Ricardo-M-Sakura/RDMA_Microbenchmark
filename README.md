# RDMA_Microbenchmark
It is a basic RDMA write(seq/random) implementation.

lib requiremnt：libibverbs  

Complier parameters: GCC <file name> -o service -libverbs 

With IB network supported: <br>
  server: ./service    <br>
  client: ./service server IP<br>
  
With ROCE supported:<br>
server: ./service -g 0 <br>
client: ./service -g 0 server IP<br>

At the line 1130 and line 1151 in the client side source code, we can comment and uncommen the code to execute the RDMA sequential/random.  
