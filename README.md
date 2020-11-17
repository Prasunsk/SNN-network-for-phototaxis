# SNN-network-for-phototaxis
A Spiking Neural Network to model a model phototaxis which is common in primitive life form.Photo-taxis refers to the innate behavioral response of organisms when excited by stimuli like light. It is an outcome of the motility (independent capacity to move using metabolic energy) of certain organisms when it finds certain stimuli .They use sensors in their body.

# Spiking Neural Networks

Spiking neural networks (SNN) have first emerged in computational neuroscience, as an attempt to model the behavior of biological neurons. This has resulted in the Leaky-Integrate-and- Fire (LIF) model, describing neuronal activity as
integration of received spike voltages and weak dissipation (leakage) to the environment. When its voltage reaches a threshold, the neuron fires a spike on its own. Following further inspiration from the brain, neuronal inputs and outputs can be encoded
in the time or rate of the spikes that it receives and emits. This type of information encoding is very robust to errors because a failure to detect a spike or two doesn’t induce a significant error on the average spike rate.

# Block Diagram
![Block ](https://user-images.githubusercontent.com/63877316/99430711-b877e900-292f-11eb-85b0-bdb68a42680d.png)

The sensor detects the light and outputs a voltage
in the range of 0-5V. The voltage is then
scaled down to the working range of the Sensory
Neuron.The voltage is also supplied to a gradient
detector.Based on the light intensity detected
by the sensory neuron and the gradient detected
by the gradient detector , a decision is being
made whether to turn Clockwise or Anticlockwise.
Based on the conditions tested and if all of them
aren’t met, the BOT also travels in a random
fashion. Also if the BOT gets stuck in a certain
place for long period , then it has the ability to
force through that areas ie escaping Local Extrema.

# Neuron Circuit
![neuron1](https://user-images.githubusercontent.com/63877316/99431035-1d334380-2930-11eb-935b-f2b8919fddc7.png)

# Complete network
![full](https://user-images.githubusercontent.com/63877316/99431384-b19da600-2930-11eb-91d8-f73c7d308d30.png)
# Requirements
1. LT Spice: The circuit files are run in LT Spice and the result is returned.
2. Python

# How to run
1. Download all the files in same folder.
2. Make sure that your LT Spice is installed in 'C:\Program Files\LTC\LTspiceXVII'. (This program works for LT Spice version 17)
3. Run the Simulate_SNN file.
4. Run the Neuron_and_Attiny_v4 file.
5. It will take long, because for every step the LT Spice files will be simulated.

# Results
![Picture1](https://user-images.githubusercontent.com/63877316/99432518-42c14c80-2932-11eb-8105-7037aeb0b24c.png)

The red line marks the movement of the worm across a concentration space.
The worm initially starts in a local minima and successfully escapes it. 
