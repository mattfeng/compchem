# OpenBabel

- Documentation for version 3.0.1: https://open-babel.readthedocs.io/en/latest
  - Github repository of OpenBabel documentation: https://github.com/openbabel/documentation

## Optimize geometry

```bash
$ obabel <input.cml> -O <optimized-out.cml> --minimize --ff uff

# source: https://archive.ph/RoNWP
```

* `obabel --minimize` is newer than the original `obminimize` command.
  - `obabel --minimize` added in 2012, `obminimize` in 2007.
  - source: https://archive.ph/tVKqi

- `-O`: Specify an output file.
- `--ff`: Select a forcefield to use. `uff` is the **Universal Forcefield**.
  - You can find all possible forcefields using `obabel -L forcefields` (`obabel -L` lists plugin classes).
