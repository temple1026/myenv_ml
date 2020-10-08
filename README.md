# Docker environments for machine learning programs

- My basic settings to run machine learning programs on docker container

# Environment
- Host machine
    - Ubuntu18.04
    - Nvidia driver: 440.100
    - CUDA Version: 10.2
    - Docker: 19.03.6, build 369ce74a3c
    - docker-compose:  version 1.25.0, build 0a186604
- Dockerfiles
    - env-tf: for tensorflow2.3-gpu, tensorboard(port 6006)

    (I will add other settings in advance)

# Run
- Set an environment variable 
    
    ```sh
    > export UID
    ```

    - I wrote UID into ~/.bashrc.

- Run docker-compose
    ```sh
    # Run docker containers
    > docker-compose up -d

    # Enter to the docker container
    > exec -it container_name bash 
    ```

Warning: In docker container, you need to run command ```su current_user_name``` before making some files. Otherwise, the owner of them will be __root__. 
