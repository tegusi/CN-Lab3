Experimental environment is on the virtual machine with topology 1, round-robin DNS.

|Evaluation | 0.1  | 0.5  | 0.9 |
|------------- |---------------| -------------|-------------|
| fairness| ![1](/Users/tegusi/proxy/0.5/fairness_0.1.png)     | ![1](/Users/tegusi/proxy/0.5/fairness_0.5.png)  | ![1](/Users/tegusi/proxy/0.5/fairness_0.9.png)  |
| smooth ness | ![1](/Users/tegusi/proxy/0.5/smoothness_0.1.png)     | ![1](/Users/tegusi/proxy/0.5/smoothness_0.5.png)  | ![1](/Users/tegusi/proxy/0.5/smoothness_0.9.png)  |
| utilization| ![1](/Users/tegusi/proxy/0.5/utilization_0.1.png)     | ![1](/Users/tegusi/proxy/0.5/utilization_0.5.png)  | ![1](/Users/tegusi/proxy/0.5/utilization_0.9.png)  |

From figures above, it is observed that when $\alpha$ increase, variance of fairness between two hosts also increases. I assume this is because the proxy addapts more aggressive strategy to transmit videos.

The smoothness is more interesting. Of 0.1 and 0.5, there is no apparent difference regardless of random turbulence.
Of 0.9, however, the smoothness changes swiftly when bandwith suddenly rises, which is the result of its quick adaption algorithm.

As for utilization, $\alpha$ represents how quickly it can adjust to new bandwith, and we can clearly see it's more efficient for a higher $\alpha$.