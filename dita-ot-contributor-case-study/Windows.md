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

Three of us use Windows, but the instructions do not have much guidance for Windows users. Also, some of us have experience with command line operation, while some of us don't. As we encountered and overcame each difficulty, we made plans to improve those instructions. 

## Step-by-Step Narrative
We intend to include here our experience, pain points, commands, and eventually screenshots.

### Installing DITA-OT
https://www.dita-ot.org/dev/topics/installing

| Current steps | My notes |
| ----------- | ----------- |
| 1. Download the dita-ot-4.4.zip package from the project website at dita-ot.org/download. |We had no problems with this step. |
| 2. Extract the contents of the package to the directory where you want to install DITA-OT. Note: The documentation refers to this location as the DITA-OT installation directory, or dita-ot-dir. |The extraction process created a "dita-ot-4.4" folder.|
| 3. Add the absolute path for the bin folder of the DITA-OT installation directory to the PATH environment variable. | Open an Administrator Command Prompt window and enter this command: `setx PATH "%PATH%;C:\path\to\dita-ot-dir\bin" /m`|

### Pain points while installing DITA-OT
* In C:\Users\ruths, I created a "dita-ot-dir" folder. When I extracted the contents of the downloaded zip file into my "dita-ot-dir" folder, that process created a "dita-ot-4.4" folder within my "dita-ot-dir" folder and unzipped all files within that 4.4 subfolder. The solution was to move the contents of the "dita-ot-4.4" folder into my "dita-ot-dir" folder.
* We learned that we need to include \bin in the path when specifying the PATH evnironment variable. In hindsight, we realized that this is what "the absolute path for the bin folder" in step 3 means. We intend to make that more clear.
* For some of us, the PATH environment variable had too many characters. We used the echo command to copy the current string from the variable. We pasted that string into Notepad++. We replaced each semicolon with a semicolon and line break, so that we could see the list of paths more clearly. We manually deleted duplicate paths. We later discovered that Notepad++ has an option to remove duplicates. As a side note, I asked Google about a more direct way to remove duplicates from the PATH environment variable; Google AI said, "On Windows, you can use specialized open-source tools like Pathix on GitHub to automatically remove duplicates and broken links."
* We learned the difference between the set command and the setx command from this page: https://superuser.com/questions/916649/what-is-the-difference-between-setx-and-set-in-environment-variables-in-windows
  * "set modifies the current shell's (the window's) environment values, and the change is available immediately, but it is temporary. The change will not affect other shells that are running, and as soon as you close the shell, the new value is lost until such time as you run set again."
  * "setx modifies the value permanently, which affects all future shells, but does not modify the environment of the shells already running. You have to exit the shell and reopen it before the change will be available, but the value will remain modified until you change it again."
* We learned that we need to run the Command Prompt as an administrator and use the /m option. This page defines the /m option: https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/setx 

### Verifying prerequisite software
https://www.dita-ot.org/dev/topics/prerequisite-software

### Testing the installation 
https://www.dita-ot.org/dev/topics/determining-version-of-ditaot

* We learned that running dita -version from the bin folder always works, because that is where the executable is. When testing whether the installation worked, we need to run dita -version from another folder. 

## Recommendations for DITA-OT Docs
(Concrete suggestions based on your experience.)
