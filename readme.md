# The Turron Experiment
The Turron Experiment was a fun exercise conducted by [Eva Benito]() and [Alejandro Riera](http://github.com/ariera/) in 2019.

The main purpose was to learn (mainly Eva teaching Alex) things like experiment design, data collection, statistical analysis, reporting, and tools such as pandas, matplotlib, seaborn, etc...

To do that, we conducted a turrón tasting experiment with the collaboration of EMBO staff. We asked participants to taste 2 turrón varieties, one that was expensive and one that was cheap. They didn't know which one was which, but they had to score it and guess.

## What is it turrón?

It is a typical spanish christmas sweet. Today comes in many different variations with all sort of ingredients, but the traditional one is made of almond and honey, in a shape and look similar to nougat in other countries.

For this experiment we chose the _soft_ version, called _Jijona_ variety, in which the almonds are reduced to a delicious paste.


## The study

In this respository, you can find:

* [The final report of our work](report.md)
* [Along with the source data collected](data.csv)
* [And our script to analyse it](analysis.py)

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
    - [x] one melted to rule them all
    - [x] group analysis by theme
- writting report
    - Alex:
        - [ ] results
        - [ ] conclussions
    - Eva:
        - [ ] Intro
        - [ ] Experimental design
- [ ] make better use of color to help differentiatie turron (a vs b) and gender (male vs female)
- [ ] delete excel fil and keep just csv
- [ ] remove emails from csv
- [x] remove sweetness from all analysis and graphs
- [x] ask annika about cake&learn