# Containers

Docker containers to run RSES data stacks. The containers need the pre-installation of Docker, see https://docs.docker.com/.

## Swiss-Toll Python-R-Julia for data science

* The Jupyter data science container (https://github.com/jupyter/docker-stacks/tree/master/datascience-notebook) provides some fundamental Python and R packages to perform some data science tasks in those languages with using the Jupyter notebooks.

	To get the container:
	
		docker pull jupyter/datascience-notebook
		
	To run the container:
	
		docker run -it --rm -p 8888:8888 -v /my_path/:/home/jovyan/work jupyter/datascience-notebook

	Be carefull to replace /mypath by your current working path.
	
## Julia

* The charlesll/julia:latest container (https://github.com/charlesll/Docker-Julia) offers a lot of julia libraries as well as pre-installed Python 2 and Python 3 kernels with machine learning librairies, accessible through Jupyter notebooks.

	To get the container:
	
		docker pull charlesll/julia:latest
		
	To run the container:
	
		docker run -it --rm -p 8888:8888 -v /my_path/:/home/jovyan/work charlesll/julia:latest
		
	Be carefull to replace /mypath by your current working path.


