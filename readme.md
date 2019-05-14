# The Turron Experiment
Repo with the data and the analysis code

## Install
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install --update pip setuptools
pip install -r requirements
```

## Working with Jupyter Notebooks on VSCode

The advantage of this system is that it allows you to control which python version and which versions of libraries are available (specified on `requirements.txt`), instead of just running whatever python VSCode happens to find installed and not knowing which libraries or versions are available.

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


# TODO:
- [x] Hours: see if there is any correlation between score/type of turron and the numbers of hours since people last eat
- [x] Delta: calculate the difference between turron A and B (delta) to see differences (maybe plot this bar charts that go up/down or left/right)
- [x] calculate all the paired tests
- [x] Contradiccion: look for patterns were people liked better A but thought B was the expensive one (or viceversa)
- [x] analyse gender by turron interaction
- [x] structure report
- cleanup
    - [] one melted to rule them all
    - [] group analysis by theme
- writting report
    - Alex:
        - [] results
        - [] conclussions
    - Eva:
        - [] Intro
        - [] Experimental design
