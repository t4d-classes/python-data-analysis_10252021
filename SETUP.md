
# Setup Demo

## Standard Python

1. Create and Activate Virtual Environment

```bash
mkdir my_project

cd my_project

python -m venv venv

#source ./venv/bin/activate
venv\Scripts\Activate.ps1
```

2. Upgrade Pip

```bash
python -m pip install --upgrade pip
```

3. Install Jupyter Lab

```bash
python -m pip install jupyterlab numpy pandas matplotlib
```

4. Install a new kernel.

```bash
ipython kernel install --name my_project
```

More info: [https://github.com/jupyter/jupyter/wiki/Jupyter-kernels](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels)


5. Run Jupyter Lab

```bash
jupyter-lab
```

6. Install additional packages in virtual environment through Jupyter Notebook.

```jupyter
import sys
!{sys.executable} -m pip install --upgrade pip
!{sys.executable} -m pip install numpy
```

7. Deactivate virtual environment.

```bash
deactivate
```

## Anaconda Python

1. Download and install Anaconda: [https://www.anaconda.com/products/individual](https://www.anaconda.com/products/individual)

2. Open the Anaconda Python terminal and update Conda.

```bash
conda update conda
```

2. Create and activate Conda Environment
con
```bash
mkdir my_project

cd my_project

conda create -n my_project

conda activate my_project
```

3. Install Jupyter Lab and other packages.

```bash
conda install -c conda-forge jupyterlab numpy pandas matplotlib
```

4. Run Jupyter Lab

```bash
jupyter-lab
```

Note: if you get the error "ImportError: DLL load failed while importing win32api: The specified procedure could not be found."

Run this command, then try to start Jupyter Lab again.

```bash
conda install pywin32 jupyter_client
```

5. Install packages with Conda via a Jupyter Notebook

```bash
import sys
!conda install --yes --prefix {sys.prefix} numpy
```

6. Install a new kernel.

```bash
ipython kernel install --name my_project
```

More info: [https://github.com/jupyter/jupyter/wiki/Jupyter-kernels](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels)

7. Deactivate Conda environment.

```bash
conda deactivate
```

## Anaconda Python Menu Item

1. Click the "Jupyter Notebook" link under the Anaconda Menu

2. Navigate to the notebook to run.

## Visual Studio Code

1. Install Microsoft's Python extension.

2. Open the existing folder and click on a notebook to run. Select the kernel. Run the notebook.







