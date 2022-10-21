# deep-learning-projects-
deep learning book


to download and unzip datasets using colab to gdrive
```
#first to mount the google drive
from google.colab import drive
drive.mount('/content/drive')

import requests
file_url = "datasets url"
    
r = requests.get(file_url, stream = True,verify = False) 
  
with open("path to download in", "wb") as file: 
    for block in r.iter_content(chunk_size = 1024):
         if block: 
             file.write(block) 
             
             
             
!unzip path_to_file.zip -d path_to_directory

```
to plot model in tensorflow 2.x 
```
from tensorflow.python.keras.utils.vis_utils import plot_model
plot_model(model, show_shapes=True, show_layer_names=True, to_file='model.png')
```
to download folder or file from google drive to kaggle
```
pip install gdown

import gdown

url = 'https://drive.google.com/uc?id=1B6_rtcmGRy49hqpwoJT-_Ujnt6cYj5Ba'
# output file should have the same extention as original file
output = 'file.npy'

gdown.download(url, output, quiet=False)
```
