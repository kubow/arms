
GPIO control

```shell
ls /sys/class/gpio/
echo 18 > /sys/class/gpio/export
echo in/out > /sys/class/gpio/gpio18/direction # change input/output
echo 0/1 > /sys/class/gpio/gpio18/value # change 0/1
```