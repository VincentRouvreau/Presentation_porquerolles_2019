% GUDHI - Porquerolles 2019
% Vincent Rouvreau
% 14 october 2019

# What's new

## GitHub

\vspace{-1.5cm}
> - [GUDHI GitHub organization](https://github.com/GUDHI)
> - [Issue tracker](https://github.com/GUDHI/gudhi-devel/issues)
> - [Code reviews on pull requests](https://github.com/GUDHI/gudhi-devel/pulls)

## MIT

\vspace{-1.5cm}
> - GUDHI moved from a GPL v.3 license to MIT in order to ease the contributions.
> - There are still GPLv3 and LGPL dependencies for many modules (Alpha complex, Bottleneck, ...).


## Sparse Rips complex python version

\vspace{-1.5cm}
[https://gudhi.inria.fr/python/latest/rips_complex_user.html](https://gudhi.inria.fr/python/latest/rips_complex_user.html)

~~~python
import gudhi
rips_complex = gudhi.RipsComplex(off_file='torus_3d.off',
                                 sparse=0.3)
simplex_tree = rips_complex.create_simplex_tree()
simplex_tree.persistence()
~~~

## Persistence density graphical tool (1/2)

\vspace{-1.5cm}
[https://www.nature.com/articles/ncomms15082](https://www.nature.com/articles/ncomms15082)

~~~python
import gudhi
persistence_file='rips_on_tore3D_1307.pers'
plt = gudhi.plot_persistence_density(
    persistence_file=persistence_file,
    max_intervals=0, dimension=1, legend=True)
plt.show()
~~~

----

\vspace{-1.5cm}
\center\includegraphics[height=5.5cm]{persistence_graphical_tools_user-3.png}

# What's next

## Strong collapse

\vspace{-1.5cm}
\center\includegraphics[height=4.9cm]{strong_collapse.png}


## sklearn-tda

\vspace{-1.5cm}


## Wasserstein distance

\vspace{-1.5cm}


## Exact d-Alpha complex

\vspace{-1.5cm}


# Notebooks

## Notebooks

\vspace{-1.5cm}

# Benchmarks

## No threshold

\vspace{-1.5cm}
