The paper related to this code has been accepted by the conference Computer Networks.  

If you want to personally try injecting BBR-R into the Linux kernel and test its performance, you can follow the instructions below.  
：）

# BBR-R
## Envs
os : Ubuntu 20/18，linux kernel-4.146-mptcp

## usage

### clone the repo
```
git clone https://github.com/SamsonZheng/BBR-R-Source-Code.git
```

### build
```
cd BBR-R
make all
```

### insert the module
```
sudo insmod bbr_r.ko
```

### set bbr-r as the current congestion control algorithm
```
sysctl net.ipv4.tcp_congestion_control=bbr_r
```
