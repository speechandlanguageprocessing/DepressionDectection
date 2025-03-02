# DepressionDectection

This depression detection work is run on **Jupyter notebook**.

### Dataset

1. DAIC: https://dcapswoz.ict.usc.edu/
2. AVID: http://avec2013-db.sspnet.eu/
3. To obtain both DAIC and AVID datasets, agreement forms should be signed and return to corresponding email address

### How to run

##### DAIC

Classification model training code and regression model training code are provided in **classfication folder** and **regression folder**. To run the code, **prefix** in *BiLSTM.ipynb, cnn_audio.py and fusion_net.ipynb* should be set to the path where DAIC dataset placed. To run *fusion_net.ipynb*, path of trained **lstm_model** and **cnn_model** should be set corresponding path.

##### AVID

Preprocessing code of audio recordings in AVID dataset is offered in **AudioPreprocess.ipynb**. You should change the paths to your AVID dataset path before runing. Regression model training code is provided in **cnn_audio_reg_avid.py**. The input required by the training code is preprocessed audio clips, which is saved in **avid_info.pkl**. Therefore, **prefix** varaible should be set to the path where **avid_info.pkl** stored during the preprocessing step.

### Ref
The code is the implementation of the paper [Towards Automatic Depression Detection: A BiLSTM/1D CNN-Based Model](https://www.mdpi.com/2076-3417/10/23/8701).
If you find the paper or the code is useful, please cite the paper below.

```
@Article{app10238701,
AUTHOR = {Lin, Lin and Chen, Xuri and Shen, Ying and Zhang, Lin},
TITLE = {Towards Automatic Depression Detection: A BiLSTM/1D CNN-Based Model},
JOURNAL = {Applied Sciences},
VOLUME = {10},
YEAR = {2020},
NUMBER = {23},
ARTICLE-NUMBER = {8701},
URL = {https://www.mdpi.com/2076-3417/10/23/8701},
ISSN = {2076-3417},
}
```
