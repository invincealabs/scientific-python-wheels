# scientific-python-wheels
A set of pre-built binary wheels for Scientific Python (numpy, scipy, sklearn) on Linux

## Why

Distributing projects that use numpy, scipy, and sklearn can be a
pain if you don't want to use Conda (for which there are
occasionally legitimate reasons), because there are no binary
wheels for Linux that properly embed the required shared object
libraries.

The wheels in this repository do just that. Each project is
compiled with OpenBLAS/LAPACK, and the required shared libraries
are baked into the wheels in the `_lib` directory with runtime
paths adjusted so that they load properly. 

## How do I get them?

Look in the release tab.

## License

Each of these wheels is licensed according to the respective
licenses of the projects they are built from.

+ [OpenBLAS](https://github.com/xianyi/OpenBLAS/blob/develop/LICENSE)
+ [LAPACK](http://www.netlib.org/lapack/LICENSE.txt)
+ [numpy](https://github.com/numpy/numpy/blob/master/LICENSE.txt)
+ [scipy](https://github.com/scipy/scipy/blob/master/LICENSE.txt)
+ [sklearn](https://github.com/scikit-learn/scikit-learn/blob/706b45e03e0a4e8aae08560853eba7b6c4853b5b/setup.py#L36)
