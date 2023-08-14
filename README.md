# qa-docker
KazanExpress docker images for QA runners etc

To maintain up-to-date versions inside the runners, this repository was created
When changing component versions, the KazanExpress/qa-docker image is recreated from the Dockerfile.env template by replacing variables.
For each image (folder), 2 latest tags are generated and by build number.

    ENV_DOCKER_REPO_TAG="$ENV_DOCKER_IMAGE_NAME.$GITHUB_RUN_NUMBER";
    ENV_DOCKER_REPO_TAG_LATEST="$ENV_DOCKER_IMAGE_NAME-latest";
    где ENV_DOCKER_IMAGE_NAME folder name in images/

kazanexpress/qa-docker:

To create an image with a new tag, you need to make a folder in images and put the Dockerfile generation files there

Generation algorithm .github/workfolws/build-images.yaml


