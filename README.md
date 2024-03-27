# Computer-Graphics-Final-Project

When analysing the effects of different stimuli on the microscopic roundworm c.elegans, Divyahsree's work at AP lab involves measuring curvature and thickness of its intestine. Her current method of analysing this includes taking an input z-stack and making measurements in 2d from roughly a middle position of the worm.

The issue with this method is that it entirely ignores curvature and thickness in the 3D dimension. Further, given that certain parts of the image are unclear in 2D, it can be difficult to tell if they are part of the intestine or not, meaning useful information may be lost. We can estimate this information from stacks adjacent to the target image. The current method is also fully manual and in this project I aim to autmoate it

For this project, I aim to create a multi stage pipeline to move from an input z-stack to 3d representation of the microscopic worm c elegans.

Input:

z stacks of different worms with sizes from 14-45. Each layer looks as below

!actual_images.gif

- stage 1: get as close to the trimap as possible
  - 
- stage 2: work on a 3D gaussian matting algorithm to segment what we know to be intestine out (discuss performance with divya)
- stage 3: work on 3D reconstrction of intestine from the matte. Done together with matting algorithm