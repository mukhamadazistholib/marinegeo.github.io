---
layout: project
title: Squidpops
thumbnail: /img/squidpop-fish3.png
editbutton: true
links:
  - name: Squidpop Protocol
    path: /assets/modules/squidpops/MarineGEO_Squidpop_Protocol_V1.0.0_JRMEdits.pdf
    icon: save_alt
 -  path: marinegeo.github.io/assets/modules/squidpops/SquidpopFieldsheet _JRMedits.pdf
    name: Squidpop Field Datasheet
    icon: save_alt
  - name: Squidpop Data Entry Template
    path: /assets/modules/squidpops/MarineGEO_squidpop_data_entry_template_V1.0.0_JRMedits.xlsx
    icon: save_alt
---

{% assign dataentry = page.links | where: "name", "Squidpop Data Entry Template" | first %}

{% assign protocol = page.links | where: "name", "Squidpop Protocol" | first %}


## Introduction

Fish predation is an important process structuring communities and a conduit of production up the food web in nearly all marine ecosystems. This protocol provides a simple, quick, standardized assay of fish predation intensity. The goal is to quantify the relative intensity of feeding by generalist predators using a standard bait and method that is simple and comparable across a wide range of sites and conditions. When coupled with camera deployments, it can also be part of a Baited Remote Underwater Video (BRUV) sampling of the fish community. We use dried squid as bait because most marine predators are generalists who readily eat it, it is widely available (e.g., in Asian grocery stores), and the dried bait can be shipped and stored without refrigeration.

The assay measures the rate of fish predation as loss of standard bait deployed for 24 hours in the field. Each bait is a 1.3-cm diameter disk of dried squid mantle tethered to a stake, which is either inserted in the sediment or secured to existing structure. Each squid bait is scored as present or absent after 1 and 24 hours, and predation rate is estimated as the proportion of replicate baits consumed at each time. Tests in several habitats have confirmed the assay’s utility for measuring variation in predation intensity among habitats, among seasons, and along environmental gradients (see Selected Literature below).

<!-- 16:9 aspect ratio https://stackoverflow.com/questions/15844500/shrink-a-youtube-video-to-responsive-width -->
<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/esSByfVlMt4"></iframe>
</div>


## Measured parameters

  - feeding intensity by generalist predators

## Requirements

**Personnel:** 2

**Time:** Preparation: 1 person x 2 hours. Field: 2 people x 2 days (roughly two half days, depending on travel time and field conditions). Data curation: 1 person x 1-2 hours.

**Frequency:** Variable (at least annually)

**Materials:** Dried squid mantle, auger hole punch, green fiberglass garden stakes, fishing line

## Methods

See the instructional video for details:

<!-- 16:9 aspect ratio https://stackoverflow.com/questions/15844500/shrink-a-youtube-video-to-responsive-width -->
<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/GP8c24aNykg"></iframe>
</div>

Please read the <a href="{{protocol.path}}">{{protocol.name}}</a> for full methods and instructions.

## Data curation     

Use the <a href="{{dataentry.path}}">{{dataentry.name}}</a> to transfer data from the field data sheets into Excel and then submit data to <a href="mailto:marinegeo-data@si.edu">marinegeo-data@si.edu</a>.

## Selected literature

Duffy, J. E., S. L. Ziegler, J. E. Campbell, P. M. Bippus, and J. S. Lefcheck. 2015. Squidpops: A Simple Tool to Crowdsource a Global Map of Marine Predation Intensity. <a href="https://doi.org/10.1371/journal.pone.0142994">PLoS ONE 10:e0142994</a>.

Gauff, R. P. M., S. Bejarano, H. H. Madduppa, B. Subhan, E. M. A. Dugény, Y. A. Perdana, and S. C. A. Ferse. 2018. Influence of predation risk on the sheltering behaviour of the coral-dwelling damselfish, *Pomacentrus moluccensis*. <a href="https://link.springer.com/content/pdf/10.1007%2Fs10641-018-0725-3.pdf">Environmental Biology of Fishes 101:639–651</a>.

Gross, C., C. Donoghue, C. Pruitt, A. C. Trimble, and J. L. Ruesink. 2017. Taxonomic and functional assessment of mesopredator diversity across an estuarine habitat mosaic. <a href="http://doi.wiley.com/10.1002/ecs2.1792">Ecosphere 8:e01792</a>.

Gusmao, J. B., M. R. Lee, I. MacDonald, N. C. Ory, J. Sellanes, Les Watling, and M. Thiel. 2018. No reef-associated gradient in the infaunal communities of Rapa Nui (Easter Island) – Are oceanic waves more important than reef predators? <a href="https://doi.org/10.1016/j.ecss.2018.06.019">Estuarine Coastal and Shelf Science 210:123–131</a>.

Lefcheck, J. S., S. J. Brandl, P. L. Reynolds, A. R. Smyth, and S. T. Meyer. 2016. Extending Rapid Ecosystem Function Assessments to Marine Ecosystems: A Reply to Meyer. <a href="http://dx.doi.org/10.1016/j.tree.2016.02.002">Trends in ecology & evolution 31:251–253</a>).

Rodemann, J. R., and S. J. Brandl. 2017. Consumption pressure in coastal marine environments decreases with latitude and in artificial vs. natural habitats. Marine ecology progress series. <a href="http://www.int-res.com/articles/meps2017/574/m574p167.pdf">Oldendorf 574:167–179</a>.
