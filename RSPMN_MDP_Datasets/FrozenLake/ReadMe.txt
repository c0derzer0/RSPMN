﻿Partial Order = 
[[state],[action],[reward]]
Decision nodes = ["action"]
Utility nodes = ["reward"]
meta_types = [MetaType.DISCRETE]*2+[MetaType.UTILITY]

//////////////////////////////////////////////////////////////////////

MEU:
Value = 0.8
Calculated as max qvalue at start state using an optimally trained DQN

Commands to reproduce MEU:
Install stable-baselines: https://github.com/hill-a/stable-baselines
Train a DQN on the environment dqn_model
use the command:
dqn_model.step_model.step(state) to return the q values for all actions
select max q value for MEU

/////////////////////////////////////////////////////////////////////

Dataset:
Horizon: 8
Instances: 100000
Policy used to generate data: Random policy

////////////////////////////////////////////////////////////////////

Reference:
    "Hill, Ashley and Raffin, Antonin and Ernestus, Maximilian and Gleave, Adam and Kanervisto, 
    Anssi and Traore, Rene and Dhariwal, Prafulla  and Hesse, Christopher and Klimov, Oleg and Nichol, 
    Alex and Plappert, Matthias and Radford, Alec and Schulman, John and Sidor, Szymon and Wu, Yuhuai. (2018). 
    Stable Baselines. GitHub repository. GitHub. https://github.com/hill-a/stable-baselines."







