# Content based image retrieval

[Content-based image retrieval][1] (CBIR) is the application of computer vision techniques to the image retrieval problem, that is, the problem of searching for digital images in large databases.

**Content-base** means that the search analyzes the contents of the image rather than the metadata such as keywords, tags, or descriptions associated with the image.

![CBIR](./notebooks/cbir.png)

It is carried out in three steps:
1. extraction of features from an image database to form a feature database,
2. extraction of the features of the input image,
3. find the most similar features in the database,
4. return the image associated with the found features


### features extraction

* [MobileNet]


**The objective is to find the right combination (extraction algorithm & similarity measure) that allows to have relevant answers.**

## Dataset

 I used the following dataset:

* Art dataset https://github.com/delchiaro/NoisyArt

## How to install
First, you need to create a MySQL database called 'tesi' with a table 'immagesforretrieval'
that has 3 rows: 
* artwork, which contains the artwork title
* detail, which specifies the detail position 
* path, which contains the image path

Then you have to execute:
1. prepairData.py that loads data into the db and creates the details
2. build_dataset.py that defines the features types
3. build_features that build features

If you want to test your app you can use the test.py file




