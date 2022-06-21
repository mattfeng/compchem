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
* Platform: `linux64`
* Installation directory: `/home/ubuntu/gamess`
* GAMESS build location: `/home/ubuntu/gamess`
* GAMESS version number: `00`
* LibXC? `yes`
* DDI communication method: `sockets`

### Download and compile [Libxc](https://tddft.org/programs/libxc/)

Libxc is a library of exchange-correlation and kinetic energy functionals for density-functional theory.

Current reference for Libxc: https://www.sciencedirect.com/science/article/pii/S2352711017300602.

```bash
~/gamess $ ./tools/libxc/download-libxc.csh
```

### Compile modules

```bash
make modules
```

### Compile GAMESS

```bash
make -j$((`nproc` - 1))
```
