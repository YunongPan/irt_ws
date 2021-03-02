# irt_ws
Workshop for IRT HiWi test.

## Installation
1. Clone this repository  
  
	`cd ~`  
  
	`git clone https://github.com/YunongPan/irt_ws.git`  
  
2. Install dependencies  
  
	`cd ~/irt_ws`  
  
	`rosdep install --from-paths src --ignore-src -r -y`  
  
3. Build the workspace  
  
	`catkin_make`  
  
	
## Testing
1. Start roscore.
  
	`roscore`  
  
2. Start another terminal and source the environment.
  
	`source ~/irt_ws/devel/setup.bash`  
  
3. Start rosnode.
  
	`cd ~/irt_ws/src/image_output/bagfile`  
  
  	`rosrun image_output image_creator.py`  
  
  	*Before start the py.file please don't forget to set `image_creator.py` as an executable file.*  
  
4. Change output model.  
  
	*If you want to output just the first image, please open `image_creator.py`, then set the parameter `more_images_output`  to False.*
	  
  
