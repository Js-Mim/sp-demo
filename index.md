---
layout: default
---
**Audio production** is a difficult process for most people, and properly manipulating sound to achieve a certain effect is **non-trivial**. We present a **method** that facilitates this process by **inferring appropriate audio effect parameters**. This page provides **supplementary material** to our work that gives an emphasis to **frequency equalization** (EQ). The supplementary material focuses on three "qualitative" aspects:
* Frequence responses
* Audio examples
* Latent feature visualization

# Frequency Responses
Using speech signals from test sub-set we compute a couple frequency responses for the **ideal** and **predicted** EQ parameters.


<p align="center"> <b>Example 1</b></p>

![Example 1](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_a.png)
<p align="center"> <img class="center" src="https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_a_cs.png" width="550" height="383" /> </p>


<p align="center"> <b>Example 2</b></p>                                        

![Example 2](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_b.png)
![Example 2](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_b_cs.png)

<p align="center"> <b>Example 3</b></p>                                        

![Example 3](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_c.png)
![Example 3](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_c_cs.png)

<p align="center"> <b>Example 4</b></p>                                        

![Example 4](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_d.png)
![Example 4](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_d_cs.png)

<p align="center"> <b>Example 5</b></p>                                       

![Example 5](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_e.png)
![Example 5](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_e_cs.png)

<p align="center"> <b>Example 6</b></p>                                       

![Example 5](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_f.png)
![Example 5](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_f_cs.png)

<p align="center"> <b>Example 7</b></p>                                       

![Example 5](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_g.png)
![Example 5](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_g_cs.png)


# Audio Examples
Audio examples using data-points from the test sub-set. The goal is to **match** the **EQ/spectral characteristics** of the **input** signal to the **reference** signal.



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
