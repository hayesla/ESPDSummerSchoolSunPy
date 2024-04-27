# SunPy tutorial
## ESPD Summer School Apr 2024

<div>
<img src="./images/sunpy_logo.png" width="500" align="left"/>
</div>


This is a reporsitory to hold all the notebooks that will be used in the hands-on session for an introduction to the SunPy project and ecosystem at the [European ](1st European solar physics division) that takes place in Dubrovnik 29 Apr - 3 May 2024.

-----------------------------------
## Resources

Below are a few helpful links for finding out more about SunPy, including our webpage, documentation, and our Matrix channel:

* [sunpy.org](https://sunpy.org/)
* [SunPy Documentation](https://docs.sunpy.org/en/stable/)
* [List of Affiliated Packages](https://sunpy.org/project/affiliated.html)
* [Matrix Chat](https://openastronomy.element.io/#/room/#sunpy:openastronomy.org)
* [OpenAstronomy Discourse](https://community.openastronomy.org/c/sunpy/5)


# How to run these notebooks:
===========================================


## Run in Binder
If you don't want to run these locally, or you are having issues with getting them started - all the notebooks in this repository can be run with binder. Click here [![Binder](https://mybinder.org/badge_logo.svg)](
https://mybinder.org/v2/gh/hayesla/solarorbiter-summerschool-sunpy/HEAD) to launch binder and then run the notebooks in your browser. 

**Note** It may take a few minutes to load up the first time you launch it.

## Run locally

Here are the steps you'll need to run:

#### 1. Download the files using git

If you want to run these notebooks locally you can clone this reposity (or fork it and then clone it from your page). To do this run this command:

- ```git clone https://github.com/hayesla/ESPDSummerSchoolSunPy.git```

If you have first forked it then you can run:

- ```git clone https://github.com/<username>/ESPDSummerSchoolSunPy.git```

You can also download these notebooks by clicking on green `code` button on the top right hand side, and then by clicking download zip. 


#### 2. Create a conda environment

We recommend creating a new conda environment and install the requried packages used in these notebooks. [Here](https://towardsdatascience.com/getting-started-with-python-environments-using-conda-32e9f2779307) is a nice introduction to anaconda environments for those new to the concept, and [here](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf) is a conda cheatsheet which may help too! 

The python packages required to run these workshop notebooks are listed in the `environment.yml` file in this repository. To create a new environment with these packages installed you can open a terminal and type:

- ```conda env create -f environment.yml```

This will then create a new conda environment called `sunpy-tutorial` (this name is listed in the `enviroment.yml` file).

You can then activate this environment by typing:

- ```conda activate sunpy-tutorial```

Note your prompt should change and now have `sunpy-tutorial` near the start. If you want to list all your conda environments you can type
``` conda info -e```. You should see `base` which is your base enviroment, the `sunpy-tutorial` one, and any others you have created! 

##### 2.2 Updating the environment.yml file
If an update is made to the `environment.yml` file then you will need to type 

- ```conda env update --file environment.yml --prune```

This may be important after you have down a `git pull` (see below 4.)

##### 2.3 Installed new packages in this environment

You can also install new packages in this environment by using `conda install <package>`or by using pip! (`pip install <package<`)

### 3. Start a jupyter notebook!

Once you have your environment activated (remember to first type `conda activate sunpy-tutorial`) then in your local `ESPDSummerSchoolSunPy` repository type

- ```jupyter lab ```

This should then open the notebooks in your default browser!

If you are having any issues - just make sure first that you are in the `sunpy-tutorial` environment before you start jupyter.

Happy coding!!

Given by **Laura A. Hayes (ESA/ESTEC)** with many thanks to **Will Barnes (AU/NASA GSFC), Stuart Mumford (Aperio Software), Albert Shih (NASA GSFC), David Stansby (UCL) and the SunPy community**.



