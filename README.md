# gaus-bin-dist

This package contains modules for working with Gaussian and Binomial Distributions.

## Files

* `gaus_bin_dist/`: Distributions package
  * `Binomialdistribution.py`: Binomial class
  * `Gaussiandistribution.py`: Gaussian class
  * `Generaldistribution.py`: Distribution class
  * `__init__.py`: Initialization script
* `license.txt`: MIT license
* `numbers.txt`: Test file for Gaussian class
* `numbers_binomial.txt`: Test file for Binomial class
* `setup.cfg`: Configuration file for code packaging
* `setup.py`: Script for code packaging
* `test.py`: Unit tests

## Installation

Download on [PyPi](https://pypi.org/project/gaus-bin-dist/) or use following command:

`pip install gaus-bin-dist`

## Python Interpreter Example

### Initialization
```python
>>> from gaus_bin_dist import Gaussian, Binomial
>>> Gaussian(10, 7)
mean 10, standard deviation 7
>>> Binomial(0.4, 25)
mean 10.0, standard deviation 2.449489742783178, p 0.4, n 25
```

### Addition
```python
>>> gaussian_one = Gaussian(25, 3)
>>> gaussian_two = Gaussian(30, 4)
>>> gaussian_one + gaussian_two
mean 55, standard deviation 5.0
>>> binomial_one = Binomial(0.4, 20)
>>> binomial_two = Binomial(0.4, 60)
>>> binomial_one + binomial_two
mean 32.0, standard deviation 4.381780460041329, p 0.4, n 80
```

### Probability Density Function
```python
>>> gaussian_one.pdf(25)  # gaussian_one PDF at x = 25
0.1329807601338109
>>> binomial_one.pdf(5)  # binomial_one PDF at x = 5
0.07464701952887093
```
