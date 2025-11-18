# INSA_notebooks
Link to the rendered notebook: https://drive.google.com/file/d/1Ckla245ZlHhbHLRnR3j0Shrr0RA2jXon/view?usp=sharing


To download the lfw dataset replace 
```
!wget http://vis-www.cs.umass.edu/lfw/lfw.tgz > /dev/null 2>&1
!tar zxvf lfw.tgz > /dev/null 2>&1
!mkdir data > /dev/null 2>&1
!mv lfw data > /dev/null 2>&1
```
with
```
import kagglehub
# Download latest version
path = kagglehub.dataset_download("jessicali9530/lfw-dataset")
print("Path to dataset files:", path)
```

And add the following cell right after:
```
!mkdir data
!mv /kaggle/input/lfw-dataset/lfw-deepfunneled/lfw-deepfunneled data/lfw
```
