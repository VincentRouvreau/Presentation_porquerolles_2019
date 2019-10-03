% GUDHI - Porquerolles 2019
% Vincent Rouvreau
% 14 october 2019

# What's new

## GitHub

> - [GUDHI organization](https://github.com/GUDHI)
    - gudhi-devel
    - TDA-tutorial
    - Web site
> - [Issue tracker](https://github.com/GUDHI/gudhi-devel/issues)
> - [Code reviews on pull requests](https://github.com/GUDHI/gudhi-devel/pulls)

## MIT

> - GUDHI moved from a GPL v.3 license to MIT in order to ease the contributions.
> - There are still GPLv3 and LGPL dependencies for many modules (Alpha complex, Bottleneck, ...).


## Sparse Rips complex python version

[https://gudhi.inria.fr/python/latest/rips_complex_user.html](https://gudhi.inria.fr/python/latest/rips_complex_user.html)

~~~python
import gudhi
rips_complex = gudhi.RipsComplex(off_file='torus_3d.off',
                                 sparse=0.3)
simplex_tree = rips_complex.create_simplex_tree()
simplex_tree.persistence()
~~~

## Persistence density graphical tool (1/2)

[https://www.nature.com/articles/ncomms15082](https://www.nature.com/articles/ncomms15082)

~~~python
import gudhi
persistence_file='rips_on_tore3D_1307.pers'
plt = gudhi.plot_persistence_density(
    persistence_file=persistence_file,
    max_intervals=0, dimension=1, legend=True)
plt.show()
~~~

## Persistence density graphical tool (2/2)

![Persistence density graphical tool](http://gudhi.gforge.inria.fr/python/latest/_images/persistence_graphical_tools_user-3.png)


# What's next

## Strong collapse

Certaines choses n'existent pas nativement en *Pandoc Markdown*, il suffit donc
d'utiliser du \LaTeX.

## sklearn-tda

\begin{alertblock}{Alerte}
Ceci est une alerte
\end{alertblock}

\begin{exampleblock}{Exemple}
Ceci est un exemple
\end{exampleblock}

## Wasserstein distance

Les images sont supportées par *Markdown*, mais on ne peut pas spécifier la
taille. Il est donc pratique d'utiliser directement \LaTeX.

----

\center\includegraphics[height=6.5cm]{croissance.jpg}

## Exact d-Alpha complex

Avec des formules :

$$
\frac{\pi}{4}=\int_0^1 \sqrt{1-x^2}\mathrm dx
$$

# Notebooks

## Notebooks

    sudo apt-get install pandoc \
                         texlive-latex-base \
                         texlive-latex-extra \
                         texlive-lang-french \
                         latex-beamer \
                         impressive
    git clone http://git.rom1v.com/mdbeamer.git
    cd mdbeamer
    make run

## DTM-filtration

----------- ----------------------------
  la source \code{slides.md}

   le thème \code{beamerthemeCustom.sty}
----------- ----------------------------

# Benchmarks

## No threshold

\scriptsize

pandoc
  ~ <http://johnmacfarlane.net/pandoc/demo/example9/pandocs-markdown.html>
pour beamer
  ~ <http://johnmacfarlane.net/pandoc/demo/example9/producing-slide-shows-with-pandoc.html>
en français
  ~ <http://enacit1.epfl.ch/markdown-pandoc/>
