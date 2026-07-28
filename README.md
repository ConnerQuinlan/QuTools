<h1>QuTools: ECM-Oriented Geometry Tools for QuPath and FIJI</h1>
<p>*"These are the tools that I wish I had when I started using QuPath"*</p>
For the corresponding methods paper, I am rolling out QuTools as I translate the logic from its initial language to the various languages such as JYthon and Groovy. 
The file structure for Step1-Fiji Batch Normalizer must be as follows with whatever names you need:
  Experiment Folder>  
  Group1 | Group2 | Group3 | Groupx... | >
  Channel 1.tif | Channel 2.tif | Channel.... |
This means that each "group" will be in its own folder with each individual channel separated as described in the methods paper. 

Your objective with Step 1 is to recreate the normalization based on the background subtraction and max-value capping as done in the paper. 
Step2 is to run the autofluorescent signal removal masking. For small-plex images, do not run this. For high-plex images, run this. You may have to mess around with the settings hence the inital dialogue box. My settings that worked the best were Sigma 3, Expansion 10, Triangle method. This is designed to be run on the FULLY ASSEMBLED IMAGE, so you will need to assemble the Channel Stack tiff prior to running this. 


QuTools-Extension.Jar is for QuPath v0.7.0 
In order to install it, simply download the file, drag it over QuPath while it is open, and it will install it automatically. If it does not appear, please restart QuPath V0.7.0.

<h1>Video Tutorial</h1>
<h2>FIJI Workflow</h2>
<h3>Set Up Files</h3>


https://github.com/user-attachments/assets/dd1cdd21-8720-46e2-aeed-0c47a63bc1a7
<h3>Step 1 Script Setup</h3>


https://github.com/user-attachments/assets/30266492-6d61-406b-9e0f-509d2584ec59
<h3>Normalization</h3>


https://github.com/user-attachments/assets/eefa2b29-8747-44dc-afac-0161c61aaa5a
<h3>Noise Reduction</h3>


https://github.com/user-attachments/assets/2f9b7ed9-87a4-4d74-88f7-ec156d82c90c
<h2>QuPath Workflow</h2>
<h3>Setup</h3>


https://github.com/user-attachments/assets/854d41dc-994f-4ab0-93c3-05b4317cbe1b
<H3>Segmentation</H3>


https://github.com/user-attachments/assets/bb20366b-dfc1-48a4-843b-68c00239d353
<h3>StarDist</h3>


https://github.com/user-attachments/assets/bafd8630-be97-4508-9a7b-3b8fde5d1a37

<h3>Analysis</h3>


https://github.com/user-attachments/assets/bbf61f55-85ca-4e57-8a37-078ac8736271
<h3>Export Histograms</h3>


https://github.com/user-attachments/assets/9821d9a0-7b93-469d-b504-b89929906227



