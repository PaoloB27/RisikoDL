# Risiko! tanks and flags detection
## Material provided
Everything has already been provided: all files after having run all the notebooks have been included in the folder.
## How to run the code
The code has been split into notebooks. Here is reported the order in which to run the notebooks:
  - “Risk!_Synthetic_Dataset_Creatore.ipynb” to generate the synthetic images (will put them in the created folder “synthetic_dataset”);
  - “Split_train_test_val.ipynb” to split the images in the three folders “real_images”, “synthetic_images” and “synthetic_dataset” into training set, validation set and test set (will create folder “datasets” containing the divided images and related labels);
  - “Tanks_flags_detection_training.ipynb” to fine tune the model yolov5 using only synthetic images and to fine tune the model yolov5 using both synthetic and real images. It will also save the results of the two training experiments in the folder "training_results";
  - “Test_detection.ipynb” to evaluate the model trained only on synthetic images and the model trained on synthetic and real images;
  - “Risk! Test.ipynb” to see how the yolov7 provided model works, in order to compare it to the two models implemented before.
