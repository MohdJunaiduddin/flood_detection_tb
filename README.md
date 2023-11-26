# flood_detection_tb
## Dataset
  - There are 31 images (complete) in folders such as nebraska_20170108t002112.
  - Images are further divided into images of size 256*256.
  - The folders have 4 types of images vv, vh, flood_label and water_body_label.
  - The complete image has padding that is empty this empty space can cause problems while training and must be dealt with.
## Preprocessing
  - Built two functions which combine vh and vv image to give a single image.
  - Built a function(out) to combine flood_label and water_body_label to only give a image which shows only a flood reigion.
  - Built a dropper function which drops the image which has significant padding.
## Modeling
  - Found a simple model on stackoverflow for image to image.
  - Model first scales down the iamge and then scales up the image.
## Traning 
  - Could not train on complete traning set due to memory restriction.
  - Used only one of the two function to combine vh and vv image, used dropper and out function.
  - Due to laptop limitations, batch_size was set to 1. 
  - Trained model is stored in h5, json file.

