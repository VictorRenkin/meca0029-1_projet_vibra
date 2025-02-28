# MECA0029–1 Theory of Vibration

## Analysis of the Dynamic Behaviour of an Offshore Wind Turbine Jacket

### Academic Year 2023 – 2024
![ViewCount](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/VictorRenkin/meca0029-1_projet_vibra&count_bg=%2379C83D&title_bg=%23555555&icon=github.svg&icon_color=%23E7E7E7&title=views&edge_flat=false)


This repository contains the code and documentation for the MECA0029–1 Theory of Vibration project for the academic year 2023–2024. The project focuses on the analysis of the dynamic behavior of an offshore wind turbine jacket. Resultat projet : 16/20 --> liens overleaf https://www.overleaf.com/read/vbgktrymyhwt#dfe4e2

## Table of Contents

- [Introduction](#introduction)
- [Usage](#usage)
- [Results](#results)

## Introduction

This project is made of 3 parts. In the first one, we are going to calculate the natural frequencies and the mode shape of the jacket. In the second part we are going to calculate the response of the jacket to the attack of a gang of killer whales. And finaly, in the last one we are going to try to reduce the model. 

## Usage
The code is really simple to use, you just need to run the src/main.py file and the code will run automaticaly. As the code is really heavy we use some parametere in order to go faster. You can change the parameters.

```bash
write_e_n       = False      # if you want to write the new nodes and element in a file and the answers
actu_graph      = False      # if you want actualisée graph
c_time          = True       # if you want to calcul the time of part of the programm
nb_elem_by_leg  = 3          #number of element by leg
nMode           = 8          # nombre de mode a calculer,nombre de mode inclus dans la superoposition modale max 8
```	
The code is based on the nodes and elements of the jacket list that you can find in data/init_nodes.txt, If you want to change the structure you need to change it. But be careful beacause the code is not really flexible. We fixe somme rigid element, some leg element and clamped nodes. You can see these in green and red on the graph.

![Turbine](picture/readme/turbine.png)  

## Results

The result are going to be shown in the terminal and on the graphs. The graphs are going to be saved in the folder picture and the results are going to be saved in the folder data/results.
