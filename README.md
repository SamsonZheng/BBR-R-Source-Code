The paper related to this code has been accepted by the conference Computer Networks.
# BBR-R
## Envs
os : Ubuntu 20/18，linux kernel-4.146-mptcp

## usage

### clone the repo
```
git clone https://github.com/opendev2020/tcp_ql.git
```

### build
```
make all
```

### insert the module
```
sudo insmod tcp_satcc.ko
```

### set satcc as the current congestion control algorithm
```
sysctl net.ipv4.tcp_congestion_control=bbr_r
```
