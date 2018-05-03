This is fully ready Docker container with:
 - NumPy
 - Pandas
 - Sklearn
 - Matplotlib
 - Seaborn
 - pyyaml
 - h5py
 - Jupyter
 - Tensorflow
 - Keras
 - OpenCV 3

 ### Quickstart

```sh
git clone git@github.com:seanfcarroll/data_science.git
cd data_science
docker build . -t data_science
```

Docker container with the following command:
```sh
docker run -it data_science -p 8888:8888 -p 6006:6006 -d -v $(pwd)/notebooks:/notebooks
```
We're using following parameters:
- ```-p 8888:8888``` to export Jupyter Web interface
- ```-p 6006:6006``` to export TensorflowDashboard Web interface
- ```-d``` to run Docker container in background
- ```-v notebooks:/notebooks``` to mount just created *notebooks* folder Docker inside container


Inspired by: https://github.com/andreivmaksimov/python_data_science
