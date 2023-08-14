# qa-docker
KazanExpress docker images for QA runners etc

Для поддержания актуальных версий внутри ранеров создан данный репозиторий
При изменении версий компонет пересоздается имидж KazanExpress/qa-docker из шаблона  Dockerfile.env путем замены переменных.
На каждый имидж (папку) генерится 2 тэга latest и по номеру сборки.

    ENV_DOCKER_REPO_TAG="$ENV_DOCKER_IMAGE_NAME.$GITHUB_RUN_NUMBER";
    ENV_DOCKER_REPO_TAG_LATEST="$ENV_DOCKER_IMAGE_NAME-latest";
    где ENV_DOCKER_IMAGE_NAME имя папки в images/

kazanexpress/qa-docker:

Для создания имиджа с новым тэгом необходимо сделать папку в images и положить туда фалы генерации Dockerfile

Алгоритм генерации .github/workfolws/build-images.yaml


