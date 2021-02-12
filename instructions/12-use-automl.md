---
lab:
    title: 'Use automated machine learning from the SDK'
---
# Use Automated Machine Learning from the SDK

Determining the right algorithm and preprocessing transformations for model training can involve a lot of guesswork and experimentation.

In this exercise, you'll use automated machine learning to determine the optimal algorithm and preprocessing steps for a model by performing multiple training runs in parallel.
## Create a compute instance 

 1. On the **Compute instances** tab, add a new compute instance with the following settings. You'll use this as a workstation to run code in notebooks. 

    - **Region**: *The same region as your workspace* 

    - **Virtual machine type**: CPU 

    - **Virtual machine size**: Standard_DS11_v2 (search for this type in the options) 

    - **Compute name**: *enter a unique name 

    - **Enable SSH access**: Unselected (you can use this to enable direct access to the virtual machine using an SSH client) 

 2. Wait for the compute instance to start and its status to change to **Running**. 

## Clone and run a notebook 

A lot of data science and machine learning experimentation is performed by running code in *notebooks*. Your compute instance includes fully featured Python notebook environments (*Jupyter* and *JuypyterLab*) that you can use for extensive work; but for basic notebook editing, you can use the built-in **Notebooks** page in Azure Machine learning studio. 

1. In Azure Machine Learning studio, view the **Notebooks** page. 

2. Open a **Terminal**, and ensure its **Compute** is set to your compute instance. 

3. Enter the following commands to clone a Git repository containing notebooks, data, and other files to your workspace: 

    ```bash 

    Use cd Users or cd .. to change into Users directory 

    git clone https://github.com/MicrosoftLearning/mslearn-dp100 

    ```

## Before You start

If you have not already done so, complete the *[Create an Azure Machine Learning Workspace](01-create-a-workspace.md)* exercise to create an Azure Machine Learning workspace and compute instance, and clone the notebooks required for this exercise.

## Open Jupyter

While you can use the **Notebooks** page in Azure Machine Learning studio to run notebooks, it's often more productive to use a more fully-featured notebook development environment like *Jupyter*.

1. In [Azure Machine Learning studio](https://ml.azure.com), view the **Compute** page for your workspace; and on the **Compute Instances** tab, start your compute instance if it is not already running.
2. When the compute instance is running, click the **Jupyter** link to open the Jupyter home page in a new browser tab.

## Use the SDK to run an automated machine learning experiment

In this exercise, the code to run an automated machine learning experiment is provided in a notebook.

1. In the Jupyter home page, browse to the **Users/mslearn-dp100** folder where you cloned the notebook repository, and open the **Use Automated Machine Learning** notebook.
2. Then read the notes in the notebook, running each code cell in turn.
3. When you have finished running the code in the notebook, on the **File** menu, click **Close and Halt** to close it and shut down its Python kernel. Then close all Jupyter browser tabs.

## Clean-up

If you're finished working with Azure Machine Learning for now, in Azure Machine Learning studio, on the **Compute** page, on the **Compute Instances** tab, select your compute instance and click **Stop** to shut it down. Otherwise, leave it running for the next lab.
