---
layout: project
title: Squidpops
thumbnail: /img/squidpop-fish3.png
editbutton: true
links:
  - path: /assets/modules/squidpops/MarineGEO_Squidpop_Protocol_V1.0.0_JRMEdits.pdf
    name: Squidpop Protocol
    icon: save_alt
 -  path: /assets/modules/squidpops/SquidpopFieldsheet _JRMedits.pdf
    name: Squidpop Field Datasheet
    icon: save_alt
  - name: Squidpop Data Entry Template
    path: /assets/modules/squidpops/MarineGEO_squidpop_data_entry_template_V1.0.0_JRMedits.xlsx
    icon: save_alt
  - name: Squidpop file packet
    path: /assets/modules/squidpops/Squidpop.zip
    icon: folder
---

{% assign dataentry = page.links | where: "name", "Squidpop Data Entry Template" | first %}

{% assign protocol = page.links | where: "name", "Squidpop Protocol" | first %}

## Introduction

This protocol provides a simple, quick, standardized assay of fish predation intensity. Fish predation is important in nearly all marine ecosystems as it structures communities and is how production moves up the food web. The goal of this protocol is to establish a simple, standard method to quantify the relative intensity of feeding by generalist predators that is comparable across a wide range of sites and conditions. 

To get started, using the links above, download the necessary files (protocol, datasheet, and entry template) either seperatly or togther using "Squidpop.zip".

## Data submission

Use the <a href="{{dataentry.path}}">{{dataentry.name}}</a> to transfer data from the field data sheets into Excel and then submit data to <a href="mailto:marinegeo-data@si.edu">marinegeo-data@si.edu</a>.

## Additional Resources

### Youtube Itroduction and Instructional Videos

<!-- 16:9 aspect ratio https://stackoverflow.com/questions/15844500/shrink-a-youtube-video-to-responsive-width -->
<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/GP8c24aNykg"></iframe>
</div>

Please read the <a href="{{protocol.path}}">{{protocol.name}}</a> for full methods and instructions.

<!-- 16:9 aspect ratio https://stackoverflow.com/questions/15844500/shrink-a-youtube-video-to-responsive-width -->
<div class="embed-responsive embed-responsive-16by9">
  <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/esSByfVlMt4"></iframe>
</div>

### Selected literature

Duffy, J. E., S. L. Ziegler, J. E. Campbell, P. M. Bippus, and J. S. Lefcheck. 2015. Squidpops: A Simple Tool to Crowdsource a Global Map of Marine Predation Intensity. <a href="https://doi.org/10.1371/journal.pone.0142994">PLoS ONE 10:e0142994</a>.

Gauff, R. P. M., S. Bejarano, H. H. Madduppa, B. Subhan, E. M. A. Dugény, Y. A. Perdana, and S. C. A. Ferse. 2018. Influence of predation risk on the sheltering behaviour of the coral-dwelling damselfish, *Pomacentrus moluccensis*. <a href="https://link.springer.com/content/pdf/10.1007%2Fs10641-018-0725-3.pdf">Environmental Biology of Fishes 101:639–651</a>.

Gross, C., C. Donoghue, C. Pruitt, A. C. Trimble, and J. L. Ruesink. 2017. Taxonomic and functional assessment of mesopredator diversity across an estuarine habitat mosaic. <a href="http://doi.wiley.com/10.1002/ecs2.1792">Ecosphere 8:e01792</a>.

Gusmao, J. B., M. R. Lee, I. MacDonald, N. C. Ory, J. Sellanes, Les Watling, and M. Thiel. 2018. No reef-associated gradient in the infaunal communities of Rapa Nui (Easter Island) – Are oceanic waves more important than reef predators? <a href="https://doi.org/10.1016/j.ecss.2018.06.019">Estuarine Coastal and Shelf Science 210:123–131</a>.

Lefcheck, J. S., S. J. Brandl, P. L. Reynolds, A. R. Smyth, and S. T. Meyer. 2016. Extending Rapid Ecosystem Function Assessments to Marine Ecosystems: A Reply to Meyer. <a href="http://dx.doi.org/10.1016/j.tree.2016.02.002">Trends in ecology & evolution 31:251–253</a>).

Rodemann, J. R., and S. J. Brandl. 2017. Consumption pressure in coastal marine environments decreases with latitude and in artificial vs. natural habitats. Marine ecology progress series. <a href="http://www.int-res.com/articles/meps2017/574/m574p167.pdf">Oldendorf 574:167–179</a>.
