# A Kernel Seedling
Create a /proc/count file that shows the current number of running processes (or tasks) running.

## Building
```shell
make
```

## Running
```shell
insmod proc_count.ko
cat /proc/count
```
results:
161

## Cleaning Up
```shell
make clean
```

## Testing
```python
python -m unittest
```
results:
Ran 3 tests in 1.089s

OK

Report which kernel release version you tested your module on
(hint: use `uname`, check for options with `man uname`).
It should match release numbers as seen on https://www.kernel.org/.

```shell
uname -r -s -v
```
kernel ver:
Linux 5.14.8-arch1-1 #1 SMP PREEMPT Sun, 26 Sep 2021 19:36:15 +0000 x86_64 GNU/Linux
