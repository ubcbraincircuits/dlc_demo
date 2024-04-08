# dlc_demo
DeepLabCut demonstration for the [Hands-on, Neural, Behavioural and Histological Data Analysis Workshop](https://can-acn.org/meeting-2024/satellite-events/hands-on-neural-behavioural-and-histological-data-analysis-workshop-can2024-satellite/) by the UBC Dynamic Brain Circuit Cluster as a part of [CAN 2024](https://can-acn.org/meeting-2024/) meeting.

# Prerequisites
Ensure you either [install Anaconda](https://www.anaconda.com/download) or [install miniconda](https://docs.anaconda.com/free/miniconda/miniconda-install/) on your computer. 

You can verify that you have Anaconda if you have Anaconda Navigator in your applications. You can also verify by running the command `conda --version` in the Terminal (Mac/Linux) or the Anaconda Prompt application (Windows).

# Environment Setup

1. Click the green "Code" button at the top of the page and select "Download Zip". This will download "dlc_demo-main.zip" onto your computer. Unzip this file.
2. Open Terminal/Anaconda Prompt and navigate to the "dlc_demo-main" folder that you just unzipped.
> NOTE: use the commands `ls` to see subdirectories and `cd <subdirectory>` to navigate through your files. You can use `cd ..` to go to the parent directory.
3. In your Terminal/Anaconda Prompt, enter these commands:
   - Windows/Linux/Intel Mac:
    ```
    conda env create -f DEEPLABCUT.yaml
    ```
   - Apple Silicon Mac:
> NOTE: You will need [homebrew](https://docs.brew.sh/Installation). After installing homebrew, download the wget library by running `brew install wget` in the Terminal.

    ```
    #get miniconda
    wget https://repo.anaconda.com/miniconda/Miniconda3-py39_4.12.0-MacOSX-arm64.sh -O ~/miniconda.sh
    bash ~/miniconda.sh -b -p $HOME/miniconda
    source ~/miniconda/bin/activate
    conda init zsh

    #create environment
    git clone DeepLabCut
    conda env create -f conda-environments/DEEPLABCUT_M1.yaml
    ```
4. Activate environment with `conda activate DEEPLABCUT` or `conda activate DEEPLABCUT_M1` depending on the YAML file you installed.