## Advanced Lane Finding
[![Udacity - Self-Driving Car NanoDegree](https://s3.amazonaws.com/udacity-sdc/github/shield-carnd.svg)](http://www.udacity.com/drive)


The Project
---
# only one source code is call 'P2.ipynb'

 ## A.Distortion Correction
 
  
 first the camera will snap some photo with a chessboard saved in the folder: camera_cal
 
 after Correction the chessboard will look as a rectangle

## B.apply binarary hightlight to bird view

### b1.binarary hightlight
 By applying a  Color and Gradient combined filter which can highlight the white line and the yellow line as the lane we want to trace
 
### b2.get the bird view
 with the Perspective Transform we can focus on the front road part and reshapeto the bird view
  
 ## C.trace the line
 
 ### c1. using the Histogram Peaks can recogizate the left lane and the right lane 
 
 ### c2. compute the curveradius and the diff_from_center
 

## D.use a pipline to include all process

 process the pipline on project_video.mp4
 and save the output video as  project_video_out.mp4



# Discussion
the curveradius will somehow have a small value in a discontinuous straight line 
we might patch the Discontinuous part using interpolation in the future
also the video render speed is not enough to process realtime.
the pipeline has to boost up to meet the realtime requirements.
