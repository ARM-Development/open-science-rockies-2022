# Open Science in the Rockies - AMS Short Course 2023

[![badge](https://img.shields.io/static/v1.svg?logo=Jupyter&label=ARM+JupyterHub&message=ACE+Environment&color=blue)](https://jupyterhub.arm.gov/hub/user-redirect/git-pull?repo=https%3A//github.com/ARM-Development/open-science-rockies-2022&urlpath=lab/tree/open-science-rockies-2022/notebooks&branch=main)

This repository hosts content related to the AMS 2023 Short Course: Open Science in the Rockies: Working With ARM Data from the Surface Atmosphere Integrated Field Laboratory

* [AMS Landing Page](https://www.ametsoc.org/index.cfm/ams/education-careers/careers/professional-development/short-courses1/open-science-in-the-rockies-working-with-arm-data-from-the-surface-atmosphere-integrated-field-laboratory/)

## Motivation

Open Science in the Rockies: Working With ARM Measurements from the Surface Atmosphere Integrated Field Laboratory. The water resources of the western United States are changing rapidly, and how the atmosphere respond. The ARM Mobile Facility (AMF) is nearing the end of a nearly two year deployment to Crested Butte, Colorado. The Surface Atmosphere Integrated Field Laboratory (SAIL) deployment involved a myriad of measurements documenting the earth system processes, extending from stratosphere through the bedrock, which control water resources in the West. This short course, aimed at a broad audience, will:

- Introduce students to the unique capabilities of the ARM program and the community of atmospheric scientists that use and produce ARM data.
- Educate attendees on ARM’s measurement suite.
- Highlight the underlying science behind SAIL and the East River watershed.
- Show how to find and access ARM measurements.
- Using a number of open source tools, train attendees how to analyze ARM’s open data in the Python programming language.


## Authors

[Dr. Daniel Feldman](@drfeldman), [Max Grover](@mgrover1), [Dr. Scott Collis](@scollis), [Dr. Monica Ihli](@monicaihli)

### Contributors

<a href="https://github.com/ARM-Development/open-science-rockies/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=ARM-Development/open-science-rockies" />
</a>

## Course program (All times in Mountain Time)
* 08:00 - 08:15 Welcome and getting started (Max Grover)
* 08:15 - 08:30 An Overview of ARM (Dr. Scott Collis)
* 08:30 - 09:00 SAIL Field Campaign Overview (Dr. Dan Feldman)
* 09:00 - 09:15 Ice Breaker! (Dr. Dan Feldman)
* 09:15 - 09:45 Accessing ARM Data + Compute (Dr. Monica Ilhi)
* 09:45 - 10:00 Break!
* 10:00 - 10:50 Radar Data with Py-ART (Max Grover)
* 11:00 - 11:50 Surface Observations with ACT (Joe O’Brien)
* 11:50 - 13:00 Lunch
* 13:00 - 13:50 Working with Aerosol Measurements (Dr. Allison Aiken)
* 14:00 - 14:50 Advanced Xarray + Visualization (Max Grover)
* 15:00 - 15:30 How to Contribute to Open Science (Dr. Scott Collis)
* 15:30 - 15:45 Closing (Dr. Dan Feldman)

## Getting Started

### Register for Access to the Tutorial Platform

Participants who do not already have one should first register for an ARM account. When filling out the form, indicate that you are affiliated with the particular workshop or course (AMS Open Science in the Rockies):

![ARM user registration screenshot](notebooks/images/arm-registration-instructions.png)

If you already have an ARM account, email clustersupport@arm.gov that you need to be granted access to the workshop or course materials.

### Investigate Tutorial Materials and Follow Prerequisites

The tutorial materials are available online (https://arm-development.github.io/open-science-rockies-2022), and we encourage participants to investigate the materials before attending the workshop. For example, in one of the first examples (the radar example), we encourage participants to investigate the prerequisites, and ensure they are familiar with the material. While this is not required for participants, it is highly encouraged.

![Example tutorial material](notebooks/images/arm-tutorial-screenshot.png)

## Structure

### Radar Data with Py-ART
Within this section, we cover the basics of Py-ART and apply it to a sample analysis workflow.

### Weather Observations with ACT
The Atmospheric data Community Toolkit (ACT) is a helpful tool when working with atmospheric observations! This portion will focus on reading, visualizing, and analyzing observational datasets from the Atmospheric Radiation Measurement user facility.

### Xarray and Pangeo
Our last section covers how to use the Pangeo stack, Xarray and other components to inspect and visualize earth system model data.

## Running the Notebooks
You can either run the notebook using [Binder](https://mybinder.org/) or on your local machine.

### Running on Jupyter

The simplest way to interact with a Jupyter Notebook is through the
[ARM Jupyter](https://jupyterhub.arm.gov), which enables the execution of a
[Jupyter Book](https://jupyterbook.org) on ARM infrastructure. The details of how this works are not
important for now. Navigate your mouse to
the top right corner of the book chapter you are viewing and click
on the rocket ship icon, (see figure below), and be sure to select
“launch Jupyterhub”. After a moment you should be presented with a
notebook that you can interact with. I.e. you’ll be able to execute
and even change the example programs. You’ll see that the code cells
have no output at first, until you execute them by pressing
{kbd}`Shift`\+{kbd}`Enter`. Complete details on how to interact with
a live Jupyter notebook are described in [Getting Started with
Jupyter](https://foundations.projectpythia.org/foundations/getting-started-jupyter.html).

### Running on Your Own Machine
If you are interested in running this material locally on your computer, you will need to follow this workflow:

(Replace "arm-cookbook-example" with the title of your cookbooks)   

1. Clone the `https://github.com/ARM-Development/open-science-rockies-2022` repository:

   ```bash
    git clone https://github.com/ARM-Development/open-science-rockies-2022
    ```  
1. Move into the `open-science-rockies-2022` directory
    ```bash
    cd open-science-rockies-2022
    ```  
1. Create and activate your conda environment from the `environment.yml` file
    ```bash
    conda env create -f environment.yml
    conda activate open-science-rockies-2022-dev
    ```  
1.  Move into the `notebooks` directory and start up Jupyterlab
    ```bash
    cd notebooks/
    jupyter lab
    ```
