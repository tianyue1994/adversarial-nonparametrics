# Nonparametric Adversarial Attack and Defense

## Install

### Dependencies
```
pip install --upgrade -r requirements.txt
```

#### LP, QP Solvers
Install gruobi: https://www.cvxpy.org/install/index.html#install-with-gurobi-support
Install GLPK: https://www.cvxpy.org/install/index.html#install-with-cvxopt-and-glpk-support

### Install C-extensions
```
./setup.py build_ext -i
```

### for robust splitting
```
pip install --upgrade ./scikit-learn
```

## Example

```
python ./main.py --dataset halfmoon_300 --model knn3 \
                 --attack rev_nnopt_k3_50_region --random_seed 0 --ord inf
```
