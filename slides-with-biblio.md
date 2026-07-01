---
title-slide: false
bibliography: references.bib
csl: vancouver.csl
citeproc: true
theme: serif
background-color: "#ffffff"
transition: slide
navigationMode: linear
hash: true
---

:::: {.columns}
::: {.column width="50%"}

## Sample slides
#### PlaceHolderName
#### Universiti Malaysia Perlis
#### [placeholder@email.com](mailto:placeholder@email.com)

<audio id="bg-music" src="media/audio/sb.m4a" loop></audio>

<div id="audio-credit"
     style="position: absolute; bottom: 40px; right: 20px; font-size: 0.6em; opacity: 0.6;">
  Music: “Adrift” by Scott Buckley (CC BY 4.0)
</div>

<script>
  document.addEventListener('DOMContentLoaded', () => {
    const audio = document.getElementById('bg-music');
    const credit = document.getElementById('audio-credit');

    // hide credit by default
    credit.style.display = 'none';

    const test = new Audio('media/audio/bgm.mp3');

    test.addEventListener('canplaythrough', () => {
      // bgm.mp3 exists → use it, keep credit hidden
      audio.src = 'media/audio/bgm.mp3';
    }, { once: true });

    test.addEventListener('error', () => {
      // bgm.mp3 missing → sb.m4a will play → show credit
      credit.style.display = 'block';
    }, { once: true });

    document.addEventListener('click', () => {
      if (Reveal.getIndices().h === 0) {
        audio.volume = 0.5;
        audio.play();
      }
    }, { once: true });

    Reveal.on('slidechanged', (event) => {
      if (event.indexh > 0) { audio.pause(); }
      else { audio.play(); }
    });
  });
</script>

:::

::: {.column width="50%"}
![](media/pics/logo1.png)
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide one
**Key Concepts:**
- Energy conservation per @carnot1824.
- $\Delta U = Q - W$
:::

::: {.column width="50%"}
![](media/pics/sample.png)
:::
::::

---

<span class="slide-title" data-title="My Hidden Slide Name"></span>

![](media/pics/wide.jpeg)

---

:::: {.columns}
::: {.column width="50%"}
### The Master Equation
The fundamental relation of thermodynamics:

$$\Delta U = Q - W$$

The work done $W$ is positive when the system expands against an external pressure.
:::

::: {.column width="50%"}
<video data-src="media/videos/sample.mp4" data-autoplay loop muted width="100%"></video>
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Visualizing the Gas Law
**Interactive Model:**

- P, V, and T relationships.
- Use the slider to adjust pressure.
- Observe the phase boundary.
:::

::: {.column width="50%"}
<iframe 
  data-src="media/plots/sample.html" 
  width="100%" 
  height="500px" 
  style="border:none;" 
  scrolling="no">
</iframe>
:::
::::

# Machine 1: Temperature Effects

::::: {.columns}
::: {.column width="50%"}
### Statistical Significance
- **p-value**: 0.0000
- Analysis indicates that varying the temperature has a statistically significant impact on product resistance.
- The resistance remains stable and well below the USL of 10 across measured levels.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/temp_res.html' width='100%' height='500px' style='border:none;'></iframe>
:::
:::::

# Machine 1: Pressure Effects

::::: {.columns}
::: {.column width="50%"}
### Statistical Significance
- **p-value**: 0.0000
- Pressure is a critical factor in determining the final resistance of the product.
- Lower resistance levels (which are preferred) are consistently achieved under the tested pressure ranges.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/press_res.html' width='100%' height='500px' style='border:none;'></iframe>
:::
:::::

# Machine 1: Temperature Effects

::::: {.columns}
::: {.column width="50%"}
### Statistical Analysis
- **Significance**: p-value = 0.0000
- Temperature variations significantly impact the electrical resistance of the part.
- Lower resistance is preferred, and results remain safely under the USL of 10.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/temp_res.html' width='100%' height='500px' style='border:none;'></iframe>
:::
:::::

# Machine 1: Pressure Effects

::::: {.columns}
::: {.column width="50%"}
### Statistical Analysis
- **Significance**: p-value = 0.0000
- Adjusting the pressure levels leads to measurable changes in part performance.
- Data shows strong process capability with all parts meeting the specification limit.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/press_res.html' width='100%' height='500px' style='border:none;'></iframe>
:::
:::::

# Machine 1: Temperature Effects

::::: {.columns}
::: {.column width="50%"}
### Statistical Significance
- **p-value**: 0.0000
- Analysis indicates that varying the temperature has a statistically significant impact on product resistance.
- The resistance remains stable and well below the USL of 10 across measured levels.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/temp_res.html' width='100%' height='500px' style='border:none;'></iframe>
:::
:::::

# Machine 1: Pressure Effects

::::: {.columns}
::: {.column width="50%"}
### Statistical Significance
- **p-value**: 0.0000
- Pressure is a critical factor in determining the final resistance of the product.
- Lower resistance levels (which are preferred) are consistently achieved under the tested pressure ranges.
:::

::: {.column width="50%"}
<iframe data-src='media/plots/press_res.html' width='100%' height='500px' style='border:none;'></iframe>
:::
:::::

---
# Bibliography
<div id="refs"></div>
