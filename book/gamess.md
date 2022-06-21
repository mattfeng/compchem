# GAMESS

## Installing GAMESS on AWS EC2

### Install dependencies

```bash
sudo apt-get install csh make cmake gfortran libopenblas64-dev
```

### Download GAMESS and extract it
```bash
tar -xvf gamess-current.tar.gz
```

### Configure installation
```bash
cd ~/gamess
./config
```

Choose the following options:
* LibXC? `yes`
* DDI communication method: `sockets`

### Download and compile LibXC
```bash
~/gamess $ ./tools/libxc/download-libxc.csh
```
