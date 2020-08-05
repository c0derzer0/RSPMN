Partial Order =
[
    [
    states_elevator_closed,
    states_person_in_elevator_going_down,
    states_elevator_at_floor_f0, states_elevator_at_floor_f1, states_elevator_at_floor_f2,
    states_person_waiting_up_f0, states_person_waiting_up_f1, states_person_waiting_up_f2,
    states_elevator_dir_up,
    states_person_waiting_down_f0, states_person_waiting_down_f1, states_person_waiting_down_f2,
    states_person_in_elevator-going-up
    ],
    [action_close_door],[action_move_current_dir], [action_open_door_going_up], [action_open_door_going_down]
    [reward]
]

Decision nodes = ["action_close_door", "action_move_current_dir", "action_open_door_going_up", "action_open_door_going_down"]
Utility node = ["reward"]
meta_types = [MetaType.DISCRETE]*17+[MetaType.UTILITY]
/////////////////////////////////////////////////////////////////////

MEU:
Value = -7.3414
Calculated as average reward over 10000 episodes

Commands to reproduce MEU in rddlsim
Initialize Server:
./run rddl.competition.Server files/final_comp/rddl/ 2323 10000
Run Client with VI policy iteration:
./run rddl.competition.Client files/final_comp/rddl localhost MyClientName rddl.solver.mdp.vi.VI 2323 123456 elevators_inst_mdp__1

/////////////////////////////////////////////////////////////////////

Dataset:
Horizon: 10
Instances: 100000
Policy used to generate data: Random policy

////////////////////////////////////////////////////////////////////

For detailed information on usage and examples, refer:
https://github.com/ssanner/rddlsim/blob/master/INSTALL.txt






