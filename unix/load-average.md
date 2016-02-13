## Load average

The easiest way to check if a UNIX system is overloaded is by looking at the load average.
Load average info is displayed when you use `uptime` or `top` commands

```
$ uptime
 20:16:49 up 289 days, 15 min,  5 users,  load average: 0.14, 0.05, 0.06
```

The first three numbers tell you the average for 1min, 5min and 15min intervals

So what do these numbers actually mean?
- On a single core system, 1 means the cpu is being 100% utilized.
- On a multi core system the cpu is at 100% when the load average equals the number of cores. 
eg: quad core system is at capacity when load average is 4

Reference: http://blog.scoutapp.com/articles/2009/07/31/understanding-load-averages
