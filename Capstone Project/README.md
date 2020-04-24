# Capstone Project - Urban Sound (Urbansound8k)

Environmental noise or noise pollution, which is defined as an unwanted or harmful outdoor sound created by human activity [1], is a growing problem in urban area. This noise pollution can affect the quality of life and health. Recent studies [2] have shown that exposure to noise pollution may increase the health risk. Therefore, decreasing the noise in the human environment can contribute to increase both the quality of life and health.

Environmental noise monitoring systems continuously measure the sound levels to quantify the noise level. However, it can be of interest to identify the type of noise source. By combining the noise level and the type of noise in real time we can describe the acoustic environment in a more complete way. Based on the outcome, actions can be taken to reduce the noise levels in urban areas. However, finding the type of noise can be a challenging task there an audio recording contains a mix of different noise sources. Here machine learning can be a helpful tool.

A way to build a real time monitoring system is the use of a low cost, small size, low power, wireless embedded device. Today, there is some attention to perform machine learning direct on these devices, so called machine learning on the edge, where we deploy a pre-trained neural network close to the sensor. However, because a limited memory footprint and compute resources the deployment of a neural network on an embedded device can be a challenge. Because these limitations trade-off needs to be made between memory footprint, compute power and the accuracy of the neural network.

The design of a real time smart embedded monitoring system is, given the limit timeframe of this capstone project, out of the scope. The main objective of this capstone project is to take a first (small) step in the design of real time smart embedded system for environmental sound classification (ESC). In this capstone project we focus on the feature engineering and the neural network design.

The dataset used in this project is the [Urbansound8k](https://urbansounddataset.weebly.com/urbansound8k.html) dataset.

<br>

- [Project Specification](https://github.com/JrVerbiest/Udacity_Machine_Learning_Engineer_Nanodegree/blob/master/Capstone%20Project/Capstone%20Project%20Specification.md)
- [Project Proposal](https://github.com/JrVerbiest/Udacity_Machine_Learning_Engineer_Nanodegree/blob/master/Capstone%20Project/Proposal.pdf) & [review from Udacity](https://github.com/JrVerbiest/Udacity_Machine_Learning_Engineer_Nanodegree/blob/master/Capstone%20Project/Capstone%20Proposal%20Review.md)
- [Project Report](https://github.com/JrVerbiest/Udacity_Machine_Learning_Engineer_Nanodegree/blob/master/Capstone%20Project/Report.pdf) & [review from Udacity](https://github.com/JrVerbiest/Udacity_Machine_Learning_Engineer_Nanodegree/blob/master/Capstone%20Project/Capstone%20Report%20Review%20Part%202.md)
- Notebooks: 
  - [Part 1: feature engineering and CNN](https://github.com/JrVerbiest/Udacity_Machine_Learning_Engineer_Nanodegree/blob/master/Capstone%20Project/UrbanSound8k%20-%20Capstone%20Project%20-%20Part%201.ipynb)
  - [Part 2: Cross Validation](https://github.com/JrVerbiest/Udacity_Machine_Learning_Engineer_Nanodegree/blob/master/Capstone%20Project/UrbanSound8k%20-%20Capstone%20Project%20-%20Part%202.ipynb)

<br>

##  Software & libraries 

- Python 3.7.3
- pandas 0.24.2
- NumPy 1.16.4
- Matplotlib 3.1.0
- Scikit-learn 0.21.2
- LibROSA 0.6.3
- Keras 2.2.4

<br>

## UrbanSound8k Dataset

[Urbansound8k](https://urbansounddataset.weebly.com/urbansound8k.html) dataset contains 8732 labeled sound excerpts (<=4s) of urban sounds from 10 classes: air_conditioner, car_horn, children_playing, dog_bark, drilling, enginge_idling, gun_shot, jackhammer, siren, and street_music.

[A Dataset and Taxonomy for Urban Sound Research](http://www.justinsalamon.com/uploads/4/3/9/4/4394963/salamon_urbansound_acmmm14.pdf), J. Salamon, C. Jacoby and J. P. Bello, 22nd ACM International Conference on Multimedia, Orlando USA, Nov. 2014.

<br>

## Reference

[1] Directive, EN, Directive 2002/49/EC of the European Parliament and of the Council of 25 June 2002 Relating to the Assessment and Management of Environmental Noise.

[2] L. Poon, The Sound of Heavy Traffic Might Take a Toll on Mental Health, CityLab, [Online Available](https://www.citylab.com/equity/2015/11/city-noise-mental-health-traffic-study/417276/)

<br>

---

Last modified: 1 January 2020
