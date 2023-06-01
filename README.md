# Pattern Recognition for Robotics

This project focuses on investigating the use of pattern recognition techniques to identify objects by touch using tactile sensors. The data set used for this coursework was collected by the PR2 robot at the University of Pennsylvania's GRASP lab, equipped with two BioTac tactile sensors on its 2-finger gripper. The data set includes measurements of pressure, temperature, vibration, and 19 electrode measurements.

## Background
Humans rely on touch to classify and understand objects, especially when visual information is limited or insufficient. The goal of this coursework is to explore whether robots can also identify objects using tactile sensors. The specific objectives are:

A. Determine if the robot can use the tactile sensors to identify objects by grasping them.
B. Investigate whether cheaper finger hardware with fewer sensor types can also identify different objects and determine the impact on performance.

The data set used in this project was collected using expensive hardware and is relatively smaller compared to typical machine learning applications. The coursework is to be completed in Matlab, utilizing built-in functions.

## Sections
## A: Data Preparation
This section involves preparing the data for analysis, including extracting relevant information and organizing it into suitable data structures.

## B: Principal Component Analysis (PCA)
1. Visualize the time series sensor data for the variables Pressure, Vibration, Temperature (PVT), and Electrodes for several objects and trials. Select a time step that allows differentiation between data for different objects.

2. Sample the PVT time series data into scalar values at the selected time step for each object/trial. Save the data structures as .mat files.

3. Create a 3D scatter plot of the complete contents of the PVT mat file, with Pressure, Vibration, and Temperature as axes, using different colors for different objects.
4. Use PCA to determine the principal components of the PVT data:
a. Report covariance matrix, eigenvalues, and eigenvectors for the data.
b. Replot the standardized data with the principal components displayed.
c. Reduce the data to 2 dimensions and replot.
d. Plot the data distribution across all principal components using separate 1D number lines.
e. Comment on the findings.
5. Perform PCA on the electrode data:
a. Determine the principal components and report the variances using a Scree plot.
b. Visualize the electrode data using the three principal components with the largest variance.
c. Comment on the findings.

## C: Linear Discriminant Analysis (LDA)
Apply Linear Discriminant Analysis (LDA) to analyze the PVT data:
a. Split the training data based on Pressure vs. Vibration, Pressure vs. Temperature, and Temperature vs. Vibration. Plot the results, including the LDA
