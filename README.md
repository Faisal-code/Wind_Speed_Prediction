 <B> Note: </B> This repository is part of an ongoing project. At this stage, we are sharing selected portions of the codebase and a sample of the dataset. The complete source code and full private dataset will be made publicly available after the project's completion.


 <B>  Model Architecture  </B>  
The figure represents the end-to-end pipeline for the proposed VAE-S2S-BiLSTM-Encoder-Decoder model for short-term wind speed prediction. The architecture includes the following stages:


 <B> 1. Data Preprocessing  </B> 

* Inputs: Raw multivariate time series data consisting of temperature, humidity, wind speed, and power from Beijing’s weather.

 <B> Operations:  </B> 
 
  * Data cleaning: Removes noise and missing values.
  * Normalization: Uses Min-Max scaling to rescale all variables to a 0 to 1 range.
  * Temporal aggregation: Features like daily, weekly, and monthly patterns are extracted.
  * Visualization: Heatmaps, line plots, and box plots are used to capture seasonal patterns and detect outliers.
    
![Model Architecture](https://github.com/user-attachments/assets/4faa0398-ed89-4d40-be38-a0759da13e48)


  <B>  2. Feature Engineering  </B>  
* Purpose: Capture meaningful temporal dependencies and hidden correlations among variables.

 <B> •Techniques:  </B> 

* Seasonal and trend pattern analysis.
* Box plots and correlation heatmaps to explore dependencies between variables.
* Weekly and quarterly aggregations for modeling long-term trends.

<B> 3. Variational AutoEncoder (VAE) Module </B>
* Encoder: Maps high-dimensional input features into a probabilistic latent space 𝑧 using neural networks.
* Latent Space Sampling: Uses mean and variance to generate latent variables via the reparameterization trick.
* Decoder: Reconstructs the original data from latent representations, learning abstract and nonlinear features.

🔹 The VAE addresses dimensionality reduction, overfitting, and nonlinearity.  

