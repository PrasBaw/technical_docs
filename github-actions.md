# Github Actions
- Feature in Github to create Automated workflows.
- Automate SDLC workflows (Coding, build, deploy, testing, Release)
- Implement CI CD Devops

**Terms in Github Actions:**
1) Workflow
2) Events
3) Jobs
4) Steps

**Workflow Example:**
---
	name: hello-world
	on: push
	jobs:
	  my-job:
	    runs-on: ubuntu-latest
	    steps:
	      - name: my-step
	        run: echo "Hello World!"
---
1) **Workflow:** collection of jobs, defined in a YAML file
	name: Name of the owrkflow
2)  **EVENTS:**, any activity in the repo that can trigger a workflow. ex: (on: push)
3)   **Jobs:** Collection of steps
4)   **Steps**: Actions to be taken, commands, scripts
