# LeoStellarMotion

Analyzing the motion of stars in the Leo constellation using spectral data

# Introduction

LeoStellarMotion is a spectral analysis project that examines the motion of stars in the Leo constellation. By analyzing their hydrogen absorption wavelengths, we determine whether the 
stars are moving toward (blueshift) or away (redshift) from us using the Doppler effect.

# Features

✔️ Loads pre-saved MATLAB workspace variables from matlab.mat

✔️ Plots stellar spectra from observational data

✔️ Identifies the hydrogen absorption line in each star's spectrum

✔️ Calculates redshift (z) and velocity of the stars

✔️ Classifies stars as redshifted (moving away) or blueshifted (moving closer)

✔️ Visualizes results with differentiated plots for redshift and blueshift


# Technologies Used

MATLAB (for data analysis and visualization)


# Installation & Setup

1. Clone the repository:

          git clone https://github.com/yourusername/LeoStellarMotion.git

          cd LeoStellarMotion

2. Open MATLAB and load the pre-saved workspace:
   
          load('matlab.mat')  % Loads the saved workspace variables

3. Run the MATLAB script to analyze stellar motion:

          run('stellar_motion_analysis.m')

# How It Works

1. Loading Spectral Data

      -Instead of manually entering data every time, the project loads matlab.mat, which contains saved workspace variables (spectra, starnames, etc.).

      -Redshift / Blueshift Analysis

2. Finds the minimum intensity (hydrogen absorption line).

      -Determines its wavelength shift (λHa).

      -Computes redshift (z) using the formula:

              𝑧= (𝜆𝐻𝑎/656.28)−1
  
      -Calculates the velocity (km/s) of the star:

              𝑣=𝑧×299792.458

      -Classifies stars as moving away (redshift) or moving closer (blueshift).

3. Plotting Results

      -Uses different line styles for redshifted and blueshifted stars.

      -Displays star names in the legend.

# Results & Insights

      -Stars (moving away) have thicker lines in the plot.

      -Blueshifted Stars (moving closer) have dashed lines.

      -The identified redshifted stars are stored in movaway.

# Future Enhancements

🔹 Automate spectral data collection from databases like Sloan Digital Sky Survey (SDSS)

🔹 Compare results with real astronomical observations

🔹 Improve visualization with interactive plots

# Contributing

Contributions are welcome! If you’d like to improve this project:

1. Fork the repository
   
2. Make changes
   
3. Submit a pull request
   
# License

This project is licensed under the MIT License.
