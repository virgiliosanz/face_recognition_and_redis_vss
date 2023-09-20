# face_recognition_and_redis_vss
Repo with a jupyter notebook to implement face recognition using redis vector similarity search

## HowTo

### How to install tensorflow (and Deepface) in Silicon Mac

[Setup Apple Mac for Machine Learning with TensorFlow (works for all M1 and M2 chips)](https://www.mrdbourke.com/setup-apple-m1-pro-and-m1-max-for-machine-learning-and-data-science/)

I checked and Tensorflow uses the GPU. :D

### Start the environment using conda

 conda create --prefix ./.env python=3.11
 conda activate ./.env

Install tensorflow packages for Mac M1:

 conda install -c apple tensorflow-deps
 conda install jupyter pandas numpy matplotlib scikit-learn
 python -m pip install tensorflow-macos
 python -m pip install tensorflow-metal
 python -m pip install tensorflow-datasets
 python -m pip install redis
 python -m pip install jupyter
 python -m pip install deepface

Then install [redis-stack](https://redis.io/docs/getting-started/install-stack/) and run it:

 $ redis-stack-server

 and run the jupyter notebook
  
 ./.env/bin/jupyter notebook

 open the notebook and start playing

### Notes

[Redis As A Vector Database: Fast Vector Similarity Search with RediSearch](https://sefiks.com/2023/07/13/redis-as-a-vector-database-fast-vector-similarity-search-with-redisearch/)
