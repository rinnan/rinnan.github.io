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

Available at <https://cran.r-project.org/package=CENFA> and <https://github.com/rinnan/CENFA>.