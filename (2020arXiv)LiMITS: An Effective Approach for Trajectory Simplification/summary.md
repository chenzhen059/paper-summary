This paper introduces a effective approach to simplify the trajectory. About Fréchet distance is to measure distance between two objects at all time stamps and take the maximum as the result. About the Minkowski distance, when the parameter p = 1, it is transformed into Manhattan distance and so on. This paper propose an effective method called L-infinity Multidimensional Interpolation Trajectory Simplification. This algorithm updates twice from one dimension to high dimension.
1. The OPW method is a greedy algorithm, and it judges whether a point can be omitted by computing the distance is exceeding the threshold or not.
2. The Link Distance Methods just like construct a polygon, and it can rebuild a path along the corner. This new path simplify the original trajectory.
3. To generalize one demension to high dimensions, this paper utilize the projection to get over them one by one.
4. DI(Direct Interpolation) simply gathers information from all dimensions and ignores the correlation among the projections. So we update the DI approach. Besides in the second iteration, the algorithm subdivides the projection into some pieces which is produced by last iteration. Then combine each piece to form a simplified trajectory.
5. VI(Various Interpolation) is to select a parameter k's value, but I don't know it clearly.

The results of this experiment is studied by compression ratios and efficiency. About the compression ratio, the VI has the highest ratio among all approaches, but it takes more time to simplify the trajectory. All the algorithms designed in this paper outperforms the old algorithms.

Experiment: 1.Baseline methods 2.Change parameters.
