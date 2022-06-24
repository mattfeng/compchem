# Gaussian

## ChemCraft

**ChemCraft can run on an M1 Mac, but it will be very slow because it is will be executed via a Docker container that is running on an emulated x86_64 Linux kernel.**

```bash
sudo apt-get install xorg libgtk2.0-0
```

```
# host machine
socat TCP-LISTEN:6000,reuseaddr,fork UNIX-CLIENT:\"$DISPLAY\"
```

## 
