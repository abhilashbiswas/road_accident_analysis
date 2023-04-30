# Reducing Deaths and Injuries in Traffic Accidents in Allegheny County
Team members: Abhilash Biswas, Matt Lampl, Vidisha Chowdhury

Road accidents are the major cause of injuries and deaths in the United States. While there are several organizations and governmental units focused on this problem full time, needs and causes of accidents may differ from place to place. More importantly, a wide range of policies could be relevant to tackle the problem, and figuring out the right mix of policies for a particular region could be a non-trivial task. 

In this project, we provide explorations and analysis from road accidents in Allegheny County between 2004-2021. Using a mix of geospatial analysis, predictive modeling and unsupervised learning, we demonstrate the various factors associated with accidents that result in major injury or death. We find that accidents are mostly concentrated in major highways and denser cities within the county (like Pittsburgh). We find that less shielded occupants of the road such as pedestrians and motorcyclists are more likely to suffer injuries and deaths in accidents. We also find that bad road conditions (such as icy roads, curved roads) combined with impaired driving (under the effect of alcohol, drugs) are likely causes of accidents of interest. 

Along with providing recommendations on the above mentioned factor, we propose a set of future work that addresses the limitations of this study. We propose an in-depth temporal analysis of these factors to differentiate between long term factors versus those that started being important more recently. Since correlation is not necessarily causation, we also propose taking advantage of differences in interstate laws to further drill down on the above mentioned factors and evaluate, using a causal study, on which of the factors has the highest potential to bring the maximum reduction in injuries and deaths and road accidents. 


## Output matrials
1. Final report -- [Here](https://docs.google.com/document/d/1gKRp6GIRNq3Eyo-XV72UTQYgTDH13PtXOCXys9Nx51s/edit#)
2. Final presentation -- [Here](https://docs.google.com/presentation/d/1nWjtHbG6MJm995zNjz3mCIcYoWwyDZOAG7NLHKI_vkE/edit#slide=id.g23952da010a_0_18)

## Repository description

### EDA
This folder contains the analysis notebook `initial_eda.ipynb`. This provides all the initial exploration data analysis that informed out subsequent analysis

### maps
This folder contains the analysis notebook `geo_analysis.ipynb`. This provides all the geospatial analysis

### machine_learning
This folder contains 2 analysis notebooks. Each of the analysis notebook perform data cleaning and preprocessing within the notebook before training models. 

- `prediction.ipynb`
This notebook contains all the code for predictive analysis and associated results

- `unsupervised.ipynb`
This notebook contains all the code for unsupervised analysis and associated results

## How to run this codebase

### Step 1:
Clone the repo into a local folder. 
`git clone https://github.com/abhilashbiswas/road_accident_analysis.git`

### Step 2:
Download the accident dataset from Western Pennsylvania Regional Data Center ([link here](https://data.wprdc.org/dataset/allegheny-county-crash-data/resource/2c13021f-74a9-4289-a1e5-fe0472c89881)). Rename the csv `accident_data.csv` and place it inside the `Data` folder. The title of the dataset is "Cumulative Crash Data (2004-2021) and can be downloaded in full by hitting the Download button at the link destination. The folder already contains the data dictionary for this data, called `accident_data_dict.csv`. 

### Step 3:
Once step 1 and 2 is done, clone any of the notebooks can be run. 