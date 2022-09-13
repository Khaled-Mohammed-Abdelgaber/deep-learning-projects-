# deep-learning-projects-
deep learning book


to download and unzip datasets using colab to gdrive
```
import requests
 
file_url = "datasets url"
    
r = requests.get(file_url, stream = True,verify = False) 
  
with open("path to download in", "wb") as file: 
    for block in r.iter_content(chunk_size = 1024):
         if block: 
             file.write(block) 
             
             
             
!unzip path_to_file.zip -d path_to_directory

```
