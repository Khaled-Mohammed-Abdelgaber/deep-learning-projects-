# deep-learning-projects-
deep learning book
## to download using colab use:
import requests
 
file_url = "http://mng.bz/0tIo" # url to download from
    
r = requests.get(file_url, stream = True,verify = False) 

with open("/content/gdrive/My Drive/imdb.zip", "wb") as file:  # "/content/gdrive/My Drive/imdb.zip" is location where we want to store in

    for block in r.iter_content(chunk_size = 1024):
    
         if block: 
         
             file.write(block) 
             
             
            
            
## to unzip file in gdrive using colab use

!unzip path_to_file.zip -d path_to_directory
