---
title: data science
layout: main
---

# Portfolio - data science

<style>
.hide {
  color: white;
}
</style>

In much of my research, I've had to do a mix of data engineering, [GIS][gis], data science and applied machine learning. (Like most computer scientists, I mainly do this kind of work in Python, dropping into C/C++ for speed and brushing up on my R, Matlab/Octave, etc. for specialized tasks.) Some examples -- i.e., those involving projects known to the public -- include:

## Remote sensing

| _thumbnails_{:.hide} | |
|-
| [![bgd-150]][bgd-400] | I applied [**functional nonparametric statistics**][fda] (in Python and [R][refund]) to estimate rainfall statistics using [satellite radar][trmm] data where long-term ground-based measurements are unavailable.<br/><br/>  P.M. Aoki. Functional Data Analysis for Rain Rate Statistics. Project report, CS 229 (Machine Learning), Stanford Univ., 2017. [[PDF]][pdf229] |
| [![plains-150]][plains-400] | I built deep **convolutional neural network** pipelines (both _ab initio_ and **transfer learning**, using [**Keras**][keras] over [**TensorFlow**][tf]) for [multispectral satellite imagery][goes] to estimate rainfall rates where ground-based measurements are unavailable.<br/><br/>  P.M. Aoki. Convolutional Neural Networks for Precipitation Estimation from Geostationary Satellite Imagery. Project report, CS 231n (Convolutional Neural Networks for Visual Recognition), Stanford Univ., 2017. [[PDF]][pdf231n] |
| [![trmm-150]][trmm-400] | At Google Access, I built a global model of rainfall rate statistics (using Python and C++) that used 20 years of [satellite radar][trmm] data to improve upon the then-current [ITU-R prediction model][itu]). The goal was to understand where point-to-point millimeter-wave radios would be appropriate for backhaul networks (particularly in developing countries).<br/><br/> P.M. Aoki. New Rain Rate Statistics for Emerging Regions: Implications for Wireless Backhaul Planning. arXiv:1609.00426, 2016. [[PDF]][pdfsprg] |
| [![ssa-150]][ssa-400] | A more primitive version of the project above addressed a (similarly speculative) question for high-throughput communications satellite coverage in various spectrum bands. |

## System modeling

| _thumbnails_{:.hide} | |
|-
| [![cover-150]][cover-400] | The Google.org Access Strategy &amp; Operations team looked at many methods to provide broadband Internet access to developing countries. I worked with a team of ex-[Big Three][big3] analysts to develop business models based on modeling RF capacity within service areas and estimated broadband demand within them. That's standard telecom practice, but some of the methods under consideration involved coverage from [low Earth orbit][gsat] and the [stratosphere][guav] so I wrote software (mostly Python) to model this. |
| [![zar-150]][zar-400] | A more down-to-earth option involved use of television white space ([TVWS][tvwsza]) spectrum to provide wireless backhaul over large service areas. Given a list of sites, wireless network design can be posed as an optimization problem; I used **mixed integer linear programming (MILP) solvers** to identify the smallest set of sites with fiber backhaul able to cover a target set of public broadband access sites in various developing countries. (Again, this is standard telecom practice.) |

## Experimental studies

| _thumbnails_{:.hide} | |
|-
| | At Google.org, I used bootstrap methods (in [R][qvalue]) to control [**false discovery rate**][fdr] due to multiple comparisons in an experimental study of mobile data use. (The experiment was conducted using internal logging infrastructure that prevented arbitrary processing of log records, for privacy reasons.)<br/><br/> N. Sambasivan, P. Lee, G. Hecht, P.M. Aoki, M.-I. Carrera, J. Chen, M. Youssefmir, D.P. Cohn, P. Kruskall, E. Wetchler and A.T. Larssen. SmartBrowse: Design and Evaluation of a Mobile Data Price Transparency Tool for Mobile Web Use. _Information Technology & International Development 11_ (1), 2015, 21-40. [[PDF]][pdfsb] |

## Environmental sensing

