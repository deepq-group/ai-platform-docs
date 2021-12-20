# Deploying Your Model(s) Elsewhere

After your training is completed, the next step is to test the performance of your trained model. This tutorial introduces how to download the trained model as well as the prediction script and the way to run the prediction on your machine locally.

## Requirements

* Nvidia docker (Ref: [https://github.com/NVIDIA/nvidia-docker](https://github.com/NVIDIA/nvidia-docker))
* Docker image (`docker pull deepqgroup/ai-platform-inference:inference-pytorch`)
* Unix-like command line interface

## Steps

### 1. Download training results

![](<../.gitbook/assets/image (74).png>)

Download the training results with the button, “models”, on the task details page. Extract the zip file, and there will be a folder, `results`. The folder contains at least `inference.py`, `model_X.bin` (X is the best step during training), and `label_name.csv`.

For this tutorial, we put `results` under the home directory, i.e.`~/results/`.

`cd ~`

`unzip ~/Downloads/results.zip`

`cd results`

### 2. Prepare a testing image

Put the image file or dataset into `~/results`. For example, we put an airplane image at `~/results/airplane.jpg`.

### 3. Prepare the Docker image

We provide a Docker image that all required packages were installed. You can easily run the test inside the docker container.

`docker pull deepqgroup/ai-platform-inference:inference-pytorch`

### 4. Start the Docker container

We mount `~/results` to `/results` inside the container with`-v`.

`docker run --runtime=nvidia -ti --rm -v ~/results:/results deepqgroup/ai-platform-inference:inference-pytorch bash`

### 5.Run testing

A scripts `predict.sh` is provided to classify an image easily. First, change directory to `/results`, and then run `predict.sh`!

`cd /results`

`./predict.sh -i ./airplane.jpg`

It will show the output of the inference with a json format. The output will look like the following:

`Output: create network: resnet18v1`

`RESULT {"scores": [0.9954907894134521, 0.00436920952051878, 0.00013990419392939657, 4.442737733256763e-08, 1.852817810288343e-08], "labels": ["airplane", "horse", "bird", "deer", "automobile"]}`

```
{
    "RESULT": {
        "scores": [
            0.9954907894134521, 
            0.00436920952051878, 
            0.00013990419392939657, 
            4.442737733256763e-08, 
            1.852817810288343e-08
        ], 
        "labels": [
            "airplane", 
            "horse", 
            "bird", 
            "deer", 
            "automobile"
        ]
    }
}
```

As shown in above output, "airplane" has the highest score, which implies the prediction is correct.

### Predict Script Usage

`./predict.sh -i ${image path or dataset dir} -h ${heatmap path} -B -b ${batchsize} -c -m`

* \-B: if specified, batch inference mode, gpu is required
* \-b: specify the batchsize for batch inference
* \-c: if specified, enable cuda
* \-h: specify the output path of heatmap, only required in classification
* \-i: specify the image path for inference mode or the dataset dir for batch inference mode
* \-m: if specified, with metrics
