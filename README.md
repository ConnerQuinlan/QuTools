For the corresponding methods paper, I am rolling out QuTools as I translate the logic from its initial language to the various languages such as JYthon and Groovy. 
The file structure for Step1-Fiji Batch Normalizer must be as follows with whatever names you need:
  Experiment Folder>  
  Group1 | Group2 | Group3 | Groupx... | >
  Channel 1.tif | Channel 2.tif | Channel.... |
This means that each "group" will be in its own folder with each individual channel separated as described in the methods paper. 

Your objective with Step 1 is to recreate the normalization based on the background subtraction and max-value capping as done in the paper. 
Step2 is to run the autofluorescent signal removal masking. For small-plex images, do not run this. For high-plex images, run this. You may have to mess around with the settings hence the inital dialogue box. My settings that worked the best were Sigma 3, Expansion 10, Triangle method. This is designed to be run on the FULLY ASSEMBLED IMAGE, so you will need to assemble the Channel Stack tiff prior to running this. 
