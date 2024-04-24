# NextGen Forcings Engine Repository Overview
Welcome to the NextGen Forcings Engine GitHub repository. This repository currently contains Python tools that allows the NextGen Water Resources Modeling Framework to be provide meteorological forcings data to NextGen formulations through either (1) csv catchment/netcdf files or (2) a Basic Model Interface (BMI) Forcings Engine. This repository also contains Forcings Extraction script repository that will allow a given user to extract all meteorological forcing data products required for National Water Model (NWM) version 3.0 operational configurations. Future endeavors for this repository will also evenetually provide users more Python tools that will implement various data assimilation techniques (dyanmic data, oceanic/freshwater circuluation models) for NextGen formulations within the framework. 

# NextGen Lumped Forcings Driver Directory
This directory contains Python modules and a driver script that will provide users lumped meteorological forcings for catchments within the NextGen hydrofabric. Users will be able to create NextGen formatted csv catchment files or a single netcdf file that can be ingested by the default NextGen Forcings Provider. Current Python modules can support Analaysis of Record and Calibration (AORC) data, GFS data, CFS data, and HRRR data products that are needed for standard NWM operational configurations (Reanlysis, Analysis and Assimilation, Short range, Medium range, and long range). Setup, installation, and examples of utilizing these Python tools are further described within The ReadMe.md file in the directory as well as it's own Wiki Pages subsection. 

# NextGen Forcings Engine BMI Directory
This directory contains a BMI application that essentially streamlines the WRF-Hydro Forcings Engine into a BMI compliant data pipeline with universal regridding capabilites. This Python BMI tool can directly provide the NextGen model engine regridded meteorological forcings that are required for all NWMv3.0 operational configurations. BMI realization configuration files have already been constructed for all NWMv3.0 operational configurations to support gridded domains, unstructured meshes, and the NextGen hydrofabric. Setup, installation, and examples of utilizing these Python tools are further described within The ReadMe.md file in the directory as well as it's own Wiki Pages subsection. 

# Forcing Extraction Scripts Directory
This directory contains a series of scripts for each NWM domain subdirectory (CONUS, Alaska, Puerto Rico, Hawaii) that encompasses the required meteorological forcing data products needed for each regional NWMv3.0 operational configuration setup. Each script is a particular meteorlogical forcing data product that is available to download off the NOMADS server. Availability of each meteorlogical forcing data product varies, but a user can generally extract at least the last 24 hours of previous data products or forecast cycles available. Setup, installation, and examples of utilizing these Python tools are further described within The ReadMe.md file in the directory as well as it's own Wiki Pages subsection. 

