This paper introduces an algorithm called feature-first trajectory simplification(FFTS) used both on batch data and stream data. At the same time, this algorithm works either by itself or with any existing simplification algorithm. This algorithm utilize GPS status, speed, track angle and the location data. Especially, these data are transformed into six signals for convenience and less storing. And it also represent two proposed algorithm called Douglas-Peucker(DP) and Uniform Sampling(US).
1. The message sent from GPS has many subfields, such as GPS status(valid or invalid data), GPS quality indicator(indicate the signal strong or weak), HDOP(the positional error), Altitude, mean sea-level(geoid), Geoidal separation. But the GPS receiver only solve part of them by editing the configuration.
2. The trajectory data can be transformed into LOST, FOUND, STALL, GO, TURN, EXTRA tune computed by FFTS. These signals represent the user's states. Part of these states are constrained, so some states must happen after another states. 
3. US Algorithm may lost significant information when the trajectory changes greatly. And the US Algorithm can collaborate with FFTS.
4. The distance in this paper computed by two methods. PED measures the shortest distance between a point and a segment. In contrast, SED has a interpolation, so the point may be a virtual data point.
 
This paper shows that FFTS performs better than DP and US, because it uses extra information to judge and compute the true situation.
Experiment: 1. Baseline methods. 2. Change parameters.
