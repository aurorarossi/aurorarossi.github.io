+++
title = "Research"
+++

## Research projects

My research lies at the intersection of graph theory, graph machine learning and network neuroscience. I develop methods and open-source tools for (temporal) networks and apply them to brain data and to other real-world systems.

~~~
<div class="project-group">
<h3>Network neuroscience</h3>

<div class="project">
  <div class="project-img"><img src="/assets/research/hyperbolic-graph.webp" alt="A random hyperbolic graph drawn in the Poincaré disk" loading="lazy"></div>
  <div>
    <h4>Temporal networks for brain dynamics</h4>
    <p>I model fMRI recordings as temporal networks, where nodes are brain regions and edges capture correlations that change over time. I study which temporal properties, such as temporal small-worldness, distinguish real brain dynamics from randomness, and proposed temporal hyperbolic random graphs as null models. The resulting temporal brain networks are openly released as datasets.</p>
    <div class="badges">
      <a href="https://hal.science/hal-04389639/document">PDF</a>
      <a href="https://docs.google.com/presentation/d/1w4Edv84NaszzNkWQM6jBevVwoXjajnX1_AzeU-7ypVQ/edit?usp=sharing">Slides</a>
      <a href="https://entrepot.recherche.data.gouv.fr/dataset.xhtml?persistentId=doi%3A10.57745%2FPR8VUV">Dataset</a>
      <a href="https://inria.hal.science/tel-05389508">PhD thesis</a>
      <a href="https://www.youtube.com/watch?v=-WM74PqyFeU">Video</a>
    </div>
  </div>
</div>

<div class="project">
  <div class="project-img"><img src="/assets/research/brain-subnetworks.webp" alt="The seven Yeo functional subnetworks of the brain" loading="lazy"></div>
  <div>
    <h4>Explainable machine learning on brain subnetworks</h4>
    <p>What happens in the brain when we listen to or watch a story? I train a neural network to classify narratives from dynamic functional connectivity, and use Shapley values to quantify how much each of the Yeo 7 subnetworks contributes to the model's decisions.</p>
    <div class="badges">
      <a href="https://hal.science/hal-04596845/document">PDF</a>
      <a href="https://docs.google.com/presentation/d/15zgW8RP0wn3PvKst521mTZsAQNjIP0dg3T0X2PpD3wo/edit?usp=sharing">Slides</a>
      <a href="https://www.youtube.com/watch?v=ge1bclA-BQQ">Video (FR)</a>
    </div>
  </div>
</div>
</div>

<div class="project-group">
<h3>Graph machine learning</h3>

<div class="project">
  <div class="project-img"><img src="/assets/research/brava-gnn.webp" alt="BRAVA-GNN architecture: degree-mass embeddings followed by message-passing layers on A and its transpose" loading="lazy"></div>
  <div>
    <h4>Graph neural networks for centrality ranking</h4>
    <p>Exact betweenness centrality is prohibitive on large networks. BRAVA-GNN is a lightweight GNN that ranks nodes by betweenness using multi-hop degree masses as size-invariant features. It works on both directed and undirected graphs and uses 56× fewer parameters than the lightest competing GNN.</p>
    <div class="badges">
      <a href="https://inria.hal.science/hal-05502800/document">PDF</a>
      <a href="https://docs.google.com/presentation/d/1i8_K0SxjpG-s73PAm1oMhlVoQG9JaQ2iDx9W_VBgreQ/edit?usp=sharing">Slides</a>
      <a href="https://github.com/justindachille/BRAVA-GNN">Code</a>
    </div>
  </div>
</div>
</div>

<div class="project-group">
<h3>Open-source software</h3>

