## Install
You need python 3 (tested with 3.6). Follow these steps to create a new python virtual environment and install the dependencies:

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --upgrade pip setuptools
pip install -r requirements
```

After that you should be able to run the `analysis.py` script:

```bash
python -m analysis
```


## Working with Jupyter Notebooks on VSCode

The main analysis file is using the mixed VSCode / Jupyter syntax. You can run it as a normal python script, but you can also execute cell by cell and see the inmediate output _a la jupyter_ just within your code editor. Read more about it here: https://code.visualstudio.com/docs/python/jupyter-support

Following these steps has advantage of allowing you to control which python version and which versions of libraries are available (specified on `requirements.txt`), instead of just running whatever python VSCode happens to find installed and not knowing which libraries or versions are available.

1. Start a Jupyter server on your console

    ```bash
    source .venv/bin/activate
    jupyter notebook
    ```

2. Check the url with the token that appears after starting the notebook server, looks like this

    ```
    http://localhost:8889/?token=bb3f6b9906d0e3d4c16ccf4fae862d795d908a0dbf75b3b6
    ```


3. On VSCode run the command (`cmd` + `shift` + `p`) called `Python: specify jupyter server URI` and paste the address of your notebook

4. Open the python file with the code and run the first cell
