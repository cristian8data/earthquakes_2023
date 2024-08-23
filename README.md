# Study of global seismic activity in 2023 using machine learning models and neural networks
This master's thesis analyses data from earthquakes that occurred in 2023 and uses machine learning and deep learning models to predict the magnitude of earthquakes.

Before developing the predictive models, an exploratory and detailed analysis of the seismic data was carried out in order to better understand the nature of the data. These analyses include graphs and tables on the distribution of different variables such as magnitude, depth or type of earthquakes, as well as geospatial maps showing the distribution of earthquakes, temporal analysis, analysis of seismic detection stations and errors made in measurements.

The dataset is uploaded on the Kaggle website (Keser, M., 2024) from where it has been used to perform the analysis. Kaggle is an online platform that allows anyone to access and use different data sets to perform data analysis challenges, being able to share the results and collaborate on projects with more people. The link to access the notebook with the code of this proyect in Kaggle is: https://www.kaggle.com/code/cristian8data/earthquakes-2023

## Authors
- [Cristian Morillo Losada](https://www.github.com/cristian8data)

## Project Structure
- `earthquakes_2023_TFM.ipynb`: Contains the full code and analysis.
- `earthquakes_2023_TFM_report.pdf`: Final project report in spanish.
- `README.md`: Project guide.

## Installation

This project utilizes a dataset available directly in the Kaggle environment. The dataset is automatically provided in the `/kaggle/input/` directory when you run the notebook on Kaggle.

To locate the CSV file used in this analysis, the following code snippet was used within the notebook:

```python
import os

for dirname, _, filenames in os.walk('/kaggle/input'):
    for filename in filenames:
        print(os.path.join(dirname, filename))
```

This code will output the path to the dataset file, which in this case is:

/kaggle/input/earthquakes-2023-global/earthquakes_2023_global.csv

## Results
This study explored the prediction of earthquake magnitudes using machine learning and deep learning models, analyzing data from the USGS in 2023. Most seismic events in the dataset were natural earthquakes with magnitudes between 4 and 5 and occurred at depths less than 100 km, primarily near tectonic plate boundaries.

Ensemble models like Random Forest and XGBoost outperformed linear models and KNN in predicting earthquake magnitude, thanks to their ability to capture complex, nonlinear relationships in the data. Neural networks also performed well but required more complex tuning. Future work could focus on refining neural networks with deeper architectures and better hyperparameter optimization.

## License
[MIT](https://choosealicense.com/licenses/mit/)
