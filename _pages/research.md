---
title: "Research - Quantitative Psychology Active Learning Lab"
layout: textlay
excerpt: "The long-term goal of our research is to improve model-based, scientific inference in psychology."
permalink: /research/
---

# Research

An approach towards understanding the underlying mechanisms of behavior is quantitative (or computational) modeling of data from controlled experiments. It aims at gaining detailed insight into the processes behind certain tasks by theorizing and empirically testing functional relationships between task settings (e.g., stimuli) and response. The long-term goal of our research is to improve such model-based, scientific inference in psychology. Reflected in our current and past research, this endeavor can be made in a number of directions, as outlined below.

### Active Learning of Computational Cognition

The method of [active learning](https://en.wikipedia.org/wiki/Active_learning_(machine_learning)) (also known as [optimal experimental design](https://en.wikipedia.org/wiki/Optimal_design)) makes it possible for behavioral scientists to conduct experiments through optimal interaction with subjects towards a clear, quantified inference goal. At every opportunity during an experiment, an active learning algorithm can evaluate all past observations and propose an optimal setting to use subsequently (e.g., stimulus) that maximizes evidence in response for model inference. The full potential of active learning for cognitive modeling research has yet to be investigated. One of our studies extended the method so as to take advantage of the hierarchical structure of a phenomenon under study:

[Kim, W., Pitt, M. A., Lu, Z.-L., Steyvers, M., & Myung, J. I. (2014). A hierarchical adaptive approach to optimal experimental design. *Neural Computation, 26*(11), 2465-2492](https://www.mitpressjournals.org/doi/abs/10.1162/NECO_a_00654).

![]({{ site.url }}{{ site.baseurl }}/images/HADO_Diagram_Verbal.svg){: style="max-width: 490px; float: right; border: 10px"}

This work stems from the observation that, in many problems of scientific modeling in behavioral and neural sciences, it is sensible to assume that the studied phenomenon has hierarchical data-generating structure: Part of it is invariant across a range of conditions (e.g., a certain parametric model), yet part of it varies across individual settings (e.g., a range of parameter values for different individuals). Establishing such higher-level, invariant structure in detail is often a major scientific goal that is yet highly elusive, especially in behavioral experiments, due to the difficulty in obtaining informative data. The paper introduces a general, theoretically justified framework for applying Bayesian adaptive estimation to hierarchical models so that experimental design choices may be optimized for the goal of best inferring either higher-level (e.g., which model is most plausible?) or lower-level (e.g., which parameter values best describe certain individuals?) structure, or both at the same time. The proposed approach has been validated empirically in the context of vision testing in subsequent research ([Gu et al., 2016](http://jov.arvojournals.org/article.aspx?articleid=2516884)). 

To date, most adaptive experiments have relied on myopic, one-step-ahead strategies in which the stimulus on each trial is selected to maximize inference on the next trial only. A lingering question in the field has been how much additional benefit would
be gained by optimizing beyond the next trial. A range of technical challenges has prevented this important question from being addressed adequately. Our study

[Kim, W., Pitt, M.A., Lu, Z.-L., & Myung, J. I. (2017). Planning beyond the next trial in adaptive experiments: A dynamic programming approach. *Cognitive Science, 41*(8), 2234-2252](http://onlinelibrary.wiley.com/doi/10.1111/cogs.12467/full)

applies dynamic programming (DP), a technique applicable for such full-horizon, "global" optimization, to model-based perceptual
threshold estimation, a domain that has been a major beneficiary of adaptive methods. The results provide insight into conditions that will benefit from optimizing beyond the next trial. These findings have general implications for scientific research adopting the method of active learning.

The current research in our lab is focused on (1) applying the method to the estimation of [stop-signal task](http://www.cambridgecognition.com/cantab/cognitive-tests/executive-function/stop-signal-task-sst/) paremeters; and (2) developing an open-source, general-purpose software package for applying the method to a wide range of cognitive modeling experiments. 

### Understanding Computational Models

When first introduced, [neural network (or parallel distributed processing) modeling](https://en.wikipedia.org/wiki/Connectionism) was received as a drastically different approach to theory formalization than traditional, symbol-processing (or box-and-arrow) models. What makes parallel distributed processing (PDP) models attractive is that many neuron-like units interacting through inhibition and excitation can provide insight into not only the end-state of learning but also crucially the learning process itself. That is, PDP models can be used as tools to understand how mastery of an ability or skill is achieved. However, insufficient understanding of PDP models’ inner workings made it difficult for their explanatory value to be rightly appreciated. This is likely one of the major reasons why they are not studied as scientific models as frequently as when they were introduced as a promising paradigm. Our study

[Kim, W., Pitt, M. A., & Myung, I. J. (2013). How do PDP models learn quasiregularity? *Psychological Review, 120*(4), 903-916](http://psycnet.apa.org/record/2013-31538-001)

![]({{ site.url }}{{ site.baseurl }}/images/3D_HiddenAll_v3_cropped.svg){: style="max-width: 470px; float: right; border: 10px"}

addressed the long standing question: How can a PDP network, apparently a single system, learn conflicting kinds of input-output relationships (e.g., read regular and exception pronunciations of English spellings) while at the same time generalize well (e.g., learn and apply regularity to read nonwords that the network has not encountered during training)? The study unveiled an elusive structure that multi-layer PDP models forms into their internal representation in order to learn quasiregularity. These findings can assist PDP modelers in understanding the causes and consequences of modeling details, as well as in further investigating their suitability as scientific models. Part of the findings have been tested in an experimental study ([Armstrong, Dumay, Kim, & Pitt, 2017](http://psycnet.apa.org/record/2017-03298-005)).

Often times, computational models in psychology are based on simulations with no explicit statistical structure. These models are not amenable for existing statistical estimation and evaluation methods. We developed a model analysis tool to assist model development in this situation ([Kim, Navarro, Pitt, & Myung, 2004](http://papers.nips.cc/paper/2374-an-mcmc-based-method-of-comparing-connectionist-models-in-cognitive-science.pdf); [Pitt, Kim, Navarro, & Myung, 2006](http://psycnet.apa.org/record/2006-01885-003)). These studies demonstrated that an algorithm, dubbed parameter space partitioning (PSP), searches a model’s predicted data space, showing what kind of data patterns the model can predict under all parameter settings without being affected by the idiosyncrasy of particular parameterization.

### Application of Bayesian Methods

[Bayesian methods for statistical inference](https://en.wikipedia.org/wiki/Bayesian_inference), which have been rising in popularity, can be useful tools for overcoming ubiquitous modeling assumptions such as normality and linearity. It is often easier within the Bayesian framework to specify and estimate models for data with arbitrarily complex structure.

As for the issue of choosing between Bayesian and classical (frequentist) approaches to data analysis, we would call ourselves pragmatic Bayesians. Only when the given problem is not straightforward to handle with conventional methods, we can have convincing arguments for an alternative approach. One such example, which we believe should be better acknowledged among researchers, is Bayesian hypothesis testing that is used to test null and alternative hypotheses in a non-nested relationship. For example, the method can test a null hypothesis that the population mean is less than a certain value against an alternative hypothesis that it is greater than another, higher value considered to represent a clinically meaningful effect. Dr. Kim has provided theoretical and technical expertise in the application of Bayesian hypothesis testing ([Lodewyckx, Kim, Lee, & Wagenmakers, 2011](http://www.sciencedirect.com/science/article/pii/S0022249611000423); [Pitt, Kim, & Myung, 2003](https://link.springer.com/article/10.3758/BF03196467); [Shiffrin, Lee, Kim, & Wagenmakers, 2008](http://onlinelibrary.wiley.com/doi/10.1080/03640210802414826/full); [Steegen, Kim, Pestman, Tuerlinckx, & Vanpaemel, 2017](https://www.sciencedirect.com/science/article/pii/S0022249617300275)).

Modeling and estimating hierarchical structure is another advantage of the Bayesian approach due to its simulation-based inference mechanism, which is easier to build and run whenever different, candidate assumptions need to be tested. Dr. Kim has worked with researchers in cognitive and clinical areas, helping to build and estimate hierarchical Bayes models ([Ahn, Krawitz, Kim, Busemeyer, & Brown, 2011](http://psycnet.apa.org/record/2011-09442-003); [Fridberg et al., 2010](http://www.sciencedirect.com/science/article/pii/S0022249609001205)).
