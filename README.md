# dinosaurs image classification

This repository follows the instruction on [YouTube](https://www.youtube.com/watch?v=QfNvhPx5Px8)

## Prerequisites

[Docker](https://www.docker.com/products/docker-toolbox)

## Running

1. Download and start the docker image `docker run -it -v $HOME/tf:/tf tensorflow/tensorflow:latest-devel bash`
2. Run label_image to classify image. `python /tf/label_image.py  <path_to_image/file>` (500 training steps) or `python /tf/label_image_1000.py  <path_to_image/file>`(1000 training steps)

## Result

### With 500 training steps

#### Accuracy

#### Testing with Animantarx

#### Testing with Carnotaurus

#### Testing with Kentrosaurus

#### Testing with Mamenchisaurus

#### Testing with other dinosaurs

### With 1000 training steps



## Retrain the model

1. Add new images/files into /tf/dinosaurs
2. Retrain by running `python retrain.py --bottleneck_dir=/tf/bottlenecks --how_many_training_steps <number_of_training_steps> --model_dir=/tf/inception --output_graph=/tf/retrained_graph.pb --output_labels=/tf/retrained_labels.txt --image_dir /tf/dinosaurs`



