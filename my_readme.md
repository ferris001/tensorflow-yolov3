# Macbook Pro
* Build docker:
    ``` shell
    cd docker
    docker build --rm -f dockerfile -t "tensorflow-yolo3:latest" .
    ```
* Run docker: 
    ``` shell
    docker run -u $(id -u):$(id -g) -it --rm -v ${PWD}/:/tensorflow-yolo3 -w /tensorflow-yolo3 tensorflow-yolo3:latest bash
    ```

# TanXufeng-ml
* Build docker:
    ``` shell
    cd docker
    docker build --rm -f dockerfile-gpu -t "tensorflow-yolo3:latest-gpu" .
    ```
* Run docker: 
    ``` shell
    nvidia-docker run -u $(id -u):$(id -g) -it --rm -v ${PWD}/:/tensorflow-yolo3 -w /tensorflow-yolo3 tensorflow-yolo3:latest-gpu bash
    ```
