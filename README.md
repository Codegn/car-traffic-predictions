# car-traffic-predictions
Using conda env
0. conda create --name keras_cpu tensorflow keras pandas matplotlib jupyterlab dask
1. conda activate keras_cpu
2. jupyter lab

Using docker:
1. docker run --name jupyter-tensorflow-rnn -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -v ${PWD}:/home/jovyan/work jupyter/tensorflow-notebook:58169ec3cfd3