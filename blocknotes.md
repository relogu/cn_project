# Project of Complex Networks

Interesting repositories:

1. [Elisa Mussumeci, modeling news spread](https://github.com/elisamussumeci/modeling-news-spread);
2. [William L. Hamilton, social LSTMs to predict intercommunity-conflict](https://github.com/williamleif/social-lstm).

Dataset web-pages: [SNAP official project page](http://snap.stanford.edu/conflict/); [body](https://snap.stanford.edu/data/soc-redditHyperlinks-body.tsv), [title](https://snap.stanford.edu/data/soc-redditHyperlinks-title.tsv) **put these in PATH_TO_REPO/data**.
To understand what LIWC (found in the explanation about the dataset), look [here](https://www2.fgw.vu.nl/werkbanken/dighum/tools/tool_list/liwc.php).

Python ODE Solvers: [Python Numerical Methods](https://pythonnumericalmethods.berkeley.edu/notebooks/chapter22.06-Python-ODE-Solvers.html).

To use git: [git - the simple guide](https://rogerdudler.github.io/git-guide/).

To use GitHub: [GitHub Tutorial - Beginner's Training Guide](https://www.youtube.com/watch?v=iv8rSLsi1xo).

To use conda(/mamba): [Master the basics of Conda environments in Python](https://www.youtube.com/watch?v=1VVCd0eSkYc).

Libraries for networks' analysis:

1. [NetworkX](https://networkx.org/);
2. [cuGraph](https://github.com/rapidsai/cugraph).

File [conda_cn_env.txt](https://github.com/relogu/cn_project/blob/master/conda_cn_env.txt) provides the list of the packages to create the conda environment.
This list has been generated using:

```bash
conda list --explicit > conda_cn_env.txt
```

File [pip_cn_env.txt](https://github.com/relogu/cn_project/blob/master/pip_cn_env.txt) provides the list of the packages to install via `pip` to complete the conda environment.
This list has been generated using:

```bash
pip freeze > pip_cn_env.txt
```

In order to create a conda environment from this file open a terminal and use the command:

```bash
conda create --name cn-env --file conda_cn_env.txt; pip install -r pip_cn_env.txt 
```

The whole environment should take ~11GB disk space.

TODO: Media Cloud etc..
