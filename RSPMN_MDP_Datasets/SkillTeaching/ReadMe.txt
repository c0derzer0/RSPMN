Partial Order =
[
    [
    states_hintDelayVar_s0,states_hintDelayVar_s1,
    states_updateTurn_s0,states_updateTurn_s1,
    states_answeredRight_s0,states_answeredRight_s1,
    states_proficiencyMed_s0,states_proficiencyMed_s1,
    states_proficiencyHigh_s0,states_proficiencyHigh_s1,
    states_hintedRight_s0,states_hintedRight_s1,
    ],
    [action_giveHint_s0],[action_giveHint_s1], [action_askProb_s0], [action_askProb_s1]
    [reward]
]

Decision nodes = ["action_giveHint_s0"],["action_giveHint_s1"], ["action_askProb_s0"], ["action_askProb_s1"]
Utility node = ["reward"]
meta_types = [MetaType.DISCRETE]*16+[MetaType.UTILITY]
/////////////////////////////////////////////////////////////////////

MEU:
Value = -3.0320
Calculated as average reward over 10000 episodes

Commands to reproduce MEU in rddlsim
Initialize Server:
./run rddl.competition.server files/final_comp/rddl/ 2323 10000
Run Client with VI policy iteration:
./run rddl.competition.Client files/final_comp/rddl localhost MyClientName rddl.solver.mdp.vi.VI 2323 123456 skill_teaching_inst_mdp__1

/////////////////////////////////////////////////////////////////////

Dataset:
Horizon: 10
Instances: 100000
Policy used to generate data: Random policy

////////////////////////////////////////////////////////////////////

For detailed information on usage and examples, refer:
https://github.com/ssanner/rddlsim/blob/master/INSTALL.txt






