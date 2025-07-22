 <B> Note: </B> This repository is part of an ongoing project. At this stage, we are sharing selected portions of the codebase and a sample of the dataset. The complete source code and full private dataset will be made publicly available after the project's completion.


 Model Architecture 
The figure represents the end-to-end pipeline for the proposed VAE-S2S-BiLSTM-Encoder-Decoder model for short-term wind speed prediction. The architecture includes the following stages:


1. Data Preprocessing 

• Inputs: Raw multivariate time series data consisting of temperature, humidity, wind speed, and power from Beijing’s weather.

•  Operations:

    * Data cleaning: Removes noise and missing values.
    * Normalization: Uses Min-Max scaling to rescale all variables to a 0 to 1 range.
    * Temporal aggregation: Features like daily, weekly, and monthly patterns are extracted.
    * Visualization: Heatmaps, line plots, and box plots are used to capture seasonal patterns and detect outliers.
    
![Model Architecture](https://github.com/user-attachments/assets/4faa0398-ed89-4d40-be38-a0759da13e48)


 2. Feature Engineering 
Purpose: Capture meaningful temporal dependencies and hidden correlations among variables.

•Techniques:

* Seasonal and trend pattern analysis.
* Box plots and correlation heatmaps to explore dependencies between variables.
* Weekly and quarterly aggregations for modeling long-term trends
