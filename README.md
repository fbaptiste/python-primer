# python-primer
Short Python primer for devs with experience in another language (such as Java) looking to quickly get up to speed with the basics of Python.

## Setting things up

* Install Python 3.9.x using the official canonical Python [web site ](https://www.python.org/)
* Clone this github repo at some preferred location on your system.
* `cd` into the cloned project
* Create a virtual Python environment (in this case named `.venv`:

	```bash
	python3.9 -m venv .venv
	
	```

* Activate the environment (you'll have to do this step every time you come back to work on this project) - this basically tells you shell which Python to use - in this this case the one located in `.venv`:

	```bash
	source .venv/bin/activate
	```
	
* The first time only, you'll need to install various 3rd party packages we'll use in this project:
 
	```bash
	pip install -r requirements.txt
	```


## Running Jupyter Notebook

Once the above steps are completed, you can run Jupyter Notebook locally (remember to activate the `.venv` Python environment before doing so):

```bash
jupyter notebook .
```

This will open up Jupyter Notebook in your default browser. Simply select a notebook you want to view/edit (or create a new one) from this interface. 

Each Jupyter notebook is essentially a front-end to the Python interactive prompt (the so-called REPL - which stands for Read-Evaluate-Print-Loop). Remember that Python is essentially an interpreted language, so you can run commands one at a time via this REPL, still maintaining state from previous issue commands in the same session. And Jupyter is a graphical layer on top of that. 

You could use the plain Python REPL by typing `python` at the command line (after activating the virtual environment) and get a text-based REPL. 

Jupyter is nicer because it remembers your code (as long as you save it), you can add non code blocks (using Markdown for example), and you can easily run previous commands by selecting the cell and running it. Amongst other things...
