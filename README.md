# Link Prediction Pipeline Demo for Cross-Device Entity Resolution (ER)
Demonstrates the application of Neo4j Link Prediction Pipelines to a Cross Device 
Entity Resolution Problem. This analysis is inspired by the blog [here](https://towardsdatascience.com/exploring-practical-recommendation-engines-in-neo4j-ff09fe767782). The steps in this analysis are similar except:
1. We use Graph Data Science (GDS) version 2.0 here, while the blog was written on GDS 1.7.2
2. We use the Graph Data Science Python Client here which allows us to all our analysis and machine learning in Python


## Loading the Data
The source data and challenge problem for this demo can be found at: https://competitions.codalab.org/competitions/11171. The data is not committed here. To work with this example, please download `data-train-dca` from the above source, unzip, and place in a subdirectory named `./data`.  

The `prepare-and-load-data.ipynb` notebook samples and formats the source data into CSVs containing Nodes and Relationships then loads them into Neo4j. A larger subsample or the complete dataset can be used.  Just keep in mind that the larger the dataset, the more memory will be needed for GDS.

## Link Prediction Pipelines for ER
The `lp-pipeline-for-supervised-er-demo.ipynb` contains the link prediction pipeline and overall analysis. 

## Prerequisites
- Neo4j = 4.3, 4.4
- GDS = 2.0
- Python >= 3.6