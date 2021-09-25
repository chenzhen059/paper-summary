This paper compares 25 algorithms about compression quality, compression error and usability which algorithms proposed before ignores. And the findings this paper prodeced present useful guidance for the selection or development of effective trajectory simplification algorithms.
1. One of the significant part of trajectory information using is to query them. When we need to query the trajecotry information from the database, the high accuracy and the speed of searching are our expectation. This paper propose a proper distance measure between two trajectories. Dynamic Time Warping(DTW), Edit distance with Real Penalty(ERP), Longest Common Subsequences(LCSS) and Edit Distance on Real Sequence(EDR) have been proposed to measure the error. The process of EDR measures both length and difference at the same index. The method Window kNN Query(W-kNN) uses EDR when comparing two trajectories.
2. When given a query trajectory T, W-kNN would return the closest k trajectories inside a given time window. But the Window Trajectory Distance Join(W-TDJ) only returns a set including all the trajectories bounded the threshold. 
3. Based on the definition of the precision and the recall, this paper define these two of trajectory clustering. Finally they help to define the F1-measure to judge the effectiveness of the model.

Several findings appear at the end of the paper, it compares these algorithms from compression time and compression error to measure which algorithm is worth of using when you concentrate one part.

Experiment: 1. Baseline methods. 2. Change parameters.
