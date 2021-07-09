<p align="center">
  <h3 align="center">Feature Selection using Genetic Algorithm</h3>
  </p>
</p>


<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
        <li><a href="#about-datasets">About Datasets</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
      </ul>
    </li>
    <li><a href="#results">Results</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

This is a thesis project submitted to the Faculty of Engineering and Natural Sciences by Ece Akcicek in partial fulfillment of the requirements for the Bachelor of Science in the Department of Computer Engineering.

Datasets with high dimensions can harm the efficiency by increasing com- plexity and computational cost. To avoid that, an evalutionary Genetic Algorithm is developed to be used in Feature Selection process with the help of Logistic Regression, Relevance and enhanced Genetic Algorithm functions. 

There are 5 important steps of that followed through iterations in this study:

1. Selection: To put a selection pressure on the system and to individuals, **_Tournament Selection_** is used to select the parents of the next generation. 

2. Cross-over: In every iterations, two types of crossovers are made. 
To increase diversity, **_two-point cross-over_** is implemented. 
To increase the fitness faster through generations, a custom cross-over method is developed called **_min-max cross-over_**. This method generates an offspring using the least and the most fit individuals, and replacing it with the least fit parent.

3. Mutation: With a low probability, given as 0.2, **_scrambled mutation_** is applied to the 20 percent of the population.

4. Feature Relevance: This attribute of Logistic Regression can show the relevance of the features to each other, which can help determine feature pairs or multiple features that carry information together, and also relevant to label class.

5. Fitness: Fitness function is the decider of the algorithm. With Logistic Regression, accuracy is calculated. To increase the selection pressure, fitness is calculated as accuracy over square root of number of features selected.

### Built With
**Python** is used to build this algorithm...
* [Python](https://www.python.org)

...with the help of libraries such as **pandas, NumPy, Scikit-Learn**.
* [Scikit-Learn](https://scikit-learn.org/stable/)
* [Numpy](https://numpy.org)
* [Pandas](https://pandas.pydata.org)

### About Datasets

5 of different artificial databases are used. These datasets vary on difficulty on classification. To be able to see the efficiency of the proposed FS method on real datasets, 2 more large datasets taken from UCI ML Repository is used.
* Telugu Vowel Dataset (TVD)
* Parkinson’s Disease Dataset (PDD)

     instnc   attr    #of classes
TVD   120     785     6
PDD   756     755     2  
AD1   1000    201     2
AD2   1000    201     5
AD3   1000    1001    3
AD4   1000    201     5
AD5   100     201     3

<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

* [Download and install Python](https://www.python.org/downloads/)

And thats all!

<!-- Results -->
## Results
After tests, it is seen that selected number of features is <20 in most cases, and accuracy is > %70.
In the best case of TVD, 4 features are selected with %99.4 accuracy.
In the best case of PDD, 12 features are selected with %84.5 accuracy.

<!-- CONTACT -->
## Contact

Please contact if you have any questions or encounter any error/bug!
Ece Akcicek - eceakcck@gmail.com
