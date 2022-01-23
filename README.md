# Proj_Deep
Megan Fillion & Killian Susini
Audio Spectrogram Transformer on FSDK50 dataset

In this directory, we have:

deep_learning_AST.ipynb which contains:
-	Dataset loader
-	AST model
-	training/test function
-	Visualization of output

Utils.ipynb: notebook containing multiple functions we needed to run before training like the mean and std of the dataset and how we created our smaller dataset

FSDK50 which contains:
-	FSDK50k.dev_audio: folder containing all images for train and validation in original dataset split (needs to be downloaded on fsdk50 website)
-	FSDK50k.eval_audio: folder containing all images for test set in original dataset split (needs to be downloaded on fsdk50 website)
-	FSDK50k.ground_truth: folder containing csvs for train/test/validation along with labels for all inputs in dev and eval audio. (only contains slim dataset)
-	dataset_slim.csv: csv containing all input audio and where they can be found in the original dataset for our custom smaller dataset 
	-	10500 entries in total
	-	5 classes
	-	Filenames.csv: name of all the files we have in the drive (seeing that the dataset is 30GB there were some issues during the upload. Just a couple of files missing here and there but this is just to avoid a ‘file not found’ error in the open() function)

Output folder containing the performance metrics and saved models for previous training:
-	18-01-2022_14:13:52
	-	Lr: 0.0001
	-	Epochs= 10
	-	Batch_size=8
-	18-01-2022_15:22:17
	-	Lr: 0.00001
	-	Epochs= 10
	-	Batch_size=8
-	18-01-2022_16:20:04
	-	Lr: 0.000005
	-	batch_size=16
	-	Epochs = 15
-	19-01-2022_12:49:19
	-	batch_size=8
	-	Data augmentation
	-	Normalization
	-	lr = 0.000005
-	19-01-2022_21:28:23
	-	Epochs = 100 
	-	21-01-2022_13:24:35
	-	Trained on small instead of tiny pretrained model