<div class="project">
  <div class="project-img"><img src="/assets/research/graphneuralnetworks-logo.svg" alt="GraphNeuralNetworks.jl logo" loading="lazy"></div>
  <div>
    <h4>Deep learning on graphs in Julia</h4>
    <p>I co-develop <a href="https://github.com/JuliaGraphs/GraphNeuralNetworks.jl">GraphNeuralNetworks.jl</a>, a Julia framework for graph neural networks with GPU support and both Flux and Lux backends. During Google Summer of Code 2023 and Julia Summer of Code 2024 I added support for temporal graphs and temporal GNN layers.</p>
    <div class="badges">
      <a href="https://jmlr.org/papers/volume26/24-2130/24-2130.pdf">PDF</a>
      <a href="https://docs.google.com/presentation/d/1ocgJj5jGwaa2fCtpL3GwlCl2zlS8MuTkS_P68gwuoAQ/edit?usp=sharing">Slides</a>
      <a href="https://github.com/JuliaGraphs/GraphNeuralNetworks.jl">Code</a>
      <a href="https://youtu.be/9JWnu5ecET8?t=12629">Video</a>
    </div>
  </div>
</div>

<div class="project">
  <div class="project-img"><img src="/assets/research/temporalgraphs-logo.svg" alt="TemporalGraphs.jl logo: snapshots of a graph along a time axis" loading="lazy"></div>
  <div>
    <h4>Temporal graph analysis in Julia</h4>
    <p><a href="https://github.com/aurorarossi/TemporalGraphs.jl">TemporalGraphs.jl</a> is a pure-Julia library for temporal graphs: temporal distances and optimal paths, temporal centralities (closeness, betweenness, Katz, PageRank), connectivity, flows, spanners, motifs and randomized models. It downloads public temporal networks (SNAP, SocioPatterns) and converts temporal graphs to GNNGraphs for GraphNeuralNetworks.jl.</p>
    <div class="badges">
      <a href="https://github.com/aurorarossi/TemporalGraphs.jl">Code</a>
      <a href="https://aurorarossi.github.io/TemporalGraphs.jl/dev/">Docs</a>
    </div>
  </div>
</div>

<div class="project">
  <div class="project-img"><img class="logo-small" src="/assets/research/juliagraphs-logo.webp" alt="JuliaGraphs logo" loading="lazy"></div>
  <div>
    <h4>Graph optimization in Julia</h4>
    <p>I am the current maintainer of <a href="https://github.com/JuliaGraphs/GraphsOptim.jl">GraphsOptim.jl</a>, a JuliaGraphs package for graph problems solved with mathematical programming: min-cost flow, assignment, graph matching and graph edit distance, maximum clique, independent set, vertex cover, fractional coloring and shortest paths.</p>
    <div class="badges">
      <a href="https://www.dropbox.com/scl/fi/5bmty02spntuo81kd4tus/GraphMatching.pdf?rlkey=w2z65wrz42sm55iqzkib30v9j&amp;dl=0">Slides</a>
      <a href="https://github.com/JuliaGraphs/GraphsOptim.jl">Code</a>
      <a href="https://juliagraphs.org/GraphsOptim.jl/dev">Docs</a>
      <a href="https://www.youtube.com/watch?v=a9Jw0LnHuGI">Video</a>
    </div>
  </div>
</div>
</div>

<div class="project-group">
<h3>AI for mathematics</h3>

<div class="project">
  <div class="project-img"><img src="/assets/research/graph-theory-ai.webp" alt="Graph Theory AI logo" loading="lazy"></div>
  <div>
    <h4>AI for open problems in graph theory</h4>
    <p>In the <a href="https://github.com/graph-theory-AI">Graph Theory AI</a> project we explore how large language models can track and support progress on open problems in graph theory: a status-annotated catalogue of graph conjectures, LLM proof attempts checked by an adversarial reviewer model, machine-checkable formalizations in Rocq, and Mathpocalypse, where an open-weight LLM re-checks proofs in published papers.</p>
    <div class="badges">
      <a href="https://graph-theory-ai.github.io/graph-conjectures/">Website</a>
      <a href="https://github.com/graph-theory-AI">Code</a>
      <a href="https://github.com/graph-theory-AI/Graph-Theory-LLM-Proofs">LLM proofs</a>
    </div>
  </div>
</div>
</div>
~~~

## Publications

### Journal papers

