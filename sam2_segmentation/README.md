### Segmenting pointcloud with SAM2: 

1. From sam2: https://github.com/facebookresearch/sam2
2. conda create --name sam2 python=3.10
3. conda activate sam2
4. pip install torch==2.5.1
5. pip install torchvision==0.20.1
6. git clone https://github.com/facebookresearch/sam2.git
7. cd sam2
8. pip install -e .
9. pip install -e ".[notebooks]"
10. add the 3 files in sam2_additional_files of this repo (segment_pointcloud.ipynb, yolo_model.pt, sam2_hiera_small.pt) into your sam2/sam2 folder
11. run segment_pointcloud.ipynb to segment pointcloud input using the segmented images

Modification to SAM2 repo: add to /sam2/sam2/ segment_pointcloud.ipynb, filter_points.pt (remeber to use yolo.detect instead of yolo.track), sam2_hiera_small.pt, yolo_model.pt
