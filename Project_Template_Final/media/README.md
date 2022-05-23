


# COMP3015: Developer Tool

This is a brief write up about my C2 project submission for COMP3015...
In this write up you will find:
A link to the video walkthrough; A link to the git repo; Information about the project and code.

## The Project
My project is a 3D Model display tool. It displays any 3D model the user wants in an environment that allows them to view the model from different angles and a range of different shading properties.

## Installation/Setup

There is no installation required for the executable, however if you wish to open and run the project in Visual Studio there are some steps that will have to follow.

### Executable
Inside the **Project.zip** there is a folder called **BUILD** It contains the executable **Project_Template.exe**.
### Project
#### Step One: Opening The Dependencies Window
As mentioned above, running the project through Visual Studio requires some basic setup. To compile the project and run it within visual studio you will need set the dependencies to fit your machine.
**First**: Open the **Project** Folder. Inside there is a Visual Studio Solution file: **Project_Template.sln** open it.
![Project SLN in folder](/project.png)
**Next:** In the solution explorer right click **Project_Template** and open **Properties**. This will open the properties window.
![Properties](/properties.png)
**Then**: Open **VC++ Directories** in the **General** drop down there will be **Include Directories** and **Library 
Directories**. Follow these next steps for both.
Click on the file path and then on the drop down arrow that will appear. Then click **<Edit...>**
![Edit Window](/Edit.png)
This will open a new window with two file paths, You need to change this file path to fit your machine.
#### Step Two: Setting Dependencies
Inside the **Project** folder there is a folder called **Dependencies** this folder contains 2 folders (**Include** and **lib**). You must add both of these directories to both the **Include Directories** and **Library Directories**.
![Library Dependencies](/LibraryDep.png)
![Include Dependencies](/IncludeDep.png)
Then Click **Apply**. You can now close this window.

#### Step Three: Build and Run
The project should now build and run. If there are build errors open the project properties as before and ensure that the project has **glfw3.lib** and **opengl32.lib** set and defined under: **Linker**-> **Input**->**Additional Dependencies**
![Additional Dependencies](/glfw.png)
![Additional Additional Dependencies](/AddDep.png)

## Program Operation
Before launching the program you can chose a model you wish to render within the program. 
To render a custom model simply place it within the **media** folder. Ensure the model is called "newModel" and that it is an object file (.obj). 
If you do not chose a model the program will place a low poly model of a VW golf in the scene. (assuming the file has not previously been removed)
### Executable
To run the project open/run the **Project_Template.exe** inside the **BUILD** folder.
The program will run and open a display window.
### Project
To run the project through visual studio ensure you have completed the "Installation/Setup" Portion of this document.
You can then click **Local Windows Debugger** which will run the program.
![Run Program](/media/Debug.png)
### During Run Time
If successfully built the program should display flat plane, a torus - semi submerged inside the plane and the chosen 3D model. The model with oscillate or rotate back and fourth while continuously changing colour. 
![Example Image](/media/Example.png)
This will continue until you wish to stop the program. 
You can stop the program by closing the program window or by stopping the program through visual studio.

## Links
### YouTube Video

### Git Repo
https://github.com/MattHough1999/COMP3015-CW2
