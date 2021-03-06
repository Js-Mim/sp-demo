---
layout: default
---
Supplementary material for our [ICASSP2020 paper](https://ccrma.stanford.edu/~njb/research/icassp2020_style_transfer.pdf).

The presentation of our work:

[![](https://img.youtube.com/vi/_djACv33tuk/0.jpg)](https://www.youtube.com/watch?v=_djACv33tuk)

### Authors
[Stylianos I. Mimilakis](https://github.com/Js-Mim), [Nicholas J. Bryan](https://research.adobe.com/person/nicholas-j-bryan/), [Paris Smaragdis](https://paris.cs.illinois.edu/)

# Introduction
**Audio production** is a difficult process for most people, and properly manipulating sound to achieve a certain effect is **non-trivial**. We present a **method** that facilitates this process by **inferring appropriate audio effect parameters**. This page provides **supplementary material** to our work that gives an emphasis to **frequency equalization** (EQ). The supplementary material focuses on three "qualitative" aspects:
* Frequency responses
* Audio examples
* Latent feature visualization
* Application Scenarios

# Frequency Responses
Using speech signals from test sub-set we compute a couple frequency responses for the **ideal** and **predicted** EQ parameters. The generation of the EQ parameters is random, following the reported experimental setup. These examples are illustrative for the inspection of the proposed method.


<p align="center"> <b>Example 1</b></p>

![Example 1](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_a.png)
<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_a_cs.png" width="600" height="380" /> </p>


<p align="center"> <b>Example 2</b></p>                                        

![Example 2](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_b.png)
<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_b_cs.png" width="600" height="380" /> </p>


<p align="center"> <b>Example 3</b></p>                                        

![Example 3](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_c.png)
<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_c_cs.png" width="600" height="380" /> </p>


<p align="center"> <b>Example 4</b></p>                                        

![Example 4](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_d.png)
<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_d_cs.png" width="600" height="380" /> </p>


<p align="center"> <b>Example 5</b></p>                                       

![Example 5](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_e.png)
<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_e_cs.png" width="600" height="380" /> </p>


<p align="center"> <b>Example 6</b></p>                                       

![Example 5](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_f.png)
<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_f_cs.png" width="600" height="380" /> </p>


<p align="center"> <b>Example 7</b></p>                                       

![Example 6](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_g.png)
<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_g_cs.png" width="600" height="380" /> </p>



# Audio Examples
Audio examples using data-points from the test sub-set. The goal is to **match** the **EQ/spectral characteristics** of the **input** signal to the **reference** signal.

## Speech Signals

|**Example**|**Input**|**Reference**|**Processed**|
|:--------:|:-------:|:-----------:|:-----------:|
| Ex. 1 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex1_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex1_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex1_estimated.wav"></audio> |
| Ex. 2 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex2_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex2_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex2_estimated.wav"></audio> |
| Ex. 3 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex3_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex3_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex3_estimated.wav"></audio> |
| Ex. 4 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex4_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex4_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex4_estimated.wav"></audio> |
| Ex. 5 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex5_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex5_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex5_estimated.wav"></audio> |
| Ex. 6 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex6_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex6_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex6_estimated.wav"></audio> |
| Ex. 7 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex7_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex7_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex7_estimated.wav"></audio> |
| Ex. 8 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex8_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex8_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex8_estimated.wav"></audio> |
| Ex. 9 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex9_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex9_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex9_estimated.wav"></audio> |
| Ex. 10 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex10_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex10_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/audio_files/ex10_estimated.wav"></audio> |

## Music Signals
The tests on music signals were simply performed by using the proposed method, that was trained on speech signals of 3 seconds, with variable length excerpts, i.e., no re-training or any additional routines were considered. The music signals were acquired from [MUSDB18](https://zenodo.org/record/3338373). To demonstrate the variability of the predicted EQ settings, we consider neighbouring music excerpts as examples and we also swap between what our proposed method considers as input and what was reference.

|**Example**|**Input**|**Reference**|**Processed**|
|:--------:|:-------:|:-----------:|:-----------:|
| Ex. 1 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_1_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_1_target.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_1_processed.wav"></audio> |
| Ex. 2 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_2_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_2_target.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_2_processed.wav"></audio> |
| Ex. 3 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_3_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_3_target.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_3_processed.wav"></audio> |
| Ex. 4 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_4_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_4_target.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_4_processed.wav"></audio> |
| Ex. 5 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_5_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_5_target.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_5_processed.wav"></audio> |
| Ex. 6 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_6_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_6_target.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_6_processed.wav"></audio> |
| Ex. 7 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_7_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_7_target.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_7_processed.wav"></audio> |
| Ex. 8 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_8_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_8_target.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_8_processed.wav"></audio> |
| Ex. 9 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_9_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_9_target.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_9_processed.wav"></audio> |
| Ex. 10 | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_10_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_10_target.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/mus_ex_10_processed.wav"></audio> |

# Latent Business

We randomly selected four data-points from the test-subset. The selection was based on the loudness of the input and reference sound files, and covering two successful and two not so successful predictions according to the computed test-error. Data-points containing less than -35 dB LUFS, were discarded. Those four data-points are served as input to the three models discussed in our paper. The following figures illustrate *two* signals:
1. The output of the **Latent Feature Extractor** sub-module (*extracted*)
2. The latent signal fed to the **Predictor** sub-module (*fed*).

###### Baseline model

|**Extracted**|**Fed**|
|:-----------:|:-----:|
| ![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/latent_tc1.png) | ![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/res_tc1.png) | 
![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/latent_tc2.png) | ![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/res_tc3.png)|
![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/latent_tc3.png) | ![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/res_tc3.png)|
![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/latent_tc4.png) | ![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/res_tc4.png)|

###### Baseline model with dB valued representation

|**Extracted**|**Fed**|
|:-----------:|:-----:|
|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/latent_tc1.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/res_tc1.png)|
![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/latent_tc2.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/res_tc3.png)|
![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/latent_tc3.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/res_tc3.png)|
![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/latent_tc4.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/res_tc4.png)|


###### Proposed model with dB valued representation

|**Extracted**|**Fed**|
|:-----------:|:-----:|
| ![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_pm/latent_tc1.png) | ![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_pm/comp_tc1.png)|
![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_pm/latent_tc2.png) | ![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_pm/comp_tc2.png)|
![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_pm/latent_tc3.png) | ![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_pm/comp_tc3.png)|
![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_pm/latent_tc4.png) | ![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_pm/comp_tc4.png)|


###### Observations & Take-home Messages
From the above collection of figures we could potentially conclude the following:
1. Our theoretical expectactions, presented in the corresponding paper, are not very far away from the experimental realization (illustrated above). That is especially for the baseline models that employ a deterministic function, i.e., the element-wise subtraction, for the computation of the latent space that is *fed* to the predictor.
2. The baseline method, that uses the element-wise subtraction, yields a degenerate (sparse and low-norm vector, wrt to our problem) latent space. This *partially* supports the experimental results presented in the paper.
3. A bartrick is to employ a dB valued representation. During training, via gradient descent, it is shown that it extends the numerical range of values in the latent space dramatically. However, this simply increases the values of the observed learned residue and the *fed* signal still suffers from a couple of nullified coefficients.
4. Using the proposed method, the latent information *fed* to the predictor lies in sensible numerical ranges.
5. The introduced novelties in our proposed method, not only alleviate the nullification of information relevant to the predictor, but also "bias" our expected predictor in a exploitable, for the predictor, manner.



# Application Scenarios
Consider a number of speech recordings that contain a perceptually disturbing frequency content. We want to predict an EQ setting that matches the frequency of a provided produced recording.
The following audio examples demonstrate the above in two scenarios:
1. "Annoying high sibilance" to "produced speech content", and **vice versa**
2. "Muddy bass" to "produced speech content", and **vice versa**

###### Annoying high sibilance
<p align="center"> <b>Example 1</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex1_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex1_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex1_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex1.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 2</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex2_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex2_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex2_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex2.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 3</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex3_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex3_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex3_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex3.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 4</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex4_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex4_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex4_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex4.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 5</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex5_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex5_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex5_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex5.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 6</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex6_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex6_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex6_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex6.png" width="600" height="380" /> </p>


<p align="center"> <b>Example 7</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex7_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex7_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex7_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex7.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 8</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex8_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex8_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex8_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/sibilance_examples/ex8.png" width="600" height="380" /> </p>

###### Muddy bass
<p align="center"> <b>Example 1</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex1_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex1_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex1_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex1.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 2</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex2_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex2_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex2_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex2.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 3</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex3_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex3_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex3_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex3.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 4</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex4_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex4_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex4_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex4.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 5</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex5_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex5_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex5_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex5.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 6</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex6_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex6_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex6_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex6.png" width="600" height="380" /> </p>


<p align="center"> <b>Example 7</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex7_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex7_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex7_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex7.png" width="600" height="380" /> </p>

<p align="center"> <b>Example 8</b></p>

|**Input**|**Reference**|**Processed**|
|:-------:|:-----------:|:-----------:|
| <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex8_input.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex8_reference.wav"></audio> | <audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex8_estimated.wav"></audio> |

<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/application_examples/bassy_examples/ex8.png" width="600" height="380" /> </p>
