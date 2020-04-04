+++
date = "2019-03-09T2:27:40-04:00"
math = false
title = "Autonomous morphing of structural form under winds"

[image]
  caption = ""
  focal_point = "Right"
+++

{{< figure library="1" src="Project4_1.jpg">}}

## Description
Motivation: Urbanization in the recent decade is resulting in moving more people to densely populated urban centers like New York City. This is leading to a burgeoning growth of tall buildings. Those urban cities are extremely vulnerable to the impacts of dynamic wind, as the wind-induced interference effects result in the cluster of tall buildings undergoing complex interactions with their surrounding wind environment, which may pose undesirable load effects or even wind hazards on those buildings, especially when we are more frequently facing climate anomalies. To address this challenge, the future building can be designed to interact with its surroundings through actively adapting its form in order to curb the source of dynamic wind loads. 


{{< figure library="1" src="Project4_2.jpg">}}

Morphology: The concept of morphology has been applied to many engineering designs. Most of the inventions originate from mimicking nature, from flying birds that manage to morph their profiles in flight to enhance aerial locomotion, to flowers that come in various shapes with the opening movement of the bud, and to marine animals such as a shark, of which the skin is covered with tiny teeth for drag reduction. These bio-inspirations have been reflected in the engineering design such as aircraft, deployable space structures, and ship hulls.


{{< figure library="1" src="Project4_3.png">}}

My current research focuses on the development of a cyber-physical sensing, control and actuating system that serves as the “central nervous system” of the building. This cyber-physical system harnesses the information collected from sensors and generates commands to actuators. A building equipped with distributed sensors helps mimic a sensing skin that can detect the wind speed and surface pressure. Actuators akin to muscles would allow the building to position its profile into the desired shape to enhance its aerodynamic performance. As sensing inputs and actuating outputs of the building are considerably high-dimensional, Deep Reinforcement Learning is well suited to inform processing in real-time to guide morphing. Control feedback technologies are designed to enhance the predictive performance of the cyber-physical system. To train the neural network, an aerodynamic database that contains the aerodynamic information of a wide range of building forms has been assembled from CFD simulations and wind tunnel experiments.

{{< figure library="1" src="Project4_4.jpg">}}

This cyber-physical system has been successfully mocked on a computational platform for a proof of the concept, in which the building’s cross-section can reconfigure in real-time to reduce the source of dynamic wind loads. Deep deterministic policy gradient (DDPG) algorithm is adopted to learn to predict the future state of the building’s profile with the sensing input of the surrounding wind speed measurements. Model predictive control (MPC) is employed for the close-loop control, tasked with minimizing the difference between the measured and predicted wind loads through tuning the building’s profile. The future applications of autonomously morphing structures would enable civil infrastructures to perform more robustly to conventional wind environments and to situations that are experienced infrequently, thus lessening the impact of climate anomalies and their extremes. 
