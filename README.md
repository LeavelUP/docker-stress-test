# docker-stress-test
Stress-ng creates sudo-processes to stress hardware

## breakdown
* stress-ng is the command
* --cpu *n* dispatches *n* hogs that target CPU cores
  * dispatching 16 maximizes stress on each core
* --vm *n* creates *n* 256mb processes that strain RAM
  * creating 125 processes stresses all 32Gb of available RAM
