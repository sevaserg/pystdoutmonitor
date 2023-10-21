# pystdoutmonitor
This module is a wrapper for strace and pidof. It launches a distinct thread and calls a user-defined callback each time it captures an output.
## Example:
```python
from stdoutmonitor import StdoutMonitorProcess

def cb(line):
    print(line)

s = StdoutMonitorProcess("someProgram", cb)
while True:
    None
```
