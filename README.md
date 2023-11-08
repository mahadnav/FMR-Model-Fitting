# FMR-Model-Fitting

This Jupyter Notebook is intended for performing model fitting on magnetic resonance data. The notebook provides functionality to fit different models to the data, including Spectrum, Kittel, and Linear models, to extract meaningful parameters. The provided code is written in Python and uses various libraries for data analysis and visualization.

## Prerequisites

Before running the notebook, make sure you have the following libraries installed:

- NumPy
- Matplotlib
- lmfit
- SciPy
- Scikit-image (skimage)

You can install these libraries using the following command:

```bash
pip install numpy matplotlib lmfit scipy scikit-image
```

## Usage

1. **Set Directory**: Change the `dir` variable to specify the directory where your data files are located.

2. **Load Data**: The notebook loads data from CSV files in the specified directory. It creates arrays for field and signal data.

3. **Set Frequency and Field Range**: Set the frequency and field range you want to analyze by adjusting the `lower_freq`, `upper_freq`, `lower_field`, and `upper_field` variables.

4. **Model Fitting**: The notebook fits the FMR Spectrum model to the data. You can customize the model by modifying the `dp_dh_script` and `dp_dh_model` functions.

5. **Smoothed Plot**: The code provides options to smooth the data using different filters and regularization techniques. You can visualize the results of smoothing using the provided functions.

6. **Integrated Plot**: The code also allows you to create an integrated plot using the fitted data. It can help visualize the integrated signal over a range of field values.

7. **Kittel Fitting**: The notebook performs Kittel fitting on the data, extracting parameters such as the gyromagnetic ratio, saturation magnetization, and uniaxial anisotropy.

8. **Linear Fitting**: The code performs linear regression on the line width data, extracting the Gilbert damping parameter.

## Outputs

The notebook generates various plots, including density plots, fitted plots, Kittel fitting plots, and linear fitting plots, depending on your chosen analysis. The results are saved in the specified output directory.

## Acknowledgment

The code provided in this notebook is intended for educational and research purposes. If you find it useful, please consider providing appropriate citations.

For more information and detailed explanations of the code, please refer to the comments within the notebook and the associated documentation.
