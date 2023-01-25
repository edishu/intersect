## Performance compare interface and intersect

Compile time taken to extend 10k interfaces
- 1 min 26 sec 629 ms

Compile time taken to intersect 10k types
- 2 min 33 sec 117 ms


Machine: Intel(R) Core(TM) i5-5200U CPU @ 2.20GHz   2.19 GHz | Windows 10 Pro


### To run performace test on windows:

**Type intersect**:
```
Measure-Command { start-process npm 'run tsc10k' -wait}
```

**Interface extend**:
```
Measure-Command { start-process npm 'run tsci10k' -wait}
```


### To run performace test on linux/macOs:

**Type intersect**:
```
time npm run tsc10k
```

**Interface extend**:
```
time npm run tsci10k
```
