---
layout: default
---
**Audio production** is a difficult process for most people, and properly manipulating sound to achieve a certain effect is **non-trivial**. We present a **method** that facilitates this process by **inferring appropriate audio effect parameters**. This page provides **supplementary material** to our work that gives an emphasis to **frequency equalization** (EQ). The supplementary material focuses on three "qualitative" aspects:
..* Frequence responses
..* Audio examples
..* Latent feature visualization

# Frequency Responses
Using speech signals from test sub-set we compute a couple frequency responses for the **ideal** and **predicted** EQ parameters.


<p align="center"> <b>Example 1</b></p>

![Example 1](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_a.png)

<p align="center"> <b>Example 2</b></p>                                        

![Example 2](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_b.png)

<p align="center"> <b>Example 3</b></p>                                        

![Example 3](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_c.png)

<p align="center"> <b>Example 4</b></p>                                        

![Example 4](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_d.png)

<p align="center"> <b>Example 5</b></p>                                       

![Example 5](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/f_r_e.png)



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
We randomly selected four data-points from the test-subset. The selection was based on the loudness of the input and reference sound files. Data-points containing less than -35 dB LUFS, were discarded. Those four data-points are served as input to the three models discussed in our paper. The following figures illustrate *two* signals:
1. The output of the **Latent Feature Extractor** sub-module (__extracted__)
2. The latent signal fed to the **Predictor** sub-module (__fed__).

###### Baseline model
|**Extracted**|**Fed**|
|:-----------:|:-----:|
|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/latent_tc1.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/res_tc1.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/latent_tc2.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/res_tc3.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/latent_tc3.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/res_tc3.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/latent_tc4.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/linear_mel_bl/res_tc4.png)|

###### Baseline model with dB valued representation
|**Extracted**|**Fed**|
|:-----------:|:-----:|
|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/latent_tc1.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/res_tc1.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/latent_tc2.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/res_tc3.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/latent_tc3.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/res_tc3.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/latent_tc4.png)|![ ](https://raw.githubusercontent.com/Js-Mim/sp-demo/master/figures/results/db_mel_bl/res_tc4.png)|


###### Proposed model with dB valued representation
|**Extracted**|**Fed**|
|:-----------:|:-----:|

