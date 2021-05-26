# Look Tests

## Introduction 
This is a full face detection and recognition system. For the detection part [MTCNN](https://github.com/ipazc/mtcnn) package is used. The recognition is achieved by using both a sparse representation method and using a Keras implementation of [FaceNet](https://github.com/faustomorales/keras-facenet) to get the embeddings.

## Getting Started

### Embeddings

1. Clone this repository. After that, you need to unzip the example dataset contained in face_recognition_embeddings/datasets.

2. With Docker installed, run the following command inside the "face_recognition_embeddings" directory

    ```
    docker build -t look_test:v1 .
    ```

3. After the image is created, run the following command

    ```
    docker run --gpus all -p 8501:8501 look_test:v1
    ```

4. Open the app in [http://localhost:8501/](http://localhost:8501/)