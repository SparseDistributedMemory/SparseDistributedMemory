---
layout: page
title: about
permalink: /about/
---

![sdm.jpeg](/sdm.jpeg)


> How is memory gradually built up during one’s conscious, or even unconscious,
> life and thought? My guess is that everything we experience is classified and
> registered on very many parallel channels in different locations.  
> __Stanislaw Ulam__




---
> Pentti Kanerva’s memory model was a revelation for me: it was
> the very first piece of research I had ever come across that made
> me feel I could glimpse the distant goal of understanding how the
> brain works as a whole. It gave me a concrete sense for how
> familiar mental phenomena could be thought of as distributed
> patterns of micro-events, thanks to beautiful mathematics.   
> __Douglas Hofstadter__




---
> The emphasis might have been on the breadth of topics, in
> detriment of depth here or there. The work on, say, reinforcement
> learning, is most definitely not the last word we will see on the
> subject, but a challenge left for readers to contemplate. But
> this is due to our research group’s enthusiasm for the topic; we
> do indeed believe that SDM is — if not correct — extremely close
> to a full scientific understanding of human long-term memory. If
> so, it is such a monumental achievement that we want readers to
> be able to see all of what we see and imagine the vastness of
> possibilities.
>
> Ralph Waldo Emerson once said: _do not go where the path may
> lead. Go, instead, where there is no path, and leave a trail_.
> Professor Pentti Kanerva has left the trail. It is my job to
> illuminate it and to pave it and to clear it; to try to deliver
> an easier pathway for the next generation. Some essays
> completely shut the door close at the end; this one intends to
> leave it wide open. As the reader might have noticed, this final
> section does not read as an analysis of the work done; it reads,
> instead, as a desideratum, a prologue, a yearning for others to
> join me in imagining the shape of things to come.  
> __Marcelo S. Brogliato__

---

### Welcome to sdm.ai.  

Exploring the AI potential of _Sparse Distributed Memory_.

Here you will find all sorts of resources to start (or enhance) your research (or industrial) work on models related to Pentti Kanerva's Sparse Distributed Memory.

Some things are as silly as a small jupyter notebook, toying around with some experiment, or with the mathematics of SDM. Others include a full-blown massively parallel GPGU Cross-platform open-source buzzword-complete framework.   



### here's our desiderata:

     * A massively parallel framework in which users can test cognitive neuroscience theories;
     * a full documentation of the framework;
     * An open-source book, with a visual tutorial of the system, its relation to neuroscience and psychology, and numerous new scientific results;
     * A collection of SDM resources, links, chronology of papers, etc;
     * Slides following the Jupyter notebooks used;
     * A video-based mini-course on SDM.

---




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
