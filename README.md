# bioimage-analysis-workshop-24-25
All material for bioimage analysis workshop at Yan-ming University, Taipei, with the Investigator Taiwan. Note that these materials have been adopted from:

- **EMBL Bio-IT bioimage analysis workshop**, especially the part by Toby Hodges and Jonas Hartmann: [https://git.embl.de/grp-bio-it-workshops/image-analysis-with-python](https://git.embl.de/grp-bio-it-workshops/image-analysis-with-python)
- **Introduction to Bioimage Analysis** by Pete Bankhead: [https://bioimagebook.github.io/](https://bioimagebook.github.io/)
- **Bioimage Analysis Lecture 2020** by Robert Haase: [https://www.youtube.com/watch?v=e-2DbkUwKk4&list=PL5ESQNfM5lc7SAMstEu082ivW4BDMvd0U](https://www.youtube.com/watch?v=e-2DbkUwKk4&list=PL5ESQNfM5lc7SAMstEu082ivW4BDMvd0U)
- Bioimaging Guide by [Various People](https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.3002167): https://www.bioimagingguide.org/
- **Bioimage analysis notebook** by Robert Haase: https://haesleinhuepf.github.io/BioImageAnalysisNotebooks

## Pre-requirement of the workshop

Please prepare the following before the workshop:

- Please install [Miniconda](https://www.anaconda.com/download/success#miniconda) on your laptop (Yes, you need a laptop). We will use miniconda to create an environment for coding (i.e. venv)

- Follow the **Creating a Python Environment for the workshop** workflow below for the setup.

- install [Visual Studio Code](https://code.visualstudio.com/download). We will use this as the coding interface (IDE)

## Creating a Python Environment for the workshop

1. Open Anaconda Prompt. 
    - if you are using a **Windows OS machine**, look for **anaconda prompt (miniconda)** in **Start (開始工具列)**. For details, check the step 1 [here](https://kiwi-half.medium.com/python-anaconda-%E8%99%9B%E6%93%AC%E7%92%B0%E5%A2%83%E5%BB%BA%E7%BD%AEanaconda-prompt-virtual-environment-9e93c5789627)
    - if you are using a **Mac OS machine**, look for **terminal (終端機)**. For detailed instruction, check [here](https://support.apple.com/zh-tw/guide/terminal/apd5265185d-f365-44cb-8b09-71a064a42125/mac)


2. With the Anaconda prompt, create a virtual environment with the name “bioimage-analysis”

    ```powershell
    conda create --name bioimage-analysis python=3.11
    ```

3. Then activate the environment

    ```powershell
    conda activate bioimage-analysis
    ```
    
4. Install all the necessary packages

    ```powershell
    conda install numpy matplotlib scipy scikit-image ipywidgets jupyter jupyterlab pandas scikit-learn seaborn
    ```
    then install [Napari](https://napari.org/stable/) with
    ```powershell
    python -m pip install "napari[all]"
    ```