# Fine-grained-Pointcloud-Object-Dataset

## 1. Fine-grained object datasets
![fine-grained object 1](imgs/fine-grained_object.png)


**Fine-grained point cloud object dataset:** (left) ****20 restaurant categories (100 objects)**** in Gazebo environment (point cloud format *.pcd)
;  (right) ****120 categories shoe objects**** in Gazebo environment (point cloud format *.pcd)
![fine-grained object 2](imgs/fine-grained_object_img.png)
**Fine-grained restaurant and shoe dataset:** (left) ****20 restaurant categories (100 objects)**** RGB images
;  (right) ****120 categories shoe objects**** RGB images
# 

We developed a simulation environment in Gazebo to record fine-grained object datasets, including cars and shoes. 
Towards these goals, firstly, we considered 100 restaurant objects, imported from different resources(e.g., YCB datasets, Gazebo repository, and so on). It should be noted that this is a very challenging dataset for fine-grained RGB-D object recognition tasks since they are very similar together. For example, there are objects with the same geometry or color but different textures in these cars, and vice versa.

Secondly, in terms of the fine-grained shoe dataset, we collected 120 shoe objects, also sourcing from the Gazebo repository. The shoe dataset is also very valuable for fine-grained object classification, given their remarkable similarity. For instance, considering the shoes with the same style or tag, they can just be recognized according to their tiny color difference. Besides, their appearance distinctions are reflected in their same color but slightly different textures, and vice versa. 

In order to extract partially visible point clouds of every object, we move every object along a rose trajectory in front of the camera and record object views of the object. Finally, the obtained 1200 partial restaurant object views and 7200 shoe views are organized into 20 restaurant object categories and 120 shoe categories, respectively. 



## Citation

Please adequately refer to the paper any time this dataset is being used. If you do publish a paper where this dataset helped your research, we encourage you to cite the following paper in your publications:

```
@article{xiong2022fine,
  title={Enhancing Fine-Grained 3D Object Recognition using Hybrid Multi-Modal Vision Transformer-CNN Models},
  author={Songsong Xiong and Georgios Tziafas and Hamidreza Kasaei},
  journal={arXiv preprint arXiv:2210.04613},
  year={2023}
}
```
