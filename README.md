# ComputerVision-Starfish-Detection-with-Yolo

## Project Description
The was a kaggle competition: TensorFlow - Help Protect the Great Barrier Reef. Detect crown-of-thorns starfish in underwater image data. [Link](https://www.kaggle.com/competitions/tensorflow-great-barrier-reef/overview)

## Aim
Predict the presence and position of crown-of-thorns starfish in sequences of underwater images taken 
at various times and locations around the Great Barrier Reef. 
Predictions take the form of a bounding box together with a confidence score for each identified starfish. 
An image may contain zero or more starfish.


## Data Description (Data [Link](https://www.kaggle.com/competitions/tensorflow-great-barrier-reef/data))

train/ - Folder containing training set photos of the form video_{video_id}/{video_frame_number}.jpg.

[train/test].csv - Metadata for the images. As with other test files, most of the test metadata data is only available to your notebook upon submission. Just the first few rows available for download.

    video_id - ID number of the video the image was part of. The video ids are not meaningfully ordered.
    video_frame - The frame number of the image within the video. Expect to see occasional gaps in the frame number from when the diver surfaced.
    sequence - ID of a gap-free subset of a given video. The sequence ids are not meaningfully ordered.
    sequence_frame - The frame number within a given sequence.
    image_id - ID code for the image, in the format '{video_id}-{video_frame}'
    annotations - The bounding boxes of any starfish detections in a string format that can be evaluated directly with Python. Does not use the same format as the predictions you will submit. Not available in test.csv. A bounding box is described by the pixel coordinate (x_min, y_min) of its upper left corner within the image together with its width and height in pixels.

## Description
The folder code/ contains jupyter notebooks which uses Yolo-m to detected starfish from the under-water images.
