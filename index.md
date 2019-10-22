---
layout: default
---
**Audio production** is a difficult process for most people, and properly manipulating sound to achieve a certain effect is **non-trivial**. We present a **method** that facilitates this process by **inferring appropriate audio effect parameters** in order to **make an input recording sound better**. This page provides supplementary material to our work that gives an emphasis to **frequency equalization** (EQ).

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
Audio examples using data-points from the test sub-set. The goal is to **match** the **EQ and spectral characteristics** of the **input** signal to the **reference** signal.

<p align="center"> <b>Example 1</b></p>
Input: 
<audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/raw/master/audio_files/ex1_input.wav"></audio>

Reference: 
<audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/raw/master/audio_files/ex1_reference.wav"></audio>

Processed: 
<audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/raw/master/audio_files/ex1_estimated.wav"></audio>

<p align="center"> <b>Example 2</b></p>
Input: 
<audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/raw/master/audio_files/ex2_input.wav"></audio>

Reference: 
<audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/raw/master/audio_files/ex2_reference.wav"></audio>

Processed: 
<audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/raw/master/audio_files/ex2_estimated.wav"></audio>

<p align="center"> <b>Example 3</b></p>
Input: 
<audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/raw/master/audio_files/ex3_input.wav"></audio>

Reference: 
<audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/raw/master/audio_files/ex3_reference.wav"></audio>

Processed: 
<audio controls="1"><source src="https://raw.githubusercontent.com/Js-Mim/sp-demo/raw/master/audio_files/ex3_estimated.wav"></audio>
