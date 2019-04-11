# simple_yolov3_keras

the code was originally from https://github.com/experiencor/keras-yolo3 with the following modifications:

- You need to run `python gen_anchors.py -c config.json` first to generate the anchors (saved in anchors.json)
- Remove the bounding box adjustment in warmup batches. Instead, implemented the burnin learning reate as in network.c from Darkent
- Migrate from keras.* to tensorflow.keras.*
- Some bug fixes for tensorflow 1.12
