# faiss_docker
Docker container for Faiss https://github.com/facebookresearch/faiss

### build
docker build . -t faiss

### Run
docker run -it -p 8000:8000 -v ~/Documents:/Documents --name faiss faiss (CPU)
nvidia-docker run -it -p 8000:8000 -v ~/Documents:/Documents --name faiss faiss (GPU)

### SSH to the container
docker exec -it faiss bash (CPU)
nvidia-docker exec -it faiss bash (CPU)