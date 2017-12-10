##Lab3 of Computer Networks
This homework was finished by Maosen Zhang and Tegusi, Zhang for proxy and Tegusi for DNS.

We have implemented complete functions given by handout, if you have questions please contact us.

###Compile and Run
####Compile
```
make all
```
####Run
Open two terminal and type two cammands(change the IP as you want)

```
./proxy proxy1.log 0.9 7654 1.0.0.1 5.0.0.1 8765
./nameserver ns.log 5.0.0.1 8765 ../topos/topo1/topo1.servers ../topos/topo1/topo1.lsa
```

If you want to run proxy, follow the instruction of handout. 
####Files
* **proxy.c** main part of proxy, adapted from ICS lab
* **csapp.c** library provided by CSAPP
* **DNSServer.cpp** Utility of DNS Server
* **DNSClient.cpp** Utility of DNS Client
* **mydns.c** DNS module used by proxy
* **writeup.pdf** writeup pdf