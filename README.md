# A Neural Conversational Model [![hb-research](https://img.shields.io/badge/hb--research-experiment-green.svg?style=flat&colorA=448C57&colorB=555555)](https://github.com/hb-research)

This is a forked version of the original [conversation-tensorflow] repository. It is aimed to prepare defined model for exporting it to `tf.saved_model` format and use it later one for serving. 

In order to export the model you would need to train it on the Cornell Movie-Dialogs Corpus or any other data source that available for you (but you need to prepare it). After model training, simply run exporting script `python export.py --config {data-profile}`. 

For the testing purposes you can do the following:
1. Train the model for a while on a sample data: 
`python main.py --config check_tiny --mode train`
2. Export the trained model:
`python export.py --config check_tiny