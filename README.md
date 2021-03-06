# Machine Learning Engineer Nanodegree
## Introduction and Foundations
## Project: Titanic Survival Exploration

My implementation of the project and the result click [here](#results-of-the-project)

### Install

This project requires **Python 2.7** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. Make sure that you select the Python 2.7 installer and not the Python 3.x installer.

### Code

Template code is provided in the notebook `titanic_survival_exploration.ipynb` notebook file. Additional supporting code can be found in `visuals.py`. While some code has already been implemented to get you started, you will need to implement additional functionality when requested to successfully complete the project. Note that the code included in `visuals.py` is meant to be used out-of-the-box and not intended for students to manipulate. If you are interested in how the visualizations are created in the notebook, please feel free to explore this Python file.

### Run

In a terminal or command window, navigate to the top-level project directory `titanic_survival_exploration/` (that contains this README) and run one of the following commands:

```bash
jupyter notebook titanic_survival_exploration.ipynb
```
or
```bash
ipython notebook titanic_survival_exploration.ipynb
```

This will open the Jupyter Notebook software and project file in your web browser.

### Data

The dataset used in this project is included as `titanic_data.csv`. This dataset is provided by Udacity and contains the following attributes:

**Features**
- `pclass` : Passenger Class (1 = 1st; 2 = 2nd; 3 = 3rd)
- `name` : Name
- `sex` : Sex
- `age` : Age
- `sibsp` : Number of Siblings/Spouses Aboard
- `parch` : Number of Parents/Children Aboard
- `ticket` : Ticket Number
- `fare` : Passenger Fare
- `cabin` : Cabin
- `embarked` : Port of Embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)

**Target Variable**
- `survival` : Survival (0 = No; 1 = Yes)

### Results of the Project

My implementation of the project can be seen at Result.html file.

#### How to view results

1. Download or clone the repo
2. Open the Results.html file on your browser

### Comments about implementation

We know that Titanic lost most of its passengers during the incident. Using my knowledge of the event and bias from the Titanic movie. I deduct the following conclusions:
1. Women and children first.
2. Lower class passenger had little chance of surviving.
3. I assume parent will sacrifice herself during that tragic event, If she has any children.

Using filters like Pclass, we can see that most of the upper class survived. After that priority of survival depend on the sex of the passenger.
If a passenger was a female, she is most likely to survive in the incident expect females at lower class cabins.
I assume that females  who have at least one child (which I use Parch filter to see that survival rate) located in lower class cabins, they did not survive.
I apply all the variables that I mentioned above to get a 80% prediction rate.
