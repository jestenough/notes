# Linux

## SSD optimizations

As root:
```
fstrim --all
systemctl enable fstrim.timer
```