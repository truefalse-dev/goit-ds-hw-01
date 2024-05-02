cd app

# Task 1
poetry install

# Task 2
docker build -t app .
docker run -it app /bin/bash