# Naive-Bees

This project helps identify input images between Honeybees(Genus Apis) and Bumblebees(Genus Bombus).

Step 1: This step involves downloading the .csv file from the website link: https://beespotter.org/beedata/rawdata. Make sure to register and login at the website before hand. Then download one of the datasets under the title "Listing of Identified Bee Spottings". The dataset has bee saved as Bee-data.csv. Since only few columns were actually required for this project, the rest were removed manually.

Step 2: The dataset Bee-data.csv has image-urls as values in one of the columns. Since our model will take a lot of time if it opens each url and then performs actions over it each time, therefore we have downloaded the images from these urls and saved it to disk using Extract-image.ipynb.

Step 3: Next step involves running Create_features.ipynb to convert images to feature matrix.

Step 4: Run Build_model.ipynb to train the models and find accuracies.

Step 5: Use Predict_img.ipynb to predict any input image as either Apis or Bombus.