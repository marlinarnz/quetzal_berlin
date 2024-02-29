# quetzal_berlin

This aggregated transport model covers the region of Berlin in Planungsraum resolution. It is based on the work of https://github.com/maximylius/quetzal_berlin

It uses the quetzal transport modelling framework: https://github.com/systragroup/quetzal and is based on https://github.com/marlinarnz/quetzal_germany and https://github.com/systragroup/quetzal_paris.

This project was developed for the course Operations Research - Modeling Sustainable Mobility (OR-MSM) at TU Berlin.


## Getting started

1. Create a virtual environment for quetzal models: Clone the quetzal package into a local folder and create a virtual environment as described here *[1]*: https://github.com/systragroup/quetzal
2. Activate your quetzal environment, if not done yet
3. Clone this repository into a local folder: In your terminal, navigate to the position where you want to store the code. Type `git clone <this repo's URL>`. Navigate into the folder `quetzal_berlin`.
5. Open the notebooks folder in Jupyter Notebook (in your terminal, navigate to `notebooks` using `cd` command, then type `jupyter notebook`) and start running the notebooks
6. For your first run, execute `04_OD-LoS-stack` once from top to bottom (not required afterwards)
7. Run scenarios as you please in `05_Simulation` and visualise the results against each other in `val_scenarios`

You can test your virtual environment by running the `00_environment_test` notebook.

*[1]*: If you face problems importing geopandas, consider uninstalling package `rtree` and reinstalling a version up to 0.9.3 (`conda install -c conda-forge rtree=0.9.3`) or uninstalling the whole environment and reinstalling it with the requirements file posted in this [issue](https://github.com/systragroup/quetzal/issues/45). If you have problems with `numba` or others, consider fetching an earlier, more stable, version of `quetzal` with this commit: `git checkout 1126c05c8366e871893b85a55bd57d9d20e7d1d0`
