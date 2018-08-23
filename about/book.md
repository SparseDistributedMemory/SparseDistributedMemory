---
layout: page
title: Book
permalink: /about/book/
---

![sdm.jpeg](sdm.jpeg)

#  sdm.ai  
We're working on a book on _Sparse Distributed Memory_.



Desiderata:
 * A massively parallel framework in which users can test cognitive neuroscience theories;
 * a full documentation of the framework;
 * An open-source book, with a visual tutorial of the system, its relation to neuroscience and psychology, and numerous new scientific results;
 * A collection of SDM resources, links, chronology of papers, etc;
 * Slides following the Jupyter notebooks used;
 * A video-based mini-course on SDM.








### Sparse Distributed Memory Framework
This is a framework which can be adapted to any usage of a Sparse Distributed Memory (Kanerva, 1988):  new theoretical results, new applications, new machine learning models, etc.  

 We have been working on Pentii Kanerva's Sparse Distributed Memory:
   - The first [paper considered the range of dimensions that an SDM should have were it to respect i) chunking-by-averaging, and ii) the "magic number 7"](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0015592);
   - a second [paper studied the critical distance as the memory becomes saturated](http://journal.frontiersin.org/article/10.3389/fnhum.2014.00222/full);
   - a third paper (underway) studies interaction effects between different attractors, and
   - a fourth paper will document this [highly-palallel SDM framework](https://github.com/msbrogli/sdm-framework) developed by [Dr. Marcelo Brogliato](https://github.com/msbrogli).  

We would really like to ask you for feedback, and, should you find it useful, please consider a link or citation:

Brogliato, M.S.; Linhares, A. (2017) Sparse Distributed Memory: a reference implementation.  Working Paper, FGV, Vialink.


#### How to build & test
To generate the library and run some tests:

    cd src/
	make
	make tests
	./test1

To run Python tests:

	python tests.py

In dev mode, there should be a symbolic link from `src/libsdm.so` to `sdm/_libsdm.so`. If it does not exist, create one running:

	cd sdm/
	ln -s ../src/libsdm.so _libsdm.so


#### How to install
This framework has the following dependencies: `libbsd` and `libOpenCL`.
