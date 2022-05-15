# dialect-prediction-with-transformers

## Tech used

Transformers, Hugginface, Pytorch, Tensorflow, DVC, LIT tool.

## help full articles of some tech used


[DVC](https://stribny.name/blog/2020/10/versioning-large-files-in-git-with-dvc/)


Many countries speak Arabic; however, each country has its own dialect, the aim of this repo is to use huggingface tranforemers to build such a model using pre trained model as feature extraction, as well as fine tune the model with the dataset as classification task.

Next will be accelerate the model to work on online site.

We will directly use dialect dataset that we have processed in other work for the same purpose [Predict Your Dialect](https://github.com/Abdelrahmanrezk/AIM_ML_Task), so you will find the data splited into train, test and validation inside the direction of dataset.

## Note !

Because the train dataset is over 50mb, it can not pushed to github so we use data version controller to push on drive, and you can download from here:

Or you can unzip the file in train direction using "unzip strat_train_set.zip"















