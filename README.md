# PowerBI Conda Environment

Just quick access to a yml file that will create a power bi compatible conda environment for you

## What is this?

When you scour the internet, it was almost impossible to find instructions on how to set up a conda environment for PowerBI. I basically pieced everthing together, posted it on my [blog](https://tengkengvang.com/2023/01/26/using-conda-in-power-bi/) and created this .yml for your convenience.

PowerBI had some weird quirks that make it annoying to work with conda. See the above blog post if you want more detail.

## What problem does this solve?

For whatever reason, PowerBI does not like conda. There are three libraries (pandas, numpy, matplotlib) that need to be installed using pip. I have no idea why, but thats what you need to do to make a conda installation of python work with PowerBI. Why is this important? For a lot of PowerBI users, it probably isn't. However, if you're trying to do any kind of geospatial analysis, meaning you want geopandas, you're probably already thinking conda.

## How do I install this?

Download the yml file and make note of which directory it's in.\
Open your Anaconda prompt and cd into the directory.\
Run `conda env create -f environment.yml`
