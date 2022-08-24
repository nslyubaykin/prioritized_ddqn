# Prioritized DDQN with [ReLAx](https://github.com/nslyubaykin/relax)
Example Prioritized DDQN implementation with [ReLAx](https://github.com/nslyubaykin/relax)

This repository contains an example implementation of Prioritized Experience Replay with DDQN algorithm
 
The performance versus vanilla DDQN is measured by averaging learning curves (for separate evaluation environment) over 4 experiments with random environment seeds.

The results are summarized in the following plot (DDQN is run only for 1.5m envsteps to save time):

![per_benchmark](https://github.com/nslyubaykin/prioritized_ddqn/blob/master/per_benchmark.png)

The differences in hyper-parameters settings between PER-DDQN and vanilla DDQN are the presence of prioritized experience replay and four times decreased learning rate for PER comparing to uniform sampling case. 
We can see that on that task PER-DDQN performs worse than a vanilla uniform version. However, that also may be the case only for this training horizon (1.5m steps instead of 200m)

__Resulting Policy__

https://user-images.githubusercontent.com/67604207/186367375-3a3cc34a-f773-422e-9180-0085b20eafd9.mp4
