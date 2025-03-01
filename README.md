# CHO_reactor_modeling

Simulating reaction kinetics of CHO cells in a bioreactor using RNN.

Data is first generated from first principles using a Monod kinetic model. Kinetic model was taken from paper *"Computers and Chemical Engineering"* (2021), by Sara BADR.

The Kinetic model is as follows (excluding the Bleed, Haversting and Suppl terms since we are simulating a fed batch model):

![1740845044268](image/README/1740845044268.png)

Second step is to use the following model to generate data to train a Recurrent Neural Network to predict concentration profiles based on various reactor inlet conditions (ie. concentration, temperature, flowrate).
