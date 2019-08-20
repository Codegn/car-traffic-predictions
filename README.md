# car-traffic-predictions
Using conda env
0. conda create --name keras_cpu tensorflow keras pandas matplotlib jupyterlab dask
1. conda activate keras_cpu
2. jupyter lab

Using docker:
1. docker run --name jupyter-tensorflow-rnn -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -v ${PWD}:/home/jovyan/work jupyter/tensorflow-notebook:58169ec3cfd3
2. docker start jupyter-tensorflow-rnn -a

In case of using tensorflow-gpu and to check if gpu is good to go paste the folowing in terminal:
1. python
2. import tensorflow as tf
3. sess = tf.Session(config=tf.ConfigProto(log_device_placement=True))
