# waifu-net
*Presented by:*

Jahel S.León R. (jleonro@unal.edu.co)* <br>
Juan C. Mora P. (jumorap@unal.edu.co)* \\
---
***NOTE:** BECAUSE OF THE SIZE OF THE DATA, IF YOU WANT TO REPRODUCE THE FULL EXPERMIENT BY YOUR OWN PLEASE GO TO THE FOLOWING KAGLE NOTEBOOK https://www.kaggle.com/jahelsantiagoleon/waifu-net. BUT IF YOU WANT TO UNDERSTAND THE FULL PROCESS, PLEASE GO TO THE FOLOWING COLAB NOTEBOOK https://colab.research.google.com/drive/1_Z-E6Cia-xCtO1CkYg6yi5_3x3ImrCEe#scrollTo=hR5jbgE0yozB

# Introduction:

In anime (japanese animation)  the main characters present personality archetypes that are represented in drawn features and characteristics. For example a character called “tsundere” are represented for being cold, reserved, temperamental and sometimes even may be hostile, but with time, she will turns in a really  warm, sweet, kind and tender person. The general appearance of these anime characters are: innocent looking, angry faces, upset expressions and usually they have long hair.

The main objective of our project is to create a neural network that can classify a given image into their personality archetype. For example if we present the following image, the model should classify it as a tsundere.

For that pourpuse, we divided the main goal in the followings tasks:
* **Construction of waifus dere-type Database:** It is necessary to create a database with the main characters of every dere-type. 
* **Images Mining:** It is necessary to create our own images dataset because there is no one avalive of this topic on the internet. For that purpose we will mine 200 images for every waifu in the previously created database.
* **Data augmentation:** There are not enough images of this topic available for mining. So it is necessary to increase the data set for other methods.
* **Model construction:** It's necessary to create a model taking into account the small data set and the class imbalance presented in the dataset.

To get the dataset we designed a function using python module Selenium Chromedriver that can scrap from the internet any amount of images of a given topic. Then we created a list of the main representative characters of every personality archetype to scrape 1000 images of each one. Additionally we divide the data set in a careful way avoiding overlapping of characters between the train, test and dev dataset.
