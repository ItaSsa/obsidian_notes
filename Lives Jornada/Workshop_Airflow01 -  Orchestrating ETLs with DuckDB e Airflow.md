1. Create a github repository
2. Create a local folder
3. Open Vscode and link local folder to repository
4. Check the python version , maybe airflow have python version restrictions
		`pyenv local 3.11.5` [[pyenv_instaltion]]
5. Config poetry
	1. Initializes
		`poetry init` [[poetry_configuration]]
	2. Set a virtual environment
		`poetry env use 3.11.5`
	3. `poetry shell`
6. `touch .gitignore`
			.venv
7. `git add .` and `git commit -m "first commit"` and `git push`
8. poetry add apache-airflow	
		***Why can't you install Airflow just by using 'pip install'*** 
				Because Airflow is not just a simple libray; it is an architecture for workflow orchestration.
				With many components: Scheduler, log, webserver.
				It needs a infrastructure.
		***Why can't you install airflow just with docker image?***
				Because even with the docker image I have to do the database , scheduler and webservice configuration.
		***What is Astro?***
				Astro is Docker + configuiration!
9. [Astronomer](https://www.astronomer.io/) X [Astro CLI](https://www.astronomer.io/docs/astro/cli/develop-project)
	[[Install  and run Astro CLI]] Astro
	1. create an Astro project  
			`astro dev init`
	2. Run astro
			`astro dev start`
	3. 
10. 