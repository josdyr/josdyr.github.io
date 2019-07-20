---
layout: home
title:  "Evolutionary Algorithms"
date:   2019-04-20 21:09:45 +0100
categories: blog
permalink: blog/:title
intro: "This is an intro to how EA work and their best practises."
---
<div class="container">
  <h1>{{page.title }}<br></h1>
  <i>{{page.date | date_to_long_string}}<br></i>
  Definition: Evolutionary Algorithms are a randomly generated population of solutions that gradually evolves to improve a fitness of the population.

  Usually they have a common generic algorithm that looks something like this:
  /Initialise Population/
  /Loop/
  /Select Parents/
  /Combine Parents to Create Offspring Mutate Offspring (small probability) Replace Into Population/
  /Until Termination Condition/

  An EA is a multi point stochastic search inspired by *Darwinian evolution*. A randomly generated *population*of solutions gradually evolves to improve the *fitness*of the population. The “fitter” individuals in the population survive to make future generations. (*survival of the fittest*).

  Later Darwin said: “It is not the strongest of the species that survives, nor the most intelligent, but the one most responsive to change” (Darwin, 1809)<br>

</div>