@@pub
[*"Characterizing Dynamic Functional Connectivity Subnetwork Contributions in Narrative Classification with Shapley Values"*](https://direct.mit.edu/netn/article/doi/10.1162/netn.a.25/131329/Characterizing-dynamic-functional-connectivity) \
**Aurora Rossi**, Yanis Aeschlimann, [Emanuele Natale](https://natema.github.io/ema-webpage/), [Samuel Deslauriers-Gauthier](https://scholar.google.com/citations?user=p3fbfPwAAAAJ&hl=en), [Peter Ford Dominey](https://scholar.google.com/citations?user=plk1bUYAAAAJ&hl=en) \
*[Network Neuroscience](https://direct.mit.edu/netn), 2025*
@@pub-links
[PDF](https://hal.science/hal-04596845/document) [Slides](https://docs.google.com/presentation/d/15zgW8RP0wn3PvKst521mTZsAQNjIP0dg3T0X2PpD3wo/edit?usp=sharing) [Video (FR)](https://www.youtube.com/watch?v=ge1bclA-BQQ)
@@
@@

@@pub
[*"GraphNeuralNetworks.jl: Deep Learning on Graphs with Julia"*](http://jmlr.org/papers/v26/24-2130.html) \
[Carlo Lucibello](https://carlolucibello.github.io/), **Aurora Rossi** \
*[Journal of Machine Learning Research](https://www.jmlr.org/), 2025*
@@pub-links
[PDF](https://jmlr.org/papers/volume26/24-2130/24-2130.pdf) [Slides](https://docs.google.com/presentation/d/1ocgJj5jGwaa2fCtpL3GwlCl2zlS8MuTkS_P68gwuoAQ/edit?usp=sharing) [Code](https://github.com/JuliaGraphs/GraphNeuralNetworks.jl) [Video](https://youtu.be/9JWnu5ecET8?t=12629)
@@
@@

@@pub
[*"A sensitivity analysis of the Earth for all model: Getting the giant leap scenario with fewer policies"*](https://onlinelibrary.wiley.com/doi/10.1111/jiec.13582) \
[Pierluigi Crescenzi](https://www.pilucrescenzi.it/), Giorgio Gambosi, Lucia Nasti, [Emanuele Natale](https://natema.github.io/ema-webpage/), **Aurora Rossi** \
*[Journal of Industrial Ecology](https://onlinelibrary.wiley.com/journal/15309290), 2024*
@@pub-links
[PDF](https://hal.science/hal-04780536/document)
@@
@@

@@pub
[*"WorldDynamics.jl: A Julia Package for Developing and Simulating Integrated Assessment Models"*](https://joss.theoj.org/papers/10.21105/joss.05772) \
[Pierluigi Crescenzi](https://www.pilucrescenzi.it/), [Emanuele Natale](https://natema.github.io/ema-webpage/), **Aurora Rossi**, [Paulo Bruno Serafim](https://paulobruno.github.io/) \
*[Journal of Open Source Software](https://joss.theoj.org/), 2024*
@@pub-links
[PDF](https://hal.science/hal-04117509/document) [Slides](https://www.dropbox.com/s/k2diduuny307ivp/worlddynamics_juliahalf-day.pdf?dl=0) [Code](https://github.com/worlddynamics/WorldDynamics.jl)
@@
@@

@@pub
[*"On null models for temporal small-worldness in brain dynamics"*](https://direct.mit.edu/netn/article/doi/10.1162/netn_a_00357/119098/On-null-models-for-temporal-small-worldness-in) \
**Aurora Rossi**, [Samuel Deslauriers-Gauthier](https://scholar.google.com/citations?user=p3fbfPwAAAAJ&hl=en), [Emanuele Natale](https://natema.github.io/ema-webpage/) \
*[Network Neuroscience](https://direct.mit.edu/netn), 2024*
@@pub-links
[PDF](https://hal.science/hal-04389639/document) [Slides](https://docs.google.com/presentation/d/1w4Edv84NaszzNkWQM6jBevVwoXjajnX1_AzeU-7ypVQ/edit?usp=sharing) [Dataset](https://entrepot.recherche.data.gouv.fr/dataset.xhtml?persistentId=doi%3A10.57745%2FPR8VUV)
@@
@@

### Conference papers

@@pub
[*"Degree-Mass Message Passing for Betweenness Ranking in Directed and Undirected Networks"*](https://inria.hal.science/hal-05502800) \
Justin Dachille, **Aurora Rossi**, Sunil Kumar Maurya, Frederik Mallmann-Trenn, Xin Liu, Frédéric Giroire, Tsuyoshi Murata, Emanuele Natale \
*[The 35th ACM International Conference on Information and Knowledge Management (CIKM 2026)](https://cikm2026.diag.uniroma1.it), November 7th - 11th 2026, Rome, Italy*
@@pub-links
[PDF](https://inria.hal.science/hal-05502800/document) [Slides](https://docs.google.com/presentation/d/1i8_K0SxjpG-s73PAm1oMhlVoQG9JaQ2iDx9W_VBgreQ/edit?usp=sharing) [Code](https://github.com/justindachille/BRAVA-GNN)
@@
@@

@@pub
[*"La vie risquée mais enrichissante d'un doctorant interdisciplinaire: accrochez-vous, une seule publication suffit!"*](https://hal.science/hal-05598152) \
Sayf Halmi, **Aurora Rossi**, Frédéric Giroire, Nicolas Nisse, Michele Pezzoni \
*[ALGOTEL 2026](https://algotel-cores26.sciencesconf.org), June 2026, Mandelieu-la-Napoule, France*
@@pub-links
[PDF](https://hal.science/hal-05598152/document)
@@
@@

@@pub
[*"Une implémentation GPU de la méthode de recherche approximative FlyHash"*](https://hal.science/hal-04328529v1/document) \
[Arthur da Cunha](https://arthurwalraven.github.io/), [Emanuele Natale](https://natema.github.io/ema-webpage/), Damien Rivet, **Aurora Rossi** \
*[Conference on Artificial Intelligence for Defense](https://caid-conference.eu/), DGA Maîtrise de l'Information, November 22nd and 23rd 2023, Rennes, France*
@@pub-links
[PDF](https://hal.science/hal-04328529v1/document)
@@
@@

@@pub
[*"Un framework open-source écrit en Julia pour la modélisation d’évaluation globale intégrée"*](https://roadef2023.sciencesconf.org/436893/document) \
[Pierluigi Crescenzi](https://www.pilucrescenzi.it/), [Hicham Lesfari](https://hlesfari.github.io/), [Emanuele Natale](https://natema.github.io/ema-webpage/), **Aurora Rossi**, [Paulo Serafim](https://paulobruno.github.io/) \
*[ROADEF 2023](https://roadef2023.sciencesconf.org/), February 20th - 23rd 2023, Rennes, France*
@@pub-links
[PDF](https://hal.science/hal-04008491/document) [Slides](https://www.dropbox.com/s/k2diduuny307ivp/worlddynamics_juliahalf-day.pdf?dl=0) [Code](https://github.com/worlddynamics/WorldDynamics.jl)
@@
@@

### Extended abstracts

@@pub
[*"Understanding the Importance of Brain Subnetworks with Shapley Values During Narrative Processing"*](https://hal.science/hal-04723178v1/document) \
**Aurora Rossi**, Yanis Aeschlimann, [Emanuele Natale](https://natema.github.io/ema-webpage/), [Samuel Deslauriers-Gauthier](https://scholar.google.com/citations?user=p3fbfPwAAAAJ&hl=en), [Peter Ford Dominey](https://scholar.google.com/citations?user=plk1bUYAAAAJ&hl=en) \
*[Complex Networks Conference](https://complexnetworks.org/), December 10th and 12th 2024, Istanbul, Turkey*
@@pub-links
[PDF](https://hal.science/hal-04723178v1/document) [Slides](https://docs.google.com/presentation/d/1xD6qvqDcO89q0gfr8MY5vP6ep8gwQ2-cP4CV3K1pPno/edit?usp=sharing)
@@
@@

@@pub
[*"Temporal Hyperbolic Graphs as Null Models for Brain Dynamics"*](https://hal.science/hal-04343066v1/document) \
**Aurora Rossi**, [Samuel Deslauriers-Gauthier](https://scholar.google.com/citations?user=p3fbfPwAAAAJ&hl=en), [Emanuele Natale](https://natema.github.io/ema-webpage/) \
*[Complex Networks Conference](https://complexnetworks.org/), November 28th and 30th 2023, Menton, France*
@@pub-links
[PDF](https://hal.science/hal-04343066v1/document) [Slides](https://www.dropbox.com/scl/fi/c7zj4h0hsx5mdld7g2yeo/NullModelBrainDynamicsCNA.pdf?rlkey=iynor4j3g8txq66ir3ctw8sql&dl=0)
@@
@@

### PhD Thesis

@@pub
[*"Computational Methods and Analysis of Temporal Networks: Applications in Neuroscience"*](https://inria.hal.science/tel-05389508) \
**Aurora Rossi** \
*[DS4H Université Côte d’Azur](https://ds4h.univ-cotedazur.eu/), 2025*. Special Award for Interdisciplinarity of the École Doctorale STIC.
@@pub-links
[PDF](https://inria.hal.science/tel-05389508/document) [Slides](https://docs.google.com/presentation/d/1pXQvo6pD9T3akMMToZfaxPCm7sivXYwVsLb5bKz4Wdk/edit?usp=sharing) [Video](https://www.youtube.com/watch?v=-WM74PqyFeU)
@@
@@

## Posters

@@pub
[*"Simulating Global Dynamics with Integrated Assessment Models"*](https://hal.science/hal-04538563v1/document) \
[Pierluigi Crescenzi](https://www.pilucrescenzi.it/), **Aurora Rossi** \
*[MOMI2024: Le Monde des Mathematiques Industrielle](https://phd-seminars-sam.inria.fr/momi-2024/), April 8th - 9th, Sophia Antipolis, France*
@@pub-links
[Poster (PDF)](https://hal.science/hal-04538563v1/document)
@@
@@

@@pub
[*"Temporal Graph Neural Networks with GraphNeuralNetworks.jl"*](https://hal.science/hal-04230797/document) \
**Aurora Rossi** \
*[Julia and Optimization Days 2023](https://julia-users-paris.github.io/workshop/en/index.html), October 3rd - 6th, CNAM Paris, France*
@@pub-links
[Poster (PDF)](https://hal.science/hal-04230797/document) [Slides](https://www.dropbox.com/scl/fi/1noza125sgmm3chb6y2gc/TGNNjl.pdf?rlkey=xhoxhxrwycrlhuw1rztskxzio&dl=0)
@@
@@

@@pub
[*"Temporal Brain Networks Dataset"*](https://hal.science/hal-04130380/document) \
**Aurora Rossi**, [Samuel Deslauriers-Gauthier](https://scholar.google.com/citations?user=p3fbfPwAAAAJ&hl=en), [Emanuele Natale](https://natema.github.io/ema-webpage/) \
*[NeuroMod](https://neuromod.univ-cotedazur.eu/) Meeting, June 28th - 29th 2023, Antibes, France*
@@pub-links
[Poster (PDF)](https://hal.science/hal-04130380/document)
@@
@@

@@pub
[*"Hyperbolic Model Captures Temporal Small Worldness of Brain Dynamics"*](https://hal.archives-ouvertes.fr/hal-03685173/document) \
**Aurora Rossi**, [Pierluigi Crescenzi](https://www.pilucrescenzi.it/), [Samuel Deslauriers-Gauthier](https://scholar.google.com/citations?user=p3fbfPwAAAAJ&hl=en), [Emanuele Natale](https://natema.github.io/ema-webpage/) \
*[NeuroMod](https://neuromod.univ-cotedazur.eu/) Meeting, June 30th -July 1st 2022, Antibes, France*
@@pub-links
[Poster (PDF)](https://hal.archives-ouvertes.fr/hal-03685173/document)
@@
@@

## Datasets

@@pub
[*"Temporal Brain Networks"*](https://entrepot.recherche.data.gouv.fr/dataset.xhtml?persistentId=doi%3A10.57745%2FPR8VUV) \
**Aurora Rossi**, [Samuel Deslauriers-Gauthier](https://scholar.google.com/citations?user=p3fbfPwAAAAJ&hl=en), [Emanuele Natale](https://natema.github.io/ema-webpage/) \
(see also [here](https://recherche.data.gouv.fr/en/dataset/temporal-brain-networks))
@@

@@pub
[*"Labeled Temporal Brain Networks"*](https://entrepot.recherche.data.gouv.fr/dataset.xhtml?persistentId=doi:10.57745/HHNT10) \
**Aurora Rossi**
@@
