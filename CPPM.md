﻿---
layout: cppm
---

![Representative Image](CPPM/papers_268s3.jpg)

## Abstract

We present a novel chi-squared progressive photon mapping algorithm (CPPM) that constructs an estimator by controlling the bandwidth to obtain superior image quality. Our estimator has parametric statistical advantages over prior nonparametric methods.
First, we show that when a probability density function of the photon distribution is subject to uniform distribution, the radiance estimation is unbiased under certain assumptions.
Next, the local photon distribution is evaluated via a chi-squared test to determine whether the photons follow the hypothesized distribution (uniform distribution) or not.
If the statistical test deems that the photons inside the bandwidth are uniformly distributed, bandwidth reduction should be suspended.
Finally, we present a pipeline with a bandwidth retention and conditional reduction scheme according to the test results. 
This pipeline not only accumulates sufficient photons for a reliable chi-squared test, but also guarantees that the estimate converges to the correct solution under our assumptions.
We evaluate our method on various benchmarks and observe significant improvement in the running time and rendering quality in terms of mean squared error over prior progressive photon mapping methods.

## Video

<section>
  <button class="btn"  onclick="loadiframe('https://www.youtube.com/embed/1iamshDsQOE')">Youtube</button>
  <button class="btn"  onclick="loadiframe('//player.bilibili.com/player.html?aid=584378199&bvid=BV1tz4y1f7u5&cid=231457632&page=1')">Bilibili</button>
</section>

<iframe id="videoiframe" width="100%" onload="resizeIframe(this)" src="https://www.youtube.com/embed/1iamshDsQOE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

<script>
  function resizeIframe(obj) {
    obj.height = obj.scrollWidth * 0.75;
  }
  function loadiframe(srcstr) {
    document.getElementById('videoiframe').src = srcstr;
  }
</script>

## BibTeX

```
@article{lin2020cppm,
  author = {Lin, Zehui and Li, Sheng and Zeng, Xinlu and Zhang, Congyi and Jia, Jinzhu and Wang, Guoping and Manocha, Dinesh},
  title = {CPPM: Chi-Squared Progressive Photon Mapping},
  year = {2020},
  publisher = {Association for Computing Machinery},
  address = {New York, NY, USA},
  issn = {0730-0301},
  url = {https://doi.org/10.1145/3414685.3417822},
  doi = {10.1145/3414685.3417822},
  volume={39},
  number={6},
  articleno = {240},
  numpages = {12},
  month = nov,
  journal = {ACM Trans. Graph.},
}
```
