Partial Order = 
[
    [
    robot_at_x1y1, robot_at_x1y2, robot_at_x1y3,
    robot_at_x2y1, robot_at_x2y2, robot_at_x2y3,
    robot_at_x3y1, robot_at_x3y2, robot_at_x3y3,
    obstacle_at_x1y1, obstacle_at_x1y2, obstacle_at_x1y3,
    obstacle_at_x2y1, obstacle_at_x2y2, obstacle_at_x2y3,
    obstacle_at_x3y1, obstacle_at_x3y2, obstacle_at_x3y3,
    ],
    [action_move_east], [action_move_north], [action_move_south],
    [action_move_west],
    [reward]
]
Decision nodes = ["action_move_east", "action_move_north", "action_move_south", "action_move_west"]
Utility nodes = ["reward"]
meta_types = [MetaType.DISCRETE]*22+[MetaType.UTILITY]
/////////////////////////////////////////////////////////////////////

MEU:
Value = -4.46
Calculated as average reward over 10000 episodes

Commands to reproduce MEU in rddlsim
Initialize Server:
./run rddl.competition.server files/final_comp/rddl/ 2323 10000
Run Client with VI policy iteration:
./run rddl.competition.Client files/final_comp/rddl localhost MyClientName rddl.solver.mdp.vi.VI 2323 123456 crossing_traffic_inst_mdp__1

/////////////////////////////////////////////////////////////////////

Dataset:
Horizon: 15
Instances: 100000
Policy used to generate data: Random policy

////////////////////////////////////////////////////////////////////

For detailed information on rddlsim usage and examples, refer:
https://github.com/ssanner/rddlsim/blob/master/INSTALL.txt






