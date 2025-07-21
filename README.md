Note: This repository is part of an ongoing project. At this stage, we are sharing selected portions of the codebase and a sample of the dataset. The complete source code and full private dataset will be made publicly available after the project's completion.

<B> Model architecture<B>
![Model Architecture](https://github.com/user-attachments/assets/4faa0398-ed89-4d40-be38-a0759da13e48)

<B> Model Architecture <B>
The figure represents the end-to-end pipeline for the proposed VAE-S2S-BiLSTM-Encoder-Decoder model for short-term wind speed prediction. The architecture includes the following stages:


<B> 1. Data Preprocessing <B> 
• Inputs: Raw multivariate time series data consisting of temperature, humidity, wind speed, and power from Beijing’s weather.

• Operations:

    - Data cleaning: Removes noise and missing values.

    - Normalization: Uses Min-Max scaling to rescale all variables to a 0–1 range.
    - Temporal aggregation: Features like daily, weekly, monthly patterns are extracted.
    - Visualization: Heatmaps, line plots, and box plots are used to capture seasonal patterns and detect outliers.
