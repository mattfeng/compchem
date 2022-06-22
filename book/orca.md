# ORCA

- [ORCA 5.0.3 manual](../orca/ref/orca_manual_5_0_3.pdf)

## Installation

### Ubuntu 20.04 LTS (Linux)

```bash
/home/ubuntu$ tar -xvf orca_5_0_3_linux_x86-64_shared_openmpi411.tar.xz
/home/ubuntu$ mv orca_* orca503

# add dynamic library to linux loader directory
/home/ubuntu$ sudo cp orca503/liborca_tools_5_0_3.so.5 /usr/lib/x86_64-linux-gnu
```

