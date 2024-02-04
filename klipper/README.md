# Notes

## Probe Accuracy

G28 -> QGL x2

### Cold

```
Send: PROBE_ACCURACY
Recv: // PROBE_ACCURACY at X:147.000 Y:150.000 Z:30.000 (samples=10 retract=3.000 speed=10.0 lift_speed=10.0)
Recv: // probe at 147.000,150.000 is z=3.857500
Recv: // probe at 147.000,150.000 is z=3.863750
Recv: // probe at 147.000,150.000 is z=3.863750
Recv: // probe at 147.000,150.000 is z=3.867500
Recv: // probe at 147.000,150.000 is z=3.865000
Recv: // probe at 147.000,150.000 is z=3.865000
Recv: // probe at 147.000,150.000 is z=3.866250
Recv: // probe at 147.000,150.000 is z=3.866250
Recv: // probe at 147.000,150.000 is z=3.865000
Recv: // probe at 147.000,150.000 is z=3.867500
Recv: // probe accuracy results: maximum 3.867500, minimum 3.857500, range 0.010000, average 3.864750, median 3.865000, standard deviation 0.002727
Recv: ok
[...]
Send: PROBE_ACCURACY
Recv: // PROBE_ACCURACY at X:147.000 Y:150.000 Z:6.867 (samples=10 retract=3.000 speed=10.0 lift_speed=10.0)
Recv: // probe at 147.000,150.000 is z=3.860000
Recv: // probe at 147.000,150.000 is z=3.862500
Recv: // probe at 147.000,150.000 is z=3.861250
Recv: // probe at 147.000,150.000 is z=3.861250
Recv: // probe at 147.000,150.000 is z=3.861250
Recv: // probe at 147.000,150.000 is z=3.861250
Recv: // probe at 147.000,150.000 is z=3.862500
Recv: // probe at 147.000,150.000 is z=3.863750
Recv: // probe at 147.000,150.000 is z=3.861250
Recv: // probe at 147.000,150.000 is z=3.861250
Recv: // probe accuracy results: maximum 3.863750, minimum 3.860000, range 0.003750, average 3.861625, median 3.861250, standard deviation 0.000976
Recv: ok
```

### Hot

PARK -> M140 S70 -> M104 S220

Soak for 10 minutes

```
Send: PROBE_ACCURACY
Recv: // PROBE_ACCURACY at X:147.000 Y:150.000 Z:30.000 (samples=10 retract=3.000 speed=10.0 lift_speed=10.0)
Recv: // probe at 147.000,150.000 is z=3.701250
Recv: // probe at 147.000,150.000 is z=3.707500
Recv: // probe at 147.000,150.000 is z=3.708750
Recv: // probe at 147.000,150.000 is z=3.707500
Recv: // probe at 147.000,150.000 is z=3.707500
Recv: // probe at 147.000,150.000 is z=3.707500
Recv: // probe at 147.000,150.000 is z=3.707500
Recv: // probe at 147.000,150.000 is z=3.706250
Recv: // probe at 147.000,150.000 is z=3.705000
Recv: // probe at 147.000,150.000 is z=3.703750
Recv: // probe accuracy results: maximum 3.708750, minimum 3.701250, range 0.007500, average 3.706250, median 3.707500, standard deviation 0.002165
Recv: ok
[...]
Send: PROBE_ACCURACY
Recv: // PROBE_ACCURACY at X:147.000 Y:150.000 Z:6.704 (samples=10 retract=3.000 speed=10.0 lift_speed=10.0)
Recv: // probe at 147.000,150.000 is z=3.700000
Recv: // probe at 147.000,150.000 is z=3.698750
Recv: // probe at 147.000,150.000 is z=3.701250
Recv: // probe at 147.000,150.000 is z=3.698750
Recv: // probe at 147.000,150.000 is z=3.698750
Recv: // probe at 147.000,150.000 is z=3.700000
Recv: // probe at 147.000,150.000 is z=3.698750
Recv: // probe at 147.000,150.000 is z=3.697500
Recv: // probe at 147.000,150.000 is z=3.696250
Recv: // probe at 147.000,150.000 is z=3.696250
Recv: // probe accuracy results: maximum 3.701250, minimum 3.696250, range 0.005000, average 3.698625, median 3.698750, standard deviation 0.001526
Recv: ok
```
