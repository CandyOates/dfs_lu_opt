# dfs_lu_opt
Create optimal lineups.

Several lineup optimizers following the same interface, each one some variant off the base. The only ones worth looking at are the top 3 (and I don't recommend MultiLineupOptimizer since it's too slow, but otherwise works beautifully).

LineupOptimizer - a standard single lineup optimizer

MultiLineupOptimizer - simultaneously create multiple lineups in the same optimization (compare to serially generating lineups with LineupOptimizer which is suboptimal, this is optimal)

CongruentLineupOptimizer - LineupOptimizer's objective is modified with a quadratic penalty term in deviating from the projected ownership rates for the contest.

RobustLineupOptimizer - A robust optimizer in the projections

RobustCongruentLineupOptimizer - A robust optimizer in the ownership rates (could be modified to be robust in projections also) INCOMPLETE

RobustMultiLineupOptimizer - Robust in the projections for contemporaneous lineup optimization

Dependencies:
- pulp
- numpy
