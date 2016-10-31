# nba_pred
Model to predict regular season win percentage for each NBA team using historical data

starting build for URL: https://github.com/shaundre3000/nba_pred
fetching source at https://github.com/shaundre3000/nba_pred
 ---> 10c75734a0d4
Step 2 : RUN mkdir /home/main/notebooks
 ---> Running in b9d64230d43d
Step 1 : FROM andrewosh/binder-base:latest
 ---> cdcb81dab9ed
Removing intermediate container b9d64230d43d
Step 3 : RUN chown main:main /home/main/notebooks
 ---> Running in e0424964fffa
 ---> 4fd0730d3419
Step 4 : WORKDIR /home/main/notebooks
Removing intermediate container e0424964fffa
 ---> Running in 4c59f42e671b
 ---> 7eb56c7a9f43
Removing intermediate container 4c59f42e671b
Step 5 : USER root
 ---> Running in 8222670dd8e2
 ---> 0b2f02b7df55
Removing intermediate container 8222670dd8e2
Step 6 : COPY . /home/main/notebooks/
 ---> 0c2ebbf8b78f
Removing intermediate container 2f12ecb2172a
Step 7 : RUN chown -R main:main $HOME/notebooks
 ---> Running in 6987761f9031
 ---> 9b3091e81c6d
Step 8 : USER main
Removing intermediate container 6987761f9031
 ---> Running in 511ab1ec9ddd
 ---> 9a19a53a4cda
Removing intermediate container 511ab1ec9ddd
Step 9 : RUN find $HOME/notebooks -name '*.ipynb' -exec jupyter trust {} \;
 ---> Running in db428b12521c
[91m[TrustNotebookApp] Writing notebook-signing key to /home/main/.local/share/jupyter/notebook_secret[0m
Signing notebook: /home/main/notebooks/Predicting NBA Win Percentage by Season.ipynb
Signing notebook: /home/main/notebooks/.ipynb_checkpoints/Predicting NBA Win Percentage by Season-checkpoint.ipynb
 ---> b1acf8471a0d
Removing intermediate container db428b12521c
Step 10 : USER main
 ---> Running in 8b74d07fab5f
 ---> 10c0aeba05fc
Removing intermediate container 8b74d07fab5f
Step 11 : WORKDIR $HOME/notebooks
 ---> Running in 2bd7c6a1254e
 ---> 2772feebcfa4
Removing intermediate container 2bd7c6a1254e
Successfully built 2772feebcfa4
registering template for shaundre3000-nba_pred
