---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
redirect_from: 
  - /research.html
---

{% include base_path %}

Here are some brief outlines of some of my current and ongoing research projects and interests.


**Spatial planning for global terrestrial and marine biodiversity conservation**

The [Half-Earth Project](https://www.half-earthproject.org/) posits that we must set aside half of the earth for the successful preservation of biodiversity. I am using a spatial conservation planning framework to address the question most succinctly stated: *“Which half?”* Working closely with the [E.O. Wilson Biodiversity Foundation](https://eowilsonfoundation.org/) and [Map of Life](https://mol.org/), I combine global patterns of the distributions of 30,000+ terrestrial vertebrates with human land use layers, and use a linear optimization approach to design global conservation networks that protect a sufficient amount of habitat for every species. I am also doing a similar study for the marine environment, focusing on marine mammals and commonly harvested fish species.

Much of this research is designed to support the [Convention on Biological Diversity](https://www.cbd.int/) and its associated [Biodiversity Targets](https://www.cbd.int/sp/targets/), and to help inform international negotiations of a post-2020 [Global Biodiversity Framework](https://www.cbd.int/conferences/post2020), reflecting the best available science and most complete and up-to-date portrait of the planet's biodiversity. A key feature of the results is that the burden of conservation is highly geographically variable, necessitating individualized conservation targets and goals at the national level as well as the species level.

<figure>
  <img src="/images/terrestrial-prioritization4.png" alt="Conservation area network.">
  <figcaption>Figure 4. Conservation area network composition across ecoregions, biomes, and countries. (A) The percentage of each ecoregion contained in the network by biome category. Point colors indicate the median amount of HM in the network within each ecoregion. Percentages in parentheses indicate the total amount of global land area within each biome. (B) The percentage of each biome contained in the network by degree of HM and the amount currently protected. (C) Differences in conservation burden between countries, calculated as a ratio of a weighted sum of each country’s area contained in the network and its gross national income adjusted for purchasing power parity (GNI PPP). The sum is weighted by HM category, with higher degrees of HM weighted more heavily. Burden is normalized by the global conservation burden (GCB), representing the weighted sum of the entire network divided by the sum of GNI PPP, and equal to 0.652. Countries in red have a higher burden than GCB, and countries in blue have a lower burden than GCB. Pie charts illustrate the proportion of each country contained in the network by degree of HM, the amount currently protected (PA), and the amount not in the network (NA). The radius of each pie chart is proportional to the total area of the country it represents. Countries in grey did not have recent estimates of GNI PPP available.</figcaption>
</figure>

**CENFA package for R: tools for climate- and environmental- niche factor analysis of spatial data**

I authored and maintain an R package that provides methods for visualization of spatial variability of species sensitivity, exposure, and vulnerability to climate change. This package complements [previous work of mine](https://rinnan.github.io/publication/2019-09-01-climate-niche-factor-analysis), and updates the ENFA method for use with large datasets and modern data formats. It also includes some functions for speeding up certain raster functions considerably via parallelization.

Available at [https://cran.r-project.org/package=CENFA](https://cran.r-project.org/package=CENFA) and [https://github.com/rinnan/CENFA](https://github.com/rinnan/CENFA).

**Incorporating biological and ecological realism into species distribution modeling**

One common criticism of species distribution models (SDMs) is their lack of realism: describing the relationship between a species and its environment using only statistical correlations ignores all of the ecological and physiological processes that constrain the distributions of populations. By not accounting for dispersal ability, for example, SDMs fail to provide any insight into a species' ability to successfully colonize new areas identified as potentially suitable future habitat. As such, SDMs can greatly underestimate species vulnerability to climate change. 

Integro-difference equations (IDEs), by contrast, offer a modeling approach that provides a mechanistic understanding of how species traits shape long-term population dynamics. IDEs are quite flexible and can accommodate a wide variety of models, including stage-structure in populations, resource competition by multiple species, changes in habitat quality, density dependence, and environmental and demographic stochasticity. Despite their flexibility, integro-difference models are more theoretical in nature, and typically use an oversimplified notion of species habitat, often reducing it down to a single spatial dimension. While this is useful for understanding population dynamics and processes, it provides little insight into how these processes translate to a physical landscape.

I am developing and exploring a novel modeling framework that bridges the gap between these two approaches by combining the strengths of SDM and IDE techniques. This framework provides key insight into how traits such as growth rate and dispersal ability affect long-term population stability in a changing environment.

<figure>
  <img src="/images/idm.jpg" alt="Model comparison." style="width:80%;height:80%;">
  <figcaption>Differences in model predictions for <i>Ochotona princeps<i>. (a) Historical predictions of a traditional SDM. No discernment is made between occupied and suitable habitat. (b) Future predictions of the SDM in (a). The suitable habitat has shifted due to climate change, with no difference between suitable and occupied habitat. (c) Future predictions of a two-dimensional IDE with no specification of habitat quality. The population has grown and dispersed into new habitat, with an invasion speed determined by the growth rate and dispersal ability. (d) Future predictions of the IDM. The suitable habitat has shifted due to climate change, but the population is limited by dispersal ability and growth rate. Some population is lost due to habitat becoming unsuitable. The SDM in (a) serves as the habitat quality function of the IDM.</figcaption>
</figure>

