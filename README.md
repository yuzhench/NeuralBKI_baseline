#### step 1: initalize the conda env 
```
conda env create -f environment.yml
conda activate NeuralBKI
```


#### step 2: Download the Datasets
* KittiOdometry
  * We preprocessed the Kitti Odometry following [Yang et al.](https://github.com/shichaoy/semantic_3d_mapping/tree/master/preprocess_data#readme).  
  * You can download the preprocessed data [here](https://curly-dataset-public.s3.us-east-2.amazonaws.com/ConvBKI/kitti_odometry/kitti_odometry.zip).
  * kitti_odometry.yml file is located in Config directory. data_dir should be the location of the KittiOdometry dataset.


#### step 3: run the generate_results.py and check the time measurement 
* only measure the time of "Add points to map"
* measure time with visualization 

```
#on my computer, the result looks like this:
Total_frame num is:  46
Total_time only add points to map is:  4.799755573272705
Total_time with visualization 55.51151895523071
average time per frame with only add points to map is:  0.1043425124624501
FPS is:  9.583821362935568
average time with visualization per frame is:  1.2067721512006677
FPS with visual is:  0.8286568421429501
```
