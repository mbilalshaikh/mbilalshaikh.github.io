---
published: false
---
## Exporting conda environments

* on real package machine
```
conda env export --no-builds | grep -v "prefix" > environment.yml
```

* on deployment machine
```
conda env create -f environment.yml
```

