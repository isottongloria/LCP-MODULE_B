# LCP-MODULE_B HMM project
#### add this header before generating the z and x sequence:
This functions generates synthetic data to train our HMM.
The generate_initial_state function generates the first hidden state and observation by sampling from the initial state distribution and emission probability distribution, respectively. The generate_sequence function then generates the remaining hidden states and observations by sampling from the transition probabilities and by sampling from a normal distribution with parameters given by the emission matrix.
Note that in the generate_sequence function, the emission probabilities are determined by the current hidden state. This assumes that the emission probabilities are dependent only on the current hidden state, and not on any other factors (such as previous observations).
