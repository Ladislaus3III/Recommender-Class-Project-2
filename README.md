# Recommender Class Project 2

### **Project description**
 This project is recommender based on recommenders included in classes. 
 
 The goal was to train recommender and achieve the best score and compare it to Amazon recommender and Netflix recommender.

 Recommenders use data from real hotel company.

 Project contains 2 the most important files: 
-  project_1_data_preparation.ipynb
-  project_2_recommender_and_evaluation.ipynb

 Other files are important to properly run everything.

 ### **Necessery libraries for this project to run:**
 - numpy
 - pandas
 - matplotlib
 - seaborn
 - sklearn
 - hyperopt
 - traceback
 - torch
 - livelossplot

 To install libraries mentioned above use:

    pip install <name_of_package>

 **You also need program to open .ipynb files.**
 
 Recommended is [Visual Studio Code](https://code.visualstudio.com/download) with Python 3.8.

 ### **Description of key parts of project**

1. project_1_data_preparation.ipynb:
    
    This notebook contains several methods to prepare data for recommender.

    It uses functions stored in **data_preprocessing\data_preprocessing_toolkit.py** to achieve final results for data.

    **This is important to run this notebook before project_2_recommender_and_evaluation.ipynb!**

2. project_2_recommender_and_evaluation.ipynb:

    This notebook contains methods to prepare user features and item features for recommender. 

    It also contains neural model used in project.

    **It uses processed data from project_1_data_preparation.ipynb**

    This file defines how recommender work. 
    
    It trains recommender to achieve the best final score and compare different recommender types.

### **Final results**

 Effectiveness of recommenders was verified by algorithms stored in **evaluation_and_testing/evaluation_measures.py** and  **evaluation_and_testing/testing.py**.

 For recommender presented in this project results are:

![My recommender](img/my.jpg)

For Amazon recommender results are:

![Amazon recommender](img/amazon.jpg)

For Netflix recommender results are:

![Netflix recommender](img/netflix.jpg)

So for all recommenders resluts are:

![Both recommenders](img/all.jpg)

### **Other things and thoughts**

1. I tried changing model and forward function but without good changes. This model also make **tuning function** don't work and crash PC.
I tried tuning manually but without heavy changes.

2. I created "ratings" for users but they are not that good they should.

3. I assume that created model is not appropriate for this problem and should be created again but time didn't allow to do it.