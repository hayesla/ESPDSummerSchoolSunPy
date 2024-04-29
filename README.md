# SunPy tutorial
## ESPD Summer School Apr 2024

<div>
<img src="./images/sunpy_logo.png" width="500" align="left"/>
</div>


This is a reporsitory to hold all the notebooks that will be used in the hands-on session for an introduction to the SunPy project and ecosystem at the European Solar Physics Division (ESPD) [summer school](https://oh.geof.unizg.hr/index.php/en/espd-2024) that takes place in Dubrovnik 29 Apr - 3 May 2024.

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
If you don't want to run these locally, or you are having issues with getting them started - all the notebooks in this repository can be run with binder. Click here [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/hayesla/ESPDSummerSchoolSunPy/HEAD) to launch binder and then run the notebooks in your browser. 

**Note** It may take a few minutes to load up the first time you launch it.

## Run locally


To run these notebooks locally, I'd recommend you follow the next steps. 
The main things here is that you have the necessary packages installed. Mainly, you'll need sunpy 5.1. If you follow below, we set up a virtual env and install the required packages needed for this tutorial, which are listed in the environment.yml file in this repository.

If you don't want to follow the next steps, you can also check out our [sunpy installation page](https://docs.sunpy.org/en/stable/tutorial/installation.html).

#### 1. Download the files using git

If you want to run these notebooks locally you can clone this reposity (or fork it and then clone it from your page). To do this run this command:

- ```git clone https://github.com/hayesla/ESPDSummerSchoolSunPy.git```

If you have first forked it then you can run:

- ```git clone https://github.com/<username>/ESPDSummerSchoolSunPy.git```

You can also download these notebooks by clicking on green `code` button on the top right hand side, and then by clicking download zip. 


#### 2. Create a conda environment

We recommend creating a new conda environment and install the requried packages used in these notebooks.

The python packages required to run these workshop notebooks are listed in the `environment.yml` file in this repository. To create a new environment with these packages installed you can open a terminal and type:

- ```conda env create -f environment.yml```

This will then create a new conda environment called `espd_summer_school` (this name is listed in the `enviroment.yml` file).

You can then activate this environment by typing:

- ```conda activate espd_summer_school```

Note your prompt should change and now have `espd_summer_school` near the start. If you want to list all your conda environments you can type
```conda info -e```. You should see `base` which is your base enviroment, the `espd_summer_school` one, and any others you have created! 


### 3. Start a jupyter notebook!

Once you have your environment activated (remember to first type `conda activate espd_summer_school`) then in your local `ESPDSummerSchoolSunPy` repository type

- ```jupyter lab ```

This should then open the notebooks in your default browser!

If you are having any issues - just make sure first that you are in the `espd_summer_school` environment before you start jupyter.

Happy coding!!


##### 4.1 Updating the environment.yml file
If an update is made to the `environment.yml` file then you will need to type 

- ```conda env update --file environment.yml --prune```

This may be important after you have down a `git pull` (see below 4.)

##### 4.2 Installed new packages in this environment

You can also install new packages in this environment by using `conda install <package>`or by using pip! (`pip install <package>`)

Given by **Laura A. Hayes (ESA/ESTEC)** with many thanks to **Will Barnes (AU/NASA GSFC), Stuart Mumford (Aperio Software), Albert Shih (NASA GSFC), David Stansby (UCL) and the SunPy community**.



