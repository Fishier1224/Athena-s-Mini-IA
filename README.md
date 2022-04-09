# Athena-s-Mini-IA
Deploying CNN model with Pytorch to iOS development 
The subjects of Pytorch model is Taichi vs. Tennis. I have selected these two subjects similarities actually exists between the poses of Taichi and the serving moves of Tennis. In addition, since they are all sports - but one Eastern and the other Western - I thought it would be interesting to compare them.

## File Descriptions
### "Taichi vs Tennis"
This is the folder for training the Pytorch model. The folder does not include the directory "Data" (which includes subfolders "train" and "val") due to file size considerations. The missing "Data" directory should include the database for this model. Which are:
<br /> train -> taichi 840 photos and tennis 840 photos
<br /> val -> taichi 210 photos and tennis 210 photos 
<br /> With such a set up, the total database is 1050 photos for both subjects - tachi and tennis - while the validation set is 20% of the total database.
#### "test.py" and "train.py" 
These are transfer learning models from the Kaggle "Cats vs Dogs" project. A total of five epochs are run. 
#### "model.pt" and "model_original.pt"
These are exports of the trained model, which will be later used for iOS development. Note that the former document will be directly included in the swift project, while the latter file is not as important.

## Bugs and Modifications
### Changing the model
My initial plan was to "simply" deploy my other CNN model (which used OpenPose) on Taichi to an iOS environment, but things got really complicated. My first attempt resulted in mismatched connection between the data collection, allocation, and model output. Thus, I decided to keep things simple and started with the Kaggle "Cats vs Dogs" model. Then transferred that model for Taichi. 
