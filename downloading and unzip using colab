import requests
 
file_url = "http://mng.bz/0tIo"
    
r = requests.get(file_url, stream = True,verify = False) 
  
with open("/content/gdrive/My Drive/imdb.zip", "wb") as file: 
    for block in r.iter_content(chunk_size = 1024):
         if block: 
             file.write(block) 
             
             
             
!unzip path_to_file.zip -d path_to_directory
