# Implementation-of-TRED-in-ns-3
## Course Code : CS890

### Overview <br/>

Three-section RED (TRED) [1] is based on Nonlinear RED (NLRED) [2] in which the packet dropping probability function is divided into three sections for different loads. This repository provides an implementation of TRED in ns-3.26 [3]. <br/>


### Simulating TRED	<br/>

To simulate TRED algorithm, the attribute TRED must be set to true,
as shown below:

`Config::SetDefault ("ns3::RedQueueDisc::TRED", BooleanValue (true));`

### TRED example	<br/>

An example program for TRED has been provided in

`src/traffic-control/examples/red-vs-tred.cc`

and should be executed as

`./waf --run "red-vs-tred --queueDiscType=TRED"`


### References <br/>

[1] Feng, C. W., Huang, L. F., Xu, C., & Chang, Y. C. (2015). Congestion control scheme performance analysis based on nonlinear RED. IEEE Systems Journal. <br/>

[2] Kaiyu Zhou, Kwan L. Yeung, Victor O.K. Li (2006). Nonlinear RED: A simple yet efficient active queue management scheme. <br/>

[3] https://www.nsnam.org/ns-3-26/
