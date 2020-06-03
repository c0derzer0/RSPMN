Partial Order = 
[[state],[action],[reward]]

/////////////////////////////////////////////////////////////////////

MEU:
Value = 9
Calculated as average reward over 10000 timesteps

Commands to reproduce MEU:
Install stable-baselines: https://github.com/hill-a/stable-baselines
Train a DQN on the environment dqn_model
Calculate Average reward

/////////////////////////////////////////////////////////////////////

Dataset:
Horizon: 15, 50
Instances: 20000
Policy used to generate data: Random action with probability 0.7 and
			      action from optimally trained DQN with 
                              proability 0.3

////////////////////////////////////////////////////////////////////

Reference:
    "Hill, Ashley and Raffin, Antonin and Ernestus, Maximilian and Gleave, Adam and Kanervisto, 
    Anssi and Traore, Rene and Dhariwal, Prafulla  and Hesse, Christopher and Klimov, Oleg and Nichol, 
    Alex and Plappert, Matthias and Radford, Alec and Schulman, John and Sidor, Szymon and Wu, Yuhuai. (2018). 
    Stable Baselines. GitHub repository. GitHub. https://github.com/hill-a/stable-baselines."







