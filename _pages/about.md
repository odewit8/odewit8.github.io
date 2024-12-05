---
permalink: /
title: "Front page"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<h1>About me</h1>
<p style='text-align: justify;'> 
I am currently a final year PhD student at the University of Cambridge. In Cambridge, I am affiliated with the Department of Applied Mathematics and Theoretical Physics  (<a href="https://www.damtp.cam.ac.uk/">DAMTP</a>). In Oxford, I am a Recognised Visiting Student at the <a href="https://www.maths.ox.ac.uk/">Mathematical Institute</a>, where my PhD supervisor is, <a href="https://people.maths.ox.ac.uk/bruna/">Maria Bruna</a>.

<h1>Research</h1>
<p style='text-align: justify;'> 
I am interested in mathematically understanding the emergence of collective behaviour in groups of animals. Examples of this emergence are lane formation in groups of ants or pedestrians, or flocking in birds.
</p>
<iframe src="https://giphy.com/embed/KJQva3zYQ2rni" width="480" height="269" style="" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/tokyo-crossing-shibuya-KJQva3zYQ2rni">Street crossing in Tokyo</a></p>
<p style='text-align: justify;'> 
I specialize in studying these phenomena using
<ul>
  <li>Stochastic differential equations (SDEs) and </li>
  <li>Partial differential equations (PDEs).</li>
</ul> 

Particularly, I am interested in modelling large collectives of animals as stochastic interacting particle systems and study them in the <em>mean-field</em> limit. This limit gives a description of the particle model by going from the \(N\times d\)-dimesional SDE model to a \(d\)-dimensional PDE model, called the <em>mean-field limit PDE</em>, by taking the number of particles to infinity, \(N\to\infty\). Using the mean-field limit PDE, particle behaviours like lane formation can be studied as a PDE dynamics.

Schematically, I consider systems of SDEs which can be written as

$$ \mathrm{d}\mathbf{X}_t^i=\sum_{j\neq i}\mathbf{b}(\mathbf{X}_t^i,\mathbf{X}_t^j)\mathrm{d}t+\sqrt{2}\mathrm{d}\mathbf{W}_t^i, \ i=1,\dots,N$$

for some drift function \(\mathbf{b}\). In the mean-field limt the $k$-marginals of the law \(f^{(k)}_t(t,\mathbf{x}_i)\) converge to a tensorised product of \(f(t,\mathbf{x})\), in some metric topology, for any $k$,

$$ d(f^{(k)}_t,f(t)^{\otimes k})\to 0 \ \mathrm{as} \ N\to\infty.$$

The density \(f\) is a solution of the mean-field limit PDE and is, in this case, of the form 

$$ \partial_t f=\nabla\cdot[\nabla f-\mathbf{b} f].$$

With the SDEs and PDEs that describe collective behaviour in mind, I focus on
<ul>
  <li>PDE analysis (well-posedness, (non)linear stability, bifurcations),</li>
  <li>Numerical PDE and SDE schemes,</li>
  <li>Numerical analysis,</li>
  <li>Rigorous mean-field limits,</li>
  <li>Parameter inference from data for SDEs.</li>
</ul> 

In my work I have studied a SDE model for lane forming ants, together with my co-authors (see <a href="https://odewit8.github.io/publications/">Publications</a> for a link to the paper). We found the following two typical behaviours.
</p>

<p align="middle">
  <img src="images/clusters.gif" width="250" />
  <img src="images/clusters2.gif" width="250" /> 
</p>

<!-- <p align="middle">
  <img src="images/output.gif" width="400" />
  <img src="images/output2.gif" width="400" /> 
</p> -->
