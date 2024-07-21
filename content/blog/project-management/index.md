---
title: Simulating a random dynamical system
summary: A network model of a bacterial population with phenotypic switching, and some results from this model abou the asymtpotic growth rate of the bacteria.
date: 2021-10-23
authors:
  - admin
tags:
  - Simulations
  - Dynamical systems
image:
  caption: 'Power law properties of the dynamical system'
---

Developing numerical simulations of a random dynamical system to depict intermittency and ergodicity breaking in some parameter regimes. Here is the [code](https://github.com/moitrishm/randomdynamicalsystem) I developed for this project and the subsequent [journal publication](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=v2wuOnoAAAAJ&citation_for_view=v2wuOnoAAAAJ:u5HHmVD_uO8C).

## Description

We analysed the behaviour of a random map [1], which can be used to model random processes like Brownian motion. 

The probabilistic parameter p influences the behaviour of the map [2]. Due to the mod1 operation, we lose one bit of data at every iteration. Hence, we simulated the map using the [MPFR](https://www.mpfr.org/) package for arbitrary precision computation.
We calculated the autocorrelation functions for the map at different parameter values and observed the decay in the function. We also computed other observables to capture ergodicity breaking, which occurs at certain p values.

## Background

I worked on this project as a part of a [summer research school](https://indico.ictp.it/event/9545/) 
organised by the London Mathematical Laboratory and the Abdus Salam International Center for
Theoretical Physics. [Dr. Yuzuru Sato](https://www2.sci.hokudai.ac.jp/dept/math/en/researcher/sato-yuzuru-2), 
[Dr. Rainer Klages](https://webspace.maths.qmul.ac.uk/r.klages/) and [Dr. Stefano Ruffo](https://www.statphys.sissa.it/wordpress/?page_id=6599) were my supervisors. 


I presented the preliminary results of this project as a talk at the end of the summer school, in July 2021.

{{< youtube PT2mHZ4U7YM >}}

## References

[1] <cite><a href="https://www.ams.org/journals/tran/1984-281-02/S0002-9947-1984-0722776-1/S0002-9947-1984-0722776-1.pdf">Pelikan, Stephan. "Invariant densities for random maps of the interval." Transactions of the American Mathematical Society 281.2 (1984): 813-825. </a></cite> 
<br/>
<br/>
[2] <cite><a href="https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.122.174101"> Sato, Yuzuru, and Rainer Klages. "Anomalous diffusion in random dynamical systems." Physical review letters 122.17 (2019): 174101. </a></cite>
<br/>

## Did you find this page helpful? Consider sharing it 🙌
