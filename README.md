I already had gcc and related stuff, so that might be a dependency.

after creating example.(i|c|h), I ran the following:

``` bash
sudo apt-get install swig
swig -python example.i   
```

Then created setup.py and ran that:
 
``` bash
python setup.py build_ext --inplace
```

and then could import:

``` python
>>> import example
>>> example.fact(4)
24
```
