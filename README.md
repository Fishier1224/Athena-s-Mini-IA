# Athena-s-Mini-IA
Deploying CNN model with Pytorch to iOS development 

## File Descriptions
### "Taichi vs Tennis"
This is the folder for training the Pytorch model. The folder does not include the directory "Data" (which includes subfolders "train" and "val") due to file size considerations. The missing "Data" directory should include the database for this model. Which are:
<br /> train -> taichi 840 photos and tennis 840 photos
<br /> val -> taichi 210 photos and tennis 210 photos 
<br /> With such a set up, the total database is 1050 photos for both subjects - tachi and tennis - while the validation set is 20% of the total database.
#### "test.py" and "train.py" 
These are transfer learning models from the Kaggle "Cats vs Dogs" project. A total of five epochs are run. 
