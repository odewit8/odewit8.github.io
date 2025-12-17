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
I am currently a postdoc at the <a href="https://math.univ-lyon1.fr/icj/">Institut Camille Jordan</a> at the Université Claude Bernard Lyon 1.
</p>

<p style='text-align: justify;'> 
The title of my PhD thesis is <em>Collective behaviour of active particles with mean-field interaction</em>. I did my PhD at the University of Cambridge, where I was affiliated with the Department of Applied Mathematics and Theoretical Physics  (<a href="https://www.damtp.cam.ac.uk/">DAMTP</a>), under supervision of <a href="https://people.maths.ox.ac.uk/bruna/">Maria Bruna</a>. In 2024-2025, I was a Recognised Visiting Student at the <a href="https://www.maths.ox.ac.uk/">Mathematical Institute</a> at the University of Oxford.</p>

<h1>Research</h1>
<p style='text-align: justify;'> 
I am interested in mathematically understanding the emergence of collective behaviour. Examples of this emergent behaviour are lane formation in groups of ants or pedestrians, or flocking in birds.
</p>
<iframe src="https://giphy.com/embed/KJQva3zYQ2rni" width="480" height="269" style="" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/tokyo-crossing-shibuya-KJQva3zYQ2rni">Street crossing in Tokyo</a></p>
<p style='text-align: justify;'> 
I specialize in studying these phenomena using
<ul>
  <li>Stochastic differential equations (SDEs) and </li>
  <li>Partial differential equations (PDEs).</li>
</ul> 

Particularly, I am interested in modelling large collectives of animals as stochastic interacting particle systems and studying them in the <em>mean-field</em> limit. This limit gives a description of the particle model by going from the \(N\times d\)-dimesional SDE model to a \(d\)-dimensional PDE model, called the <em>mean-field limit PDE</em>, by taking the number of particles to infinity, \(N\to\infty\). Using the mean-field limit PDE, particle behaviours like lane formation can be studied as a dynamics of this mean-field limit PDE.
</p>
<p style="text-align: justify; border: 2px solid black; padding: 0.5em"> 
Schematically, I consider \(\mathbb{R}\)-valued systems of SDEs which can be written as

$$ \mathrm{d}\mathbf{X}^{i,N}_t=\mathbf{b}^N(\mathbf{X}^{i,N}_t,\mathbf{X}_t^N)\mathrm{d} t+\sqrt{2}\mathrm{d}\mathbf{W}_t^{i,N}, \ i=1,\dots,N $$

for some drift function \(\mathbf{b}^N\). In the mean-field limit the \(k\)-marginals of the law, \(f^{(k)}_t(t,(\mathbf{x}_i)_i)\), converge to a tensorised product of \(f(t,\mathbf{x})\), in some \(d\)-metric topology, for any \(k\),

$$ d(f^{(k)}_t,f(t)^{\otimes k})\to 0 \ \mathrm{as} \ N\to\infty.$$

In general, this needs to be proven for the specific modelling choice for the drift function \(\mathbf{b}^N\). The limit density \(f\) is a solution of the mean-field limit PDE and is, in this case, of the form 

$$ \partial_t f=\nabla\cdot[\nabla f-\mathbf{b} f],$$
if the limit \(\mathbf{b}=\lim_{N\to\infty} \mathbf{b}^N\) exists.
</p>
<p style='text-align: justify;'> 
With this way that SDEs and PDEs describe collective behaviour in mind, I focus on
<ul>
  <li>PDE analysis (well-posedness, (non)linear stability, bifurcations),</li>
  <li>Developing numerical PDE and SDE schemes,</li>
  <li>Numerical analysis of these schemes,</li>
  <li>Rigorous mean-field limits,</li>
  <li>SDE parameter inference from data.</li>
</ul> 

In my work I have studied a model for lane forming ants, together with my co-authors (see <a href="https://odewit8.github.io/publications/">Publications</a> for a link to the paper). 
</p>
<!-- We found the following two typical behaviours.
<p align="middle">
  <img src="images/clusters.gif" width="300" />
  <img src="images/clusters2.gif" width="300" /> 
</p>

<!-- <p style='text-align: justify;'> 
The first is an aggregation type behaviour. The second is the formation of a traveling cluster. In the paper we explain how this is related to lane formation and ant antennas.
</p> -->

<p style='text-align: justify;'> 
An interesting feature of the PDE for our ant model, and of many other PDEs used to study models of so-called <em>active matter</em> such as groups of ants, birds and pedestrians, is that the PDE is different from a particular class of PDEs for which a substantial level of understanding has been achieved. This is the class of PDEs that can be written in the form 

$$ \partial_t f=\nabla\cdot\left(f\nabla\frac{\delta\mathcal{F}}{\delta\mathcal{f}}\right),$$

where \(\mathcal{F}\) is a functional of \(f\). These are PDEs that can be described as a <em>gradient flow</em> and the functional \(\mathcal{F}\) can be used to describe the PDE dynamics via a LaSalle Invariance Principle (see, for example, this <a href="https://doi.org/10.1016/j.jde.2022.11.028">paper</a>).
</p>

<p style='text-align: justify;'> 
In our case, for active matter PDE models, the PDE cannot be of this form, because the curl of the drift function \(\mathbf{b}\) is non-zero in our model. To give an example of how gradient flow dynamics can be different from a model that is not of the above form, we can consider the following two linear models. The first model has a mean-field limit PDE of the form

$$ \partial_t f=\nabla\cdot[\nabla f-\nabla V f], $$

where we have exponential relaxation to the unique normalised steady state \(f_\infty(\mathbf{x})=\frac{1}{\int\mathrm{e}^V\mathrm{d}x}\mathrm{e}^{V(\mathbf{x})}\) for some potential \(V(\mathbf{x})\), and the second model is 

$$ \partial_t f=\nabla\cdot[\nabla f-(\nabla V+ \mathbf{U})f], $$

such that the perturbation \(\mathbf{U}\) satisfies \(\nabla\cdot\mathbf{U}=0\) and \(\mathbf{U}\perp\nabla V\), so that the steady state is preserved. The typical particle behaviour for these models is quite different. In the below videos, the grey background hue is the amplitude of the steady state potential \(V(\mathbf{x})\).
</p>

<p align="middle">
  <img src="images/lineargf.gif" width="300" />
  <img src="images/linearngf.gif" width="300" /> 
</p>

<p style='text-align: justify;'> 
In general, I am interested in studying these type of active matter models to understand emergent collective behaviours.
</p>