| _thumbnails_{:.hide} | |
|-
| | At Intel Research, I built **logging and processing pipelines** (from device firmware to database) for gas and particulate matter pollution measurements collected by three generations of mobile data collection units.<br/><br/>P. Aoki, A. Woodruff, B. Yellapragada and W. Willett. Environmental Protection and Agency: Motivations, Capacity, and Goals in Participatory Sensing. ACM CHI 2017. [[PDF]][pdfoak]<br/><br/> P. Dutta, P.M. Aoki, N. Kumar, A. Mainwaring, C. Myers, W. Willett and A. Woodruff. Common Sense: Participatory Urban Sensing Using a Network of Handheld Air Quality Monitors. ACM SenSys 2009. [[PDF]][pdfsys]<br/><br/> P.M. Aoki, R.J. Honicky, A. Mainwaring, C. Myers, E. Paulos, S. Subramanian and A. Woodruff. A Vehicle for Research: Using Street Sweepers to Explore the Landscape of Environmental Community Action. ACM CHI 2009. [[PDF]][pdfsfo] |

## Speech processing

| _thumbnails_{:.hide} | |
|-
| [![floors-150]][floors-400] | At Xerox PARC, I built a pipeline to segment and visualize utterances captured from **multi-party speech** (4-10 speakers) to enable human [conversation analysts](https://en.wikipedia.org/wiki/Conversation_analysis) to label the audio segments.<br/><br/> P.M. Aoki, M.H. Szymanski, L. Plurkowski, J.D. Thornton, A. Woodruff and W. Yi. Where's the \`Party' in \`Multi-Party'? Analyzing the Structure of Small-Group Sociable Talk. ACM CSCW 2006. [[PDF]][pdftalk] |

[pdf229]: ../papers/cs229.pdf
[pdf231n]: ../papers/cs231n.pdf
[pdfsprg]: http://arxiv.org/abs/1609.00426
[pdfsb]: ../papers/itid15.pdf
[pdfoak]: ../papers/chi17-science.acm.pdf
[pdfsys]: ../papers/sensys09-demo.acm.pdf
[pdfsfo]: ../papers/chi09.acm.pdf
[pdftalk]: ../papers/cscw06.acm.pdf
[gis]: https://en.wikipedia.org/wiki/Geographic_information_system
[fda]: https://en.wikipedia.org/wiki/Functional_data_analysis
[refund]: https://cran.r-project.org/web/packages/refund/
[trmm]: https://en.wikipedia.org/wiki/Tropical_Rainfall_Measuring_Mission
[keras]: https://keras.io/
[tf]: https://tensorflow.org/
[goes]: https://en.wikipedia.org/wiki/Geostationary_Operational_Environmental_Satellite
[itu]: https://www.itu.int/rec/R-REC-P.837/en
[big3]: https://en.wikipedia.org/wiki/Big_Three_(management_consultancies)
[gsat]: https://archive.is/RC5ps
[guav]: https://archive.is/Dsa8A
[tvwsza]: https://www.tenet.ac.za/tvws
[qvalue]: https://github.com/StoreyLab/qvalue
[fdr]: https://en.wikipedia.org/wiki/False_discovery_rate
[bgd-150]: ../assets/stations.150.png
[bgd-400]: ../assets/stations.400.png
[plains-150]: ../assets/b3.150.png
[plains-400]: ../assets/b3.400.png
[trmm-150]: ../assets/super.mt.bias.121.gauss.5.tif.150.png
[trmm-400]: ../assets/super.mt.bias.121.gauss.5.tif.400.png
[ssa-150]: ../assets/rain.150.jpg
[ssa-400]: ../assets/rain.400.jpg
[cover-150]: ../assets/coverage.150.jpg
[cover-400]: ../assets/coverage.400.jpg
[zar-150]: ../assets/school.150.jpg
[zar-400]: ../assets/school.400.jpg
[floors-150]: ../assets/040813-four-floors-2.150.png
[floors-400]: ../assets/040813-four-floors-2.400.png
