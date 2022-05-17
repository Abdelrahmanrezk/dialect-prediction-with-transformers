# dialect-prediction-with-transformers

Many countries speak Arabic; however, each country has its own dialect, the aim of this repo is to use huggingface tranforemers and its datasets to:

- Push new datasets that was mentioned in the reference paper into the hub [Arabic Dialect Identification](https://arxiv.org/pdf/2005.06557.pdf)

- Build such a model using pre trained model as feature extraction with that pushed data. 

- Fine tune the model with the dataset as classification task.

- Next will be accelerate the model to work on online site.

We will directly use dialect dataset that we got in other work [Predict Your Dialect](https://github.com/Abdelrahmanrezk/Arabic-Dialect-Identification), so you will find the data splited into train, test and validation inside the direction of dataset.

## Note !

Aready we have pushed the data into the hub so you can use:

```
dialect_datasets = load_dataset('Abdelrahman-Rezk/Arabic_Dialect_Identification')
dialect_datasets

```

But, otherwise, Because the train dataset is over 50mb, it can not pushed to github so we use data version controller to push on drive, and you can download from here and put into dataset/train/:

[Download](https://drive.google.com/u/3/uc?id=1NEZufxSP9O6OjX7Lxzy6VByaGHxaq0BM&export=download)

Or you can unzip the file in dataset/dialect_data/train direction using "unzip strat_train_set.zip"



## Tech used

Transformers, Hugginface, Pytorch, Tensorflow, DVC, LIT tool.

## help full articles of some tech used

[DVC](https://stribny.name/blog/2020/10/versioning-large-files-in-git-with-dvc/)













