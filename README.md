# Fine-grained-Pointcloud-Object-Dataset

### 1. Fine-grained object datasets
![fine-grained object 1](imgs/fine-grained_object.png)

**Synthetic point cloud object dataset:** (left) 13 categories car objects in Gazebo environment (point cloud format *.pcd)
;  (right) 120 categories shoe objects in Gazebo environment (point cloud format *.pcd)


# 

We developed a simulation environment in Gazebo to record fine-grained object datasets including cars and shoes. Towards this goal, we considered 90 simulated household objects, imported from different resources (e.g., the YCB dataset, Gazebo repository, and etc). It should be noted that this is a very challenging dataset for object recognition tasks since we include both basic-level (i.e., objects that are not similar to each other such as apple vs. book) and fine-grained (the object that are very similar together spoon vs. fork) object categories. Furthermore, there are several objects with the same geometry, but different textures, and vice versa. In order to extract partially visible point clouds of an object, we move the object along a rose trajectory in front of the camera and record 300 views of the object. The obtained 27000 partial views are then organized into 90 object categories. 

