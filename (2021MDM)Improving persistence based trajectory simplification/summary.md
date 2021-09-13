This paper introduces three methods for trajectory simplification, such as Douglas Peucker, Persistence MRS, Persistence SDS. The last two methods perform better than the first one, and the SDS work well in most situation than MRS. About the data, trajectory, is divided two class. One is solved by the batch algorithm, the other is solved by the stream algorithm. This needs extra work to process the data.
1.	The main idea of the persistence algorithm is to remove some points from the trajectory T. This algorithm compute the adjacent points' angle to extract minima and maxima. Furthermore, if the point is a local maximum, one is to merge the current component with another which the point is parted of, the other is closing the current component and storing that maximum is used later.
2.	When we tackle the stream data, we must redefine the minima and maxima. For example, a point is minimum if it is smaller than the predecessor and successor.
3.	The key of the SDS Algorithm is to compute the distance between a point and a line connected the predecessor and successor, and the threshold is as well grown in rounds.

Finally, the persistence simplification with beta-pruning leads to clusters of points in curved area leading to unneeded redundancy and defects.
Experiment: 1. Baseline methods. 2. Change parameters.
