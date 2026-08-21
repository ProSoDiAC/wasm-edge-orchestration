# Energy records

Paired idle/active cycles and the workload-size sweep behind the energy figure
and the workload CPU-time table.

`workload-size-and-idle-active.json` is the combined dataset the paper reports:
one point per workload size $N$, each carrying the mean CPU time per call with
its interval, the load and idle CPU seconds, and the Kepler-attributed watts.
`pass1.json` and `pass2.json` are the two collection passes it is assembled
from; the combined file records which pass each point came from.

The wattage is a regression estimate, not a measurement: the host exposes no
RAPL counters, which is why the paper treats CPU time as the primary quantity
and the wattage as a secondary signal consistent with it.
