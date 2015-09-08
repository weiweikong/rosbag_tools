
Some tools to manage `rosbag` topics.

## `image_converter.cpp`
- extract images from `rosbag` to opencv format frame by frame
- TODO
	- save each frame seperately
	- convert to a video


## `bag2csv.py`
- convert `rosbag` topics to csv file
- usage
```
python bag2csv.py -b your_bag_file_name.bag -t /your_topic
```

- Reference: https://github.com/unl-nimbus-lab/bag2csv
