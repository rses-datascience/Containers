# Containers

Docker containers to run RSES data stacks. The containers need the pre-installation of Docker, see https://docs.docker.com/.

## Julia

* The charlesll:julia:latest container offers a lot of julia libraries as well as pre-installed Python 2 and Python 3 kernels, accessible through Jupyter notebooks.

	To get the container:
	
		docker pull charlesll/julia:latest
		
	To run the container:
	
		docker run -it --rm -p 8888:8888 -v /my_path/:/home/jovyan/work charlesll/julia:latest
		
	Be carefull to replace /mypath by your current working path.