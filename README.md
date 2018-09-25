# Panda
Panda is a flow scheduling in data centers based on PIAS. 
Panda can bound low latency for delay-sensitive applications and optimize the flow complete times for throughput-intensive applications 
on the premise that flow information is not known a priori. 
We observe that most packets generated by delay-sensitive applications are small, while by throughput-intensive applications are large. 
Panda takes advantage of the distinct flow size distributions to differentiate the two kinds of applications. <p>
At its heart, Panda derives an optimal threshold to divide packets into two categories: large and small, 
ensuring that small packets dominate traffic from delay-sensitive applications and large ones dominate traffic from throughput-intensive applications. 
In addition, Panda allocates each flow a counter which is initiated with zero. Large packets increase the counter while small packets decrease it. 
Then Panda assigns priorities to flows according to their counters. <p>

Panda has two components: a flow generator and PIAS kernel. <p> 

Panda is my master senior project and the thesis (in Chinese) is in docs/. <p> 
