# Assignment 1.1: Automated GIS Analyses using the QGIS Model Builder

This is the first part of assignment 1. The second part will follow next week. 

**Submission deadline is Friday, Nov 20 2020 on your forked GitHub repository.**

This is a **group assignment** in which you are supposed to solve these exercises in pairs of two students. Please explain things to each other especially git and the Model Builder if one of you already has experience with it. 

In this assignment you will use the QGIS Model Builder within the QGIS Processing Toolbox to calculate the Topographic Wetness Index (TWI) for a study area in Slovenia. This index is frequently used within flood risk analysis as described by [Pourali et al (2016)](https://idp.springer.com/authorize/casa?redirect_uri=https://link.springer.com/content/pdf/10.1007/s12061-014-9130-2.pdf&casa_token=556pHuCiUZQAAAAA:WO37dPPHnd7NObyhuElNhxtywKsM0oq7Z9WX6odYtXlU_oGh7VyPl4_blLJZXa4u8ztt05CSVIkqj_O_ku0). 

#### 0. Fork and clone the repository 
Although you will solve the exercises together as a group, every student in your group should 
* fork this repository using their own account and 
* clone it to their computer.

This is easier than working together on the same repository, since we haven't learned how to collaborate on the same repository. 

#### 1. Answer the following questions: [2pt]
  1. What is the Topographic Wetness Index? 
  2. How are the TWI values related to the flood probability?
  
Write your answer in a new file called answers.txt in this repository. 

**&rarr; Synchronize with git** Create a commit containing the the new file _answers.txt_ and push it to GitHub. You can find an introduction to git and two videos in the [wiki](https://github.com/fossgis2021/home/wiki/git)
  
#### 2. Search for FOSS GIS tools to calculate the TWI. [3pt]
Search within the QGIS Processing Toolbox, but also for other FOSS projects (e.g. Python or R based).

Add your answer to the file _answers.txt_ in this repository. 

**&rarr; Synchronize with git** Create a commit containing the edited file _answers.txt_ and push it to GitHub. You can find an introduction to git and two videos in the [wiki](https://github.com/fossgis2021/home/wiki/git)

#### 3. Implement the calculation of the TWI using the QGIS Model Builder. [5pt]

The data for this analysis can be downloaded from [here](https://heibox.uni-heidelberg.de/f/d0392835aa3b43a7a676/). It contains a SRTM digital elevation model (DEM) with 1 arc second resolution and a vector file containing the area of interest (AOI), a region on the coast of Slovenia.  

Create a model within the QGIS Model Builder which contains the following processing steps:
1. Clip the DEM to the study area. 
2. Reproject the DEM to a suitable coordinate reference system.
2. Calculate the TWI. 

**Note:** For a short tutorial on the Model Builder watch this [video](https://www.youtube.com/watch?v=eZb5VLTc9-o&t=449s).

**&rarr; Synchronize with git** Copy your your \*.model file to your repository. Create a commit and pushing it to GitHub. 


#### References

Pourali, S. H., Arrowsmith, C., Chrisman, N., Matkan, A. A., & Mitchell, D. (2016). Topography wetness index application in flood-risk-based land use planning. Applied Spatial Analysis and Policy, 9(1), 39-54.
