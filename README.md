# Data Science: Introduction to Machine Learning for Data Science Python and Machine Learning Studio

## Engagement Expectations

This workshop is meant to be highly interactive. The instructor will lead you in two interactive teaching styles:

1. **Interactive Lecturing:** The majority of content for this workshop is in a Notebook. Though the content will be introduced via PowerPoint, the rest of the workshop will consist of walking them through the Azure Notebooks. During this time, instructors will employ an interactive lecture style, where learners will be asked to participate by asking questions and offering up ideas.

2. **Think, Pair, Share:** For some of the more complex topics, the instructor will use the "Think, Pair, Share" method. This is where you will be asked a question and given about 45 seconds to think quietly to yourself. During this time it is imperative that you are not discussing with others yet. Then, you will have an opportunity to discuss with the 1-2 people next to you. Make sure you don't just share your answer, but *why* you think that is the answer. Finally, the instructor will ask for a few people to share what they discussed with their neighbors.

*Notice*: Various interactive cues are called out in the Notebooks. These are suggestions and at the instructor's discression.

## Today's Schedule

| Hour | | Topic |
| ---- |-| ----- | 
| 9:30 - 10:00am | | Introduction to Data Science Keynote |
| 10:00 - 11:00pm | | Introduction and Refresher [Python](Course%20Materials/1-Python-Reference.ipynb)
| 12:00 - 1:00pm | | Introduction to [NumPy](Course%20Materials/2-NumPy-Reference.ipynb) & [Pandas](Course%20Materials/3-Pandas-Reference.ipynb) |
| 12:00 - 12:30pm | | Lunch | 
| 12:30 - 1:30pm | | Introduction to [Data cleaning and manipulation](Course%20Materials/4-Cleaning_and_Manipulating-Reference.ipynb)| 
| 1:30 - 2:30pm | | [Introduction to Machine Learning Models and Linear Regression](Course%20Materials/5-MachineLearningModels-Reference.ipynbb) |
| 2:00 - 2:10pm | | Break |
| 2:30 - 3:45pm | | [Using the Cloud for Machine Learning with Azure ML Studio](Course%20Materials/6-AzureMLStudio-Reference.ipynb) |
| 3:45 - 4pm | | Wrap Up |

# Using Visual Studio Code 

This repository contains a Visual Studio Code container build.

## One Button Click Deploy of Visual Studio Online Environment

