# Python Basics Jupyter Notebooks

Python labs for the Swiss German Videos on [Youtube](https://www.youtube.com/playlist?list=PLRANZYigacWIDKePwwsmYykytkw5_M_OU).
Partitioning is mostly congruent with the book [Automate the Boring Stuff](https://automatetheboringstuff.com/) and can be used as a supplement.


## Run locally with VS Code

Running notebooks in VS Code is easy and fun. Just install the Microsoft Python extension.

https://code.visualstudio.com/docs/datascience/jupyter-notebooks


## Run locally with Docker

Just run the following script within the folder of the readme. You need to have Docker installed.

```bash
docker run -ti --rm \
  -p 8888:8888 \
  -e JUPYTER_ENABLE_LAB=yes \
  -v "$PWD":/home/jovyan/work \
  jupyter/minimal-notebook
```

Then, visit the website shown in the terminal output.


## Run locally in a virtual Python environment

Just run the following script within the folder of the readme. You need to have Python3 installed.

```bash
python -m venv .venv
source .venv/bin/activate
pip install notebook
jupyter notebook
```

Then, visit the website shown in the terminal output.
