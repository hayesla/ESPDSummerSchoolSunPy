# SunPy tutorial
## Solar Orbiter Summer School 2022
Given by **Laura A. Hayes (ESA/ESTEC)** with many thanks to **Will Barnes (AU/NASA GSFC), Stuart Mumford (Aperio Software), Albert Shih (NASA GSFC), David Stansby (UCL) and the SunPy community**.

<div>
<img src="./images/sunpy_logo.png" width="500" align="left"/>
</div>


This is a reporsitory to hold all the notebooks that will be used in the hands-on session for an introduction to the SunPy project and ecosystem at the [Solar Orbiter summer school](https://solarorbiter.sciencesconf.org) that takes place in Sète 30 May - 3 June 2022.

These notebooks are heavily based on other tutorials such as the [AAS/SPD meeting](https://github.com/sunpy/aas-2021-workshop) and those at the [Python in Heliophysics Summer School](https://github.com/heliophysicsPy/summer-school).  


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

- ```git clone  https://github.com/hayesla/solarorbiter-summerschool-sunpy```

If you have first forked it then you can run:

- ```git clone  https://github.com/<username>/solarorbiter-summerschool-sunpy```

You can also download these notebooks by clicking on green `code` button on the top right hand side, and then by clicking download zip. 


#### 2. Create a conda environment

We recommend creating a new conda environment and install the requried packages used in these notebooks. [Here](https://towardsdatascience.com/getting-started-with-python-environments-using-conda-32e9f2779307) is a nice introduction to anaconda environments for those new to the concept, and [here](https://docs.conda.io/projects/conda/en/4.6.0/_downloads/52a95608c49671267e40c689e0bc00ca/conda-cheatsheet.pdf) is a conda cheatsheet which may help too! 

The python packages required to run these workshop notebooks are listed in the `environment.yml` file in this repository. To create a new environment with these packages installed you can open a terminal and type:

- ```conda env create -f environment.yml```

This will then create a new conda environment called `sunpy-tutorial` (this name is listed in the `enviroment.yml` file).

You can then activate this environment by typing:

- ``` conda activate sunpy-tutorial```

Note your prompt should change and now have `sunpy-tutorial` near the start. If you want to list all your conda environments you can type
``` conda info -e```. You should see `base` which is your base enviroment, the `sunpy-tutorial` one, and any others you have created! 

##### 2.2 Updating the environment.yml file
If an update is made to the `environment.yml` file then you will need to type 

- ```conda env update --file environment.yml --prune```

This may be important after you have down a `git pull` (see below 4.)

##### 2.3 Installed new packages in this environment

You can also install new packages in this environment by using `conda install <package>`or by using pip! (`pip install <package<`)

### 3. Start a jupyter notebook!

Once you have your environment activated (remember to first type `sunpy-tutorial`) then in your local `solarorbiter-summerschool-sunpy` repository type

- ```jupyter notebook ```

This should then open the notebooks in your default browser!

If you are having any issues - just make sure first that you are in the `sunpy-tutorial` environment before you start jupyter.

Happy coding!!


#### 4. Pulling the most up-to-date version
Throughout the workshop, these notebooks were updated and further notebooks were added. To make sure that your local repository reflects whats currently here you will need to run a `git pull`. This will pull the most up-to-date version of this repository. Before you do this however, you will want to check which remote you have linked to this repository. To find out this you can type this in your local `solarorbiter-summerschool-sunpy` repository:

- ```git remote -v``` 

and this will list the current remotes
It might looks something like this

```
origin	https://github.com/<username>/solarorbiter-summerschool-sunpy (fetch)
origin	https://github.com/<username>/solarorbiter-summerschool-sunpy (push)
upstream	https://github.com/hayesla/solarorbiter-summerschool-sunpy (fetch)
upstream	https://github.com/hayesla/solarorbiter-summerschool-sunpy (push)
```

what you will want to do is pull the main branch from the one that is linked to `https://github.com/hayesla/solarorbiter-summerschool-sunpy` - which in this example is `upstream`. Hence to pull the latest version of this repository you would type:

- `git pull upstream main` 

and this will update your local files. 

Otherwise if when you typed `git remote -v` and it looks like
```
origin	https://github.com/hayesla/solarorbiter-summerschool-sunpy (fetch)
origin	https://github.com/hayesla/solarorbiter-summerschool-sunpy  (push)
```
then you would type

- ``` git pull origin main```

to update your local files. 




