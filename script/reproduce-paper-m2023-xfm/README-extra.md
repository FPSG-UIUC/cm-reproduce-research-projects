# CM script to run and reproduce experiments

Original repository: https://github.com/neel-patel-1/XFM_MICRO2023.git

### Reusability using MLCommons CM automation language

Install MLCommmons CM using [this guide](https://github.com/mlcommons/ck/blob/master/docs/installation.md).

Install reusable MLCommons automations: 

```bash
cm pull repo mlcommons@ck
```

Install this repository with CM interface for reproduced experiments:
```bash
cm pull repo ctuning@cm-reproduce-research-projects
```

### Run XFM via CM interface

1) Install deps:
```bash
cmr "reproduce project micro-2023 xfm _install_deps"
```

2) Run experiments:

```bash
cmr "reproduce project micro-2023 xfm _run" 
```

3) Plot results:

```bash
cmr "reproduce project micro-2023 xfm _plot"
```

You should find `XFM_Access_Distribution.png` and `results.csv` in the `results` folder current directory.
