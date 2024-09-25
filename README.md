The paper related to this code has been accepted by the conference Computer Networks.  

If you want to personally try injecting BBR-R into the Linux kernel and test its performance, you can follow the instructions below.  
：)

# BBR-R
## Envs
OS: Ubuntu 20/18，Linux kernel-4.146-mptcp

## Usage

### Clone the repo
```
git clone https://github.com/SamsonZheng/BBR-R-Source-Code.git
```

### Build the module
```
cd BBR-R
make all
```

### Insert the module
```
sudo insmod bbr_r.ko
```

### Set BBR-R as the current congestion control algorithm
```
sysctl net.ipv4.tcp_congestion_control=bbr_r
```
