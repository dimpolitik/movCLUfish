# MovCLUfish
A tool for visualising fish movement patterns from individual-based models using data mining. It's based on the paper

•	Politikos, D.V., Kleftogiannis, D., Tsiaras, K. Rose, K. MovCLUFish: A data mining tool for discovering novel fish movement patterns from individual-based models (under review).

The repository includes:

* Source code in Matlab for implementing MovCLUFish
* Source code in R for implementing MovCLUFish

![Farmers Market Finder Demo](Fish_tracks_movement.gif)

## Functions

### Tracking Moving Centroids (TMC)

- tmc.m: compute the cenroids clusters of fish tracks using SOM.

% Inputs:
  
% Outputs: 
% 1. centroids: centroids of clusters
% 2. sil: silouette coefficients 
% -------------------------------------------------------------------------
% Example of use:
% [centroids, sil] = tmc(x,y,1,20,3,2,[22 26.5 39 41.2]);
% See also visualize_tcm.m example for ploting the centroids

* **visualize_tmc.m**: plot the centroid clusters generated from tmc.m and their shift.

### Aggregating Moving Clusters (AMC)

* **amc.m**: compute the surface baf area of moving clusters with SOM.

* **visualize_amc_bagplot.m**: visualize bagplots of moving clusters at specific timestamps.

### Tracking Fish Mobility (TFM). 

* **tfm.m**: tracking of fish mobility between moving clusters







