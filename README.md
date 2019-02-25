# panoptic

Files related to implementation of panoptic segmentation for Cityscapes dataset.

Combines semantic segmentation from Deeplab V3 (Google) with instance segmentation from Mask R-CNN (Matterport) using heuristics described in Kirillov, et al, 2018.

instance_to_panoptic.ipynb : Main file used to produce panoptic segmentation from semantic segmentation and instance segmentation of images. This notebook has been adapted from the Mask R-CNN demo notebook to perform instance segmentation of a directory of image files, and combine these instance segmentations with semnatic segmentations using hueristics. The model implementation is the work of Matterport, while subsequent production of panoptic segmentations is due to Casey Galvin.

TFrecord_creator_cityscapes.ipynb : Jupyter notebook for converting Cityscape image data to TFrecord files for training and inference using Deeplab V3+. Adapted for use in Jupyter notebook from file included with Deeplab V3+.

vis.py : File from Deeplab V3+ to perform inference on images. Adapted to use for the purpose of this repository.

train_vis_commands.txt : Command line commands to execute vis.py or train.py to perform inference or train Deeplab model

panoptic_results.zip : Contains panoptic segmentation maps colored according to class label and instance number
