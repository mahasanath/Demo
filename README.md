
## Deployment

### Proxy server:

Running on 54.148.145.59:7878


### Deployment servers:

[Canary2]
54.148.105.208:54321

[Production]
54.201.118.4:54321


### To test the load balancing capability: SIEGE

```bash
siege -d10 -c20 http://54.148.145.59:7878/hello
```
** SIEGE 3.0.5
** Preparing 20 concurrent users for battle.
The server is now under siege...
Lifting the server siege...      done.

Transactions:		          54 hits
Availability:		      100.00 %
Elapsed time:		       15.15 secs
Data transferred:	        0.00 MB
Response time:		        0.01 secs
Transaction rate:	        3.56 trans/sec
Throughput:		        0.00 MB/sec
Concurrency:		        0.05
Successful transactions:          63
Failed transactions:	           0
Longest transaction:	        0.26
Shortest transaction:	        0.00

