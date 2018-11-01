In this file, we explain how to install Nvidia GPU of tensorflow  on
your local machine running Ubuntu 16.04 LTS. I just followed the steps
at https://github.com/tensorflow/tensorflow/tree/master/tensorflow/tools/docker or  https://www.tensorflow.org/install/.

Since I needed several dependencies for each task, I learned about the first package at the last node. So I though I should document the steps I took. The overal process is easy.

## Step 1.  Install the Docker

The Docker comes with two editions: Enterprise Edition (EE) and Communitee Edition (CE), which is free. You just need to sign up and get it from here: https://docs.docker.com/install/linux/docker-ce/ubuntu/#install-docker-ce-1


## Step 2. Install nvidia-docker

You just need to follow the steps at https://github.com/NVIDIA/nvidia-docker.


## Step 3. Enjoy working with tensorflow-GPU

run the follwoing command to open a jupyter nortebook and enjoy your GPU version of tensorflow, see https://github.com/tensorflow/tensorflow/tree/master/tensorflow/tools/docker.
<pre><code>
nvidia-docker run -it -p 8888:8888 tensorflow/tensorflow:latest-gpu
</code></pre>


## Other Good Resources

* https://affinelayer.com/docker/ 
* https://medium.com/@flavienguillocheau/documenting-docker-with-gpu-deep-learning-for-noobs-2edd350ab2f7
* https://blogs.technet.microsoft.com/machinelearning/2018/03/15/demystifying-docker-for-data-scientists-a-docker-tutorial-for-your-deep-learning-projects/
* https://docs.nvidia.com/deeplearning/dgx/pdf/User-Guide.pdf
