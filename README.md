# Variety_training_test_split
Overall, the function performs PCA decomposition and selects specific data points based on their distance to the origin point on the PCA coordinate system.

The function takes in a prepared data frame (df_prep) and performs PCA decomposition with a manually specified number of components. It then calculates the distance of each data point to the origin point on the PCA coordinate system and uses this metric to select certain data points. 

All observations are classified by a combination of the signs of all principal components (-1 or 1). For each class, a certain number of maximum distance points are chosen as corner points. Additionally, a certain number of minimum distance points are chosen as center points. 

Arguments : 

    1) df_prep: a preprocessed dataset that filters out features requiring PCA decomposition.
    
    2) n_components: number of PCs
    
    3) n_obs_each_corner: number of observation on each corner of factorial desgin.
    
    4) n_center_point: number of center points.
