---
layout: post_interview
title: Interview with the developer behind GloBI - Jorrit Poelen
date: 2019-03-07
author: Ciera Martinez (CM)
avatar: avatars/cieraavatar2.png
interview: Jorrit Poelen (JP)
avatar2: avatars/jorrit.png
description: null
output: 
  html_document: 
    keep_md: yes
img: 2019-03-08-interview_jorrit/interactions2.jpg
legend: biodiversitylibrary.org/page/50095133
tags: Interviews
---

This is the first in a series where I interview people involved in the the biodiversity and natural history data community. I met Jorrit Poelen last year at the [Digital Data in Biodiversity Conference](http://curiositydata.org/Meeting-the-Modern-Naturalists_at_the_digital_data_conference/) and was really struck by his ideas on data persistance and software design. His background in industry as a software developer gives him a clear vision on how biodiveristy data can be used and maintained.  Currently he is a freelance software developer and lead maintainer of the [Global Biotic Interactions](https://www.globalbioticinteractions.org/) GloBI platform. At GloBI researchers can explore data describing the relationships between organisms and their enviroment. GloBI is unique in that it builds biodiversity data infrastructures for analyses and isn't just data aggregation like many other biodiversity data portals. See tutorials on how to use the site in previous posts [here](http://curiositydata.org/part1_globi_access/) and [here](http://curiositydata.org/part2_globi_exploration/).

Recently we found the time to discuss his work with GloBi and how he came to be involved in the natural history data community. 

**Ciera Martinez (CM)**: <intq>Can you briefly tell me how you became involved with the GloBI database? </intq>

**Jorrit Poelen (JP)**: In 2011, I was asked to join the Ecological Integration Symposium at Texas A&M College Station to present "Evidence of Use", a video art installation. In a short introduction talk about the artwork for the conference audience, I invited the audience to integrate their datasets into the video art installation. Dr. James D. Simons, a marine biologist, came up to me after my talk and shared his data on predator-prey relationships of fish in the Gulf of Mexico. I took his dataset and integrated it into the video installation in about 10 minutes. This initial and pragmatic data exchange led to a continued collaboration and an Encyclopedia of Life Rubenstein Fellowship award in 2013 along with Jim Simons and Chris Mungall. This fellowship provided the initial focus and time to develop GloBI as a way to more easily combine existing species interaction datasets and link them to other biodiversity data projects.

**CM**: <intq>By now you must have seen a lot of different data sets, is there a data set(s) that stands out as your favorite?  Why?</intq>

**JP**: GloBI currently indexes over 100 existing species interactions datasets. Each dataset has a unique story and took their authors energy and persistence to compile. Because each dataset is unique in its own way, I find it hard to pick favorites. However, my favorite datasets are those that are published openly in an easy to understand data format suitable for re-use and re-archiving. One particular dataset, the Africa Tree Database, contains plant-animal interactions from Africa ([Seltzer et al. 2015](https://dx.doi.org/10.6084/m9.figshare.1526128)) and is still available today because Carrie Seltzer and collaborators published, following my advice, a web archive of the database on FigShare. Without her data publication, the valuable species interaction dataset would have been lost today, because the original website at http://africatreedatabase.org is no longer active.  

**CM**: <intq>Along those same lines, is there a favorite case in which the GloBI data was used?</intq>

**JP**: GloBI's method paper has been used and cited in over 40 peer-reviewed articles. To me, this indicates that GloBI is used as an example of how to discover and re-use existing species interaction datasets. Also, I get excited to see how GloBI data products are used to create a [food web map of the world](http://127.0.0.1:4000/assets/img/2019-03-08-interview_jorrit/interactions2.jpg), an [interactive interaction explorer](http://danielabar.github.io/globi-proto) or an [educational cluster visualization](see https://github.com/terschure/reimagined-lamp). In addition, playful data explorations like [Hungry Caterpillar](http://timotheepoisot.fr/2015/05/10/hungry-caterpillars/) show how GloBI can be used for quick data exploration and analysis.

**CM**: <intq>One of the unique aspects of GloBI is the automation of data retrieval. Can you briefly explain how and why you came up with strategy?</intq>

**JP**: I noticed that datasets were already being published in data journals and platforms like FigShare, Zenodo, GitHub, iNaturalist and Dryad. I also found that datasets are often updated to include data corrections and new data. To make best use of these established platforms and ways of working, I developed Elton (see [https://doi.org/10.5281/zenodo.998263](https://doi.org/10.5281/zenodo.998263) and [https://github.com/globalbioticinteractions/](https://github.com/globalbioticinteractions/)), a computer program, to automatically keep track of datasets by periodically discovering, and retrieving, datasets across various publication platforms. Elton allows GloBI to automatically make data updates available in a timely fashion while leaving the original data contributors in control of their datasets without having to change established data sharing methods.  

**CM**: <intq>I found a section on the GloBI website entitled <a href="https://www.globalbioticinteractions.org/2017/01/24/lifestages-of-species-interaction-datasets/"> Lifestages of Species Interaction Datasets</a>, and it starts with the sentence "Just like organisms, datasets get born, grow up, reproduce, and die." What do you think the biggest challenge is for a biodiversity dataset to survive?</intq>

**JP**: I think the biggest challenge for biodiversity datasets to survive is to develop methods that demonstrate that openly publishing, re-using and combining biodiversity datasets is beneficial to individual researchers and allow to answer bigger questions with smaller budgets. Why would an individual researcher spend their precious time to publish their valuable datasets if this does not work towards achieving their research goals? Without a clear answer to this question, datasets are less likely to survive because there's no reason to keep them around. One of the emerging benefits from openly publishing datasets is that researchers can use the published datasets as a backup in case their original data is lost due to a harddisk crash, theft or some other data disaster. 
 
**CM**: <intq>A large part of GloBI is talking to individuals about their data and convincing them that it should be incorporated into GloBI. How do convince someone the importance of their data being part of GloBI? What are the main benefits of someone investing in making their data available for the GloBI database?</intq>

**JP**: Openly sharing datasets help others to re-use your work, make it more visible and provide feedback on it. GloBI facilitates re-use by discovering and combining openly published species interaction datasets. Also, GloBI provides automated quality metrics for each dataset to help correct unintended mistakes and inconsistencies. Another advantage is that projects like the Encyclopedia of Life, World Register for Marine Species, NCBI Taxonomy, iNaturalist, FishBase and SeaLifeBase link to datasets indexed by GloBI. This means that by sharing data with GloBI, your data gets published across many different platforms and increases the visibility of your data.  

**CM**: <intq>What are the biggest push backs when talking to people?</intq>

**JP**: Some people have spent years of their life to compile a dataset. They feel that they'd lose their edge in today's competitive academic environment by giving their dataset away for free. Others are hesitant to publish because they fear that their data would be misinterpreted. Another reason for postponing openly publishing is that getting a dataset ready for publication is often an afterthought and not factored into a research plan. So rather than considering a data publication as an essential part of doing research, it is often skipped because it is treated as an optional extra-curricular activity. 

**CM**: <intq>When Yikang Li was presenting me her work, I was surprised to find 36 unique interaction types, but when I looked even further into the documentation, I found a <a href="https://github.com/globalbioticinteractions/inaturalist/blob/master/interaction_types.csv"> list of over 151 different types</a> of interaction types found in all the datasets.  What was the process of linking how people describe their data to fitting their data into GloBI? Was there already established Interaction Ontology established?</intq>

**JP**: Existing species interaction datasets are mapped and transformed into GloBI using dataset importers. These importers are computer programs that take an existing dataset in their original format, extract the relevant terms and map these terms into naming schemes such as the [OBO Relations Ontology](https://doi.org/10.5281/zenodo.593101). The OBO Relations Ontology (RO) is an independently curated collection of relationship terms. RO includes definitions of biotic interaction terms (e.g.,"eats") using managed, machine readable definitions (e.g., http://purl.obolibrary.org/obo/RO_0002470). Sometimes, existing datasets adopt RO as a way to express interaction types. However, for other datasets, custom terms are mapped into RO using a mapping table. For instance, in case of species interaction in iNaturalist, 151 different iNaturalist interaction types are mapping into RO using the mapping table published at [https://github.com/globalbioticinteractions/inaturalist/blob/master/interaction_types.csv](https://github.com/globalbioticinteractions/inaturalist/blob/master/interaction_types.csv). 

**CM**: <intq>What advice do you have for people interested in using biodiversity data and also new to programming?</intq>

**JP**: First, and most importantly, treat datasets the same as research publications to ensure that future generations can reference and use your work. Similarly, treat your computer program like datasets and research publications. Others (including your future self) should be able to read, understand and perhaps even re-run your program against your original input data to reproduce your results. If you are tempted to follow the latest trends or fashion in data formats or programming language, ask yourself the question: would someone be able to read and understand the data and source code with methods available 10 years *ago*? When I ask myself this question, I often find that UTF-8 encoded text files for both data (e.g., tab-separated values) and source code are the way to go. 

**CM**: <intq>Thank you Jorrit for taking the time to talk with me!</intq> For a more in depth look at what GloBI has to offer see Yikang Li's last two posts: 

1. [Measuring the interactions of species with GloBI](http://curiositydata.org/part1_globi_access/) 
2. [Learn to ask about species interactions effectively using automation and network graph visualization](http://curiositydata.org/part2_globi_exploration/)

You can find Jorrit on Github [@jhpoelen](https://github.com/jhpoelen)