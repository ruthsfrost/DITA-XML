# Case Study: Preparing to Contribute to DITA-OT

## Purpose
* Help myself (Ruth: https://www.linkedin.com/in/ruthfrost)
* Help current volunteer group members: Shane (https://www.linkedin.com/in/shaneataylor), Robin (link TBD), & Eddie (https://www.linkedin.com/in/edwardmcham)
* Help future members  
* Improve DITA-OT onboarding documentation

## Overview of DITA-OT Tasks
1. Installing DITA-OT
1. Verifying prerequisite software
1. Testing the installation by checking the DITA-OT version

## Overview of Git Tasks
1. Forking the DITA-OT docs directory (one member of the volunteer group)
1. Installing Git or GitHub Desktop
1. Cloning the repository

## Why This Case Study Exists
In the chat of a Write the Docs networking meeting, I posted a request for a mentor and/or accountability partners while working on my structured authoring portfolio. A handful of other technical writers replied with interest, so I started coordinating meetings with three of them: Shane, Robin, & Eddie. Shane has experience with contributing to DITA Open Toolkit. He suggested that we volunteer to improve the DITA-OT getting started documentation. In that way, we can learn, help DITA-OT, build our portfolios, build our networks, and support each other all at the same time. We all agreed. Shane offered to be our mentor in this project while I continued scheduling and facilitating meetings. 

Three of us use Windows, but the instructions do not have much guidance for Windows users. As we encountered and overcame each difficulty, we made plans to improve those instructions. 

(Does this sufficiently explain the gaps we observed, the confusion points, and the value of documenting the process?)

## Step-by-Step Narrative
(Write your experience, pain points, screenshots, commands, etc.)

### Installing DITA-OT
https://www.dita-ot.org/dev/topics/installing

| Current steps | My notes |
| ----------- | ----------- |
| 1. Download the dita-ot-4.4.zip package from the project website at dita-ot.org/download. |We had no problems with this step. |
| 2. Extract the contents of the package to the directory where you want to install DITA-OT. Note: The documentation refers to this location as the DITA-OT installation directory, or dita-ot-dir. |When I extracted the contents of the downloaded zip file into my "dita-ot-dir" folder, that process created a "dita-ot-4.4" folder within my "dita-ot-dir" folder and unzipped all files within that 4.4 subfolder. The solution was to move the contents of the "dita-ot-4.4" folder into my "dita-ot-dir" folder.|
| 3. Add the absolute path for the bin folder of the DITA-OT installation directory to the PATH environment variable. |I used this command: setx PATH "%PATH%;C:\Users\ruths\dita-ot-dir" /M|

### Verifying prerequisite software
https://www.dita-ot.org/dev/topics/prerequisite-software

### Testing the installation 
https://www.dita-ot.org/dev/topics/determining-version-of-ditaot

## Recommendations for DITA-OT Docs
(Concrete suggestions based on your experience.)
