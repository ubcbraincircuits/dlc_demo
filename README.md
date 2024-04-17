# dlc_demo
DeepLabCut demonstration for the [Hands-on, Neural, Behavioural and Histological Data Analysis Workshop](https://can-acn.org/meeting-2024/satellite-events/hands-on-neural-behavioural-and-histological-data-analysis-workshop-can2024-satellite/) by the UBC Dynamic Brain Circuit Cluster as a part of [CAN 2024](https://can-acn.org/meeting-2024/) meeting.

# Environment Setup

1. Click the green "Code" button at the top of the page and select "Download Zip". This will download "dlc_demo-main.zip" onto your computer. Unzip this file.
2. Open Terminal/Anaconda Prompt and navigate to the "dlc_demo-main" folder that you just unzipped.
> NOTE: use the commands `ls` to see subdirectories and `cd <subdirectory>` to navigate through your files. You can use `cd ..` to go to the parent directory.
3. In your Terminal/Anaconda Prompt, enter one of these commands:
    ```
    conda env create -f DEEPLABCUT.yaml # for Windows/Linux/Intel Mac
    ```

    ```
    conda env create -f DEEPLABCUT_M1.yaml # for Apple Silicon Mac
    ```

# Downloading Data
All of the data used for this tutorial can be found <a href="https://osf.io/g9d76/?view_only=4dee0dec63c74fe8ab4f5b0a48623c43">here</a>. 

1. <em>Sample Videos</em><br>
For this workshop, you will download some sample videos to try implementing the deeplabcut tool. 
>4 sample videos have been made available; however the steps for all 4 videos will be the same in our workshop. In the interest of time, we recommend downloading <b>only '00602.avi'.</b>
* <b>Click</b> "00602.avi" and select "Download" to download it (258 MB).
* <b>Move</b> the video file into "DLC_DEMO" > "my_files" > "videos".
2. <em>Pre-Trained Model</em> (in the <a href="https://osf.io/a3gmp/?view_only=35aa9a33ad90429a81d73dfce04f70a9">Trained Model OSF Componant</a>)<br>
In the interest of time, a pre-trained model has been provided to use in the second half of the workshop.
* <b>Click</b> "dlc_trained_model.zip" and select "Download" to download it (2.17 GB zipped, 2.33 GB unzipped).
* <b>Move</b> the unzipped "test-AshliandJeff-2021-03-17" folder into "DLC_Demo" > "my_files" > "working_dir"

# Prerequisites
Ensure you either [install Anaconda](https://www.anaconda.com/download) or [install miniconda](https://docs.anaconda.com/free/miniconda/miniconda-install/) on your computer. 

You can verify that you have Anaconda if you have Anaconda Navigator in your applications. You can also verify by running the command `conda --version` in the Terminal (Mac/Linux) or the Anaconda Prompt application (Windows).

# Activate the Environment

Activate environment with `conda activate DEEPLABCUT` or `conda activate DEEPLABCUT_M1`, depending on the YAML file you installed.

To activate Jupyter Notebooks, you can either:

1. Open the Anaconda Navigator application and press "Launch" on Jupyter Notebook.
2. Open Terminal/Anaconda Prompt and run this command in the deeplabcut environment:
    ```
    jupyter notebook
    ```
This will open up the Jupyter Notebook Home Page in your default browser. You will need to navigate to where "dlc_demo" is located on your computer. In this folder, open "dlc_tutorial.ipynb" to start.

Then, you need to run the Jupyter Notebook using the deeplabcut environment we just created. You can modify this by going Kernel > Change Kernel > Python [conda env:DEEPLABCUT] <em>or</em> Python [conda env:DEEPLABCUT_M1] option in the menu bar.

# Workshop Instructions

<b>Start with the 'dlc-tutorial_part-1.ipynb' notebook.</b> This will teach you the basics of setting up labelled data in order to train the model.
Afterwards, you can start on the second notebook, dlc-tutorial_part-2.ipynb, where you will make use of a model that has already been trained to analyze a video and label it accordingly.

# Citation Instructions

If you use DeepLabCut in your future research projects, please read the information <a href="https://github.com/DeepLabCut/DeepLabCut?tab=readme-ov-file">here</a> and reference the original papers as per the author's request. 