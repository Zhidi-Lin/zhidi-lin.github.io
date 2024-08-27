---
layout: page
permalink: /publications/
title: Publications
description:
nav: true
nav_order: 2
---

- See full list of publications on [Google Scholar](https://scholar.google.com/citations?user=8BmRXqMAAAAJ&hl=en)

<!-- <div class='paper-box'><div class='paper-box-image'><div><div class="badge">IEEE ICASSP</div><img src='images/Graphical abstract.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Output-Dependent Gaussian Process State-Space Model](https://ieeexplore.ieee.org/document/9755128)

**Zhidi Lin**, Lei Cheng, Feng Yin, Lexi Xu, Shuguang Cui

[**Project**](https://ieeexplore.ieee.org/document/10095784) <strong><span class='show_paper_citations' data='cuDwCOwAAAAJ&hl=zh-CN'></span></strong>
- We proposed a multi-level detection scheme inspired by human immune system against selective forwarding attacks in WSNs. 
- The detection accuracy and the false alarm rate are much lower than other effective methods.
- We also reduced the computation complexity to $$O(n)$$.
</div></div> -->

## Journal
- <b>[Fedloc: Federated learning framework for data-driven cooperative localization and location data processing](<https://ieeexplore.ieee.org/abstract/document/9250516>)</b><br>
Feng Yin, <b>Zhidi Lin</b>,  Qinglei Kong, Yue Xu, Deshi Li, Sergios Theodoridis and Shuguang Cui. <em>IEEE Open Journal of Signal Processing</em>, vol. 1, pp. 187-215, November 2020. <br>

- <b>[One-Class classifier based fault detection in distribution systems with varying penetration levels of distributed energy resources](<https://ieeexplore.ieee.org/abstract/document/9141286>)</b><br>
<b>Zhidi Lin</b>,  Dongliang Duan, Qi Yang, Xuemin Hong, Xiang Cheng, Liuqing Yang and Shuguang Cui. <em>IEEE Access</em>, vol. 8, pp. 130023-130035, July 2020. <br>
  
- <b>[Data-driven fault localization in distribution systems with distributed energy resources](<https://www.mdpi.com/1996-1073/13/1/275>)</b><br>
<b>Zhidi Lin</b>,  Dongliang Duan, Qi Yang, Xuemin Hong, Xiang Cheng, Liuqing Yang and Shuguang Cui. <em>Energies</em>, vol. 13, no. 1, pp. 275, January 2020. <br>


## Conference
- <b>[Output-dependent Gaussian process state-space model](https://ieeexplore.ieee.org/document/10095784)  [[code]](https://github.com/zhidilin/gpssmProj) </b><br>
<b>Zhidi Lin</b>, Lei Cheng, Feng Yin, Lexi Xu and Shuguang Cui. <em>IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)</em>, 2023. <br>
  
- <b>[Gaussian process regression with grid spectral mixture kernel: Distributed learning for multidimensional data](<https://ieeexplore.ieee.org/document/9841347>)  [[code]](<https://github.com/richardcsuwandi/distributed-gsm>) </b><br>
Richard Cornelius Suwandi\*, <b>Zhidi Lin</b>\*, Yiyong Sun, Zhiguo Wang, Lei Cheng, and Feng Yin. <em>The 25th International Conference on Information Fusion (FUSION)</em>, 2022. <br>

- <b>[Graph neural network for large-scale network localization](<https://ieeexplore.ieee.org/abstract/document/9414520>)  [[code]](<https://github.com/Yanzongzi/GNN-For-localization>)</b><br>
Wenzhong Yan, Di Jin, <b>Zhidi Lin</b>, Feng Yin. <em>IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)</em>, 2021. <br>

- <b>[An interpretable and sample efficient deep kernel for Gaussian process](<http://proceedings.mlr.press/v124/dai20a.html>)</b><br>
Yijue Dai, Tianjian Zhang, <b>Zhidi Lin</b>, Feng Yin, Sergios Theodoridis, Shuguang Cui. <em> Conference on Uncertainty in Artificial Intelligence (UAI)</em>, 2020. <br>

- <b>[A flexible approach for human activity recognition based on broad learning system](<https://dl.acm.org/doi/abs/10.1145/3318299.3318318>)</b><br>
<b>Zhidi Lin</b>, Haipeng Chen, Qi Yang, Xuemin Hong. <em> International Conference on Machine Learning and Computing (ICMLC)</em>, 2019. <br>


- <b>[Data-driven fault localization in distribution systems with distributed energy resources](<https://ieeexplore.ieee.org/document/8974949>)</b><br>
<b>Zhidi Lin</b>, Dongliang Duan, Qi Yang, Xiang Cheng, Liuqing Yang, Shuguang Cui. <em> IEEE Sustainable Power and Energy Conference, (iSPEC)</em>, 2019. <br>

- <b>[One-class classifier based fault detection in distribution systems with distributed energy resources](<https://ieeexplore.ieee.org/abstract/document/8646526>)</b><br>
<b>Zhidi Lin</b>, Dongliang Duan, Qi Yang, Xiang Cheng, Liuqing Yang, Shuguang Cui. <em> IEEE Global Conference on Signal and Information Processing (GlobalSIP)</em>, 2018. <br>

- <b>[Online MEM based binary classification algorithm for China Mobile imbalanced dataset](<https://ieeexplore.ieee.org/abstract/document/8641222>)</b><br>
Shuqing Lin, Feng Yin, <b>Zhidi Lin</b>, Yanbin Lin, Shuguang Cui, Teng Li, Fengli Yu, Wei Yu, Xuemin Hong, Jianghong Shi, Zhi-Quan Luo. <em> IEEE/CIC International Conference on Communications in China (ICCC)</em>, 2018. <br>
  
 (\* indicates equal contributions).<br>


{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}<br>
    {% if pub.address %}{{pub.address}}
    {% endif %} {{pub.month}}, {{pub.year}} {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}
