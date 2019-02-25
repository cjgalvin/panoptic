# panoptic

Files related to implementation of panoptic segmentation for Cityscapes dataset.

Combines semantic segmentation from Deeplab V3 (Google) with instance segmentation from Mask R-CNN (Matterport) using heuristics described in Kirillov, et al, 2018.

vis.py : File from Deeplab V3+ to perform inference on images. Adapted to use for the purpose of this repository.

train_vis_commands.txt : Command line commands to execute vis.py or train.py to perform inference or train Deeplab model

panoptic_results.zip : Contains panoptic segmentation maps colored according to class label and instance number
