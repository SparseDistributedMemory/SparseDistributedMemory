#  sdm.ai:  Explorations into the AI capabilities of Sparse Distributed Memory




Sparse Distributed Memory Framework
===================================
This project intends to be a framework which can be adapted to any usage of a Sparse Distributed Memory (Kanerva, 1988).  

 We have been working on Pentii Kanerva's Sparse Distributed Memory:
   - The first [paper considered the range of dimensions that an SDM should have were it to respect i) chunking-by-averaging, and ii) the "magic number 7"](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0015592);
   - a second [paper studied the critical distance as the memory becomes saturated](http://journal.frontiersin.org/article/10.3389/fnhum.2014.00222/full);
   - a third paper (underway) studies interaction effects between different attractors, and
   - a fourth paper will document this [highly-palallel SDM framework](https://github.com/msbrogli/sdm-framework) developed by [PhD Candidate Marcelo Brogliato](https://github.com/msbrogli).  

We would really like to ask users for feedback, and, should they find it useful, a link or citation:

Brogliato, M.S.; Linhares, A. (2017) Sparse Distributed Memory: a reference implementation.  Working Paper, FGV, Vialink.


How to build & test
===================
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


How to install
==============
This framework has the following dependencies: `libbsd` and `libOpenCL`.
