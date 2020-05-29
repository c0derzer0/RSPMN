Partial Order =
[
    [
    states_alive_x1y1, states_alive_x1y2, states_alive_x1y3,
    states_alive_x2y1, states_alive_x2y2, states_alive_x2y3,
    states_alive_x3y1, states_alive_x3y2, states_alive_x3y3,
    ],
    [action_set_x1y1], [action_set_x1y2], [action_set_x1y3],
    [action_set_x2y1], [action_set_x2y2], [action_set_x2y3],
    [action_set_x3y1], [action_set_x3y2], [action_set_x3y3],
    [reward]
]
//////////////////////////////////////////////////////////////////////

MEU:
Value = 59.1223
Calculated as average reward over 10000 episodes

Commands to reproduce MEU in rddlsim
Initialize Server:
./run rddl.competition.server files/final_comp/rddl/ 2323 10000
Run Client with VI policy iteration:
./run rddl.competition.Client files/final_comp/rddl localhost MyClientName rddl.solver.mdp.vi.VI 2323 123456 game_of_life_inst_mdp__1

/////////////////////////////////////////////////////////////////////

Dataset:
Horizon: 12
Instances: 100000
Policy used to generate data: Random policy

////////////////////////////////////////////////////////////////////

For detailed information on usage and examples, refer:
https://github.com/ssanner/rddlsim/blob/master/INSTALL.txt




scp -r ht68099@172.22.147.20:/home/ht68099/Projects/Thesis_Project/RDDL1/rddlsim/datasets /home/hari/Desktop/Projects/Thesis_Project/RSPMNMDPDatasets






