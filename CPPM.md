---
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

## Codes
Our codes can be found [here](https://github.com/bacTlink/mitsuba-CPPM)

## BibTeX

```
@article{lin2020cppm,
  title={CPPM: Chi-squared Progressive Photon Mapping},
  author={Zehui Lin and Sheng Li and Xinlu Zeng and Congyi Zhang and Jinzhu Jia and Guoping Wang and Dinesh Manocha},
  journal={ACM Transactions on Graphics (TOG)},
  volume={39},
  number={6},
  article={240},
  year={2020},
  publisher={ACM},
  DOI = {10.1145/3414685.3417822}
}
```