[![Open in Visual Studio Online](https://img.shields.io/endpoint?style=social&url=https%3A%2F%2Faka.ms%2Fvso-badge)](https://online.visualstudio.com/environments/new?name=intro-DataScience&repo=leestott/intro-Datascience)

The setup of the one button click deployment is explained in more details below. 

## Before You Start

The Visual Studio Code Remote - Containers extension lets you use a Docker container as a full-featured development environment. It allows you to open any folder inside (or mounted into) a container and take advantage of Visual Studio Code's full feature set. A .devcontainer folder in your project tells VS Code how to access (or create) a development container with a well-defined tool and runtime stack. This container can be used to run an application or to sandbox tools, libraries, or runtimes needed for working with a codebase.

Workspace files are mounted from the local file system or copied or cloned into the container. Extensions are installed and run inside the container, where they have full access to the tools, platform, and file system. This means that you can seamlessly switch your entire development environment just by connecting to a different container.

# Running the container within VSCode on Windows, Mac or Linux

## The following Requirements are installed as part of the container build

- jupyter
- numpy
- pandas
- scipy
- folium==0.2.1
- matplotlib
- ipywidgets>=7.0.0
- bqplot
- nbinteract==0.0.12

You can run this container from VSCode locally see <a href ='https://code.visualstudio.com/docs/remote/containers' target='_blank'>https://code.visualstudio.com/docs/remote/containers</a>.

## Quick Start Installation

To get started, follow these steps:

Install and configure [Docker](https://www.docker.com/get-started) for your operating system.

Windows / macOS:

Install Docker [Desktop for Windows/Mac](https://www.docker.com/products/docker-desktop)

Right-click on the Docker taskbar item and update Settings / Preferences > Shared Drives / File Sharing with any source code locations you want to open in a container. If you run into trouble, see [Docker Desktop for Windows](https://code.visualstudio.com/docs/remote/troubleshooting#_docker-desktop-for-windows-tips) tips on avoiding common problems with sharing.

Linux:

Follow the official [install instructions for Docker](https://docs.docker.com/install/#supported-platforms) CE/EE for your distribution. If you are using Docker Compose, follow the [Docker Compose](https://docs.docker.com/compose/install/) directions as well.

Add your user to the docker group by using a terminal to run: sudo usermod -aG docker $USER

Sign out and back in again so your changes take effect.

Install [Visual Studio Code](https://code.visualstudio.com/)

Install the [Remote Development extension pack](https://aka.ms/vscode-remote/download/extension)

## Loading the Docker container in Visual Studio Code 

Let's start by using a sample project to try things out.

Clone one of the repository

Start VS Code and click on the quick actions Status Bar item in the lower left corner of the window.
![VScodeStatusBar](https://code.visualstudio.com/assets/docs/remote/common/remote-dev-status-bar.png)

Quick actions Status bar item

Select Remote-Containers: Open Folder in Container... from the command list that appears, and open the root folder of the project you just cloned.

The window will then reload, but since the container does not exist yet, VS Code will create one. This may take some time, and a progress notification will provide status updates. Fortunately, this step isn't necessary the next time you open the folder since the container will already exist.

![ContainerProgress](https://code.visualstudio.com/assets/docs/remote/containers/dev-container-progress.png)

Dev Container Progress Notification

After the container is built, VS Code automatically connects to it and maps the project folder from your local file system into the container. Check out the Things to try section of README.md in the repository you cloned to see what to do next.

Tip: Want to use a remote Docker host? See the Advanced Containers article for details on setup

# Running the container in Visual Studio Online (Browser Experience)

## One Button Click Deploy

[![Open in Visual Studio Online](https://img.shields.io/endpoint?style=social&url=https%3A%2F%2Faka.ms%2Fvso-badge)](https://online.visualstudio.com/environments/new?name=intro-DataScience&repo=leestott/intro-Datascience)

The way this works is as follows is simply calling a specific URL which creates your Visual Studio Online Environment

https://online.visualstudio.com/environments/new?name=intro-DataScience&repo=leestott/intro-Datascience

We also have the domain env.new which allows you to replace online.visualstudio.com making the url shorter

https://env.new?name=intro-DataScience&repo=leestott/intro-Datascience

You could also load this in a new window using target="_blank" so as an example so <a href="https://new.env?name=..." target="_blank">{your image}</a>

## Manual Installation

install this in Visual Studio Online <a href='https://visualstudio.microsoft.com/services/visual-studio-online/' target ='blank'>https://visualstudio.microsoft.com/services/visual-studio-online/ you'll need the following:

- A Microsoft Azure subscription. If you don't already have one, you can sign up for a free trial at <a href ='https://azure.microsoft.com' target='_blank'>https://azure.microsoft.com</a> or a Student Subscription at <a href ='https://aks.ms/azureforstudents' target='_blank'>https://aka.ms/azureforstudents</a>.
- A Visual Studio Online environment. This provides a hosted instance of Visual Studio Code, in which you'll be able to run the notebooks for the lab exercises. To set up this environment:
    1. Browse to <a href ='https://online.visualstudio.com' target='_blank'>https://online.visualstudio.com</a>
    2. Click **Get Started**.
    3. Sign in using the Microsoft account associated with your Azure subscription.
    4. Click **Create environment**. If you don't already have a Visual Studio Online plan, create one. This is used to track resource utlization by your Visual Studio Online environments. Then create an environment with the following settings:
        - **Environment Name**: *A name for your environment - for example, **intro-Datascience**.*
        - **Git Repository**: leestott/intro-Datascience
        - **Instance Type**: Standard (Linux) 4 cores, 8GB RAM
        - **Suspend idle environment after**: 120 minutes
    5. Wait for the environment to be created, and then click **Connect** to connect to it. This will open a browser-based instance of Visual Studio Code.
    6. Wait for a minute or so while the environment is set up for you. It might look like nothing is happening, but in the background we are installing some extensions that you will use in the labs.
    7. Copy your notebooks files and data and undertake your learning

> **Tip**: you can change the color scheme back to a dark background if you prefer - just click the **&#9881;** icon at the bottom left and select a new **Color Theme**.

# Using Azure Notebooks http://notebooks.azure.com

## Content

The primary source of content will be relatively bare Azure Notebooks where the instructor will guide you through discovering the different features of Python, NumPy, Pandas, and general data cleaning and manipulation.

The folder called "Course Material" has all of the content and exercises, plus written explanations and additional features and exercise not covered in this workshop.

## Clone the Content

Cloning creates a copy of an existing project in your own account, where you can then run and modify any notebook or other file in the project. You can also use cloning to make copies of your own projects in which you do experiments or other work without disturbing the original project.

To clone a project

Clone command on project context menu

![NotebookClone](Images/Clone.png)

In the Clone Project popup, enter a name and ID for the clone, and specify whether the clone is public. These settings are the same as for a new project.

After you select the Clone button, Azure Notebooks navigates directly to the copy

## Tips and Tricks

Azure Notebooks is still in Preview. This means that there are some times when it will fail. Here are some tips for avoiding losing your work:
- Ensure their work is being saved. In the Jupyter Notebook there is always one of two messages to the right of the title of the notebook: `(autosaved)` or `(unsaved changes)`. Make sure you're noticing that your work is being saved. You should consider checking every 10 minutes or so.
- Sometimes Notebooks get into a state where the Kernel cannot be started. Sometimes re-starting the kernel will work. But often you will have to somepletely sign out of Azure Notebooks and then sign back in.

## New to Python, Pandas, NumPy or Data Cleaning and Manipulation?

Additionally, if you need a referesher on how to code in Python or work with NumPy or Pandas, we recommend you check out the materials from our other Reactor Workshop:

#### Introduction and Refresher

[Python](Course%20Materials/1-Python-Reference.ipynb)

[NumPy](Course%20Materials/2-NumPy-Reference.ipynb)

[Pandas](Course%20Materials/3-Pandas-Reference.ipynb)

[Data cleaning and manipulation](Course%20Materials/4-Cleaning_and_Manipulating-Reference.ipynb)

## Additional Learning Resources

Microsoft Learn Interactive Labs

[Intro to ML](https://docs.microsoft.com/en-us/learn/paths/intro-to-ml-with-python)

[Building an AI Solution with ML Services](https://docs.microsoft.com/en-us/learn/paths/build-ai-solutions-with-azure-ml-service/)

[Getting Started with Azure DSVM](https://docs.microsoft.com/en-us/learn/paths/get-started-with-azure-dsvm/)

[DataScience Tools in Azure](https://docs.microsoft.com/en-us/learn/paths/explore-data-science-tools-in-azure/)

[Azure Fundamentals](https://docs.microsoft.com/en-us/learn/paths/azure-fundamentals/)
