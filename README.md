# qa-docker
KazanExpress docker images for QA runners etc

Для поддержания актуальных версий внутри ранеров создан данный репозиторий
При изменении версий компонет пересоздается имидж из шаблона  Dockerfile.env путем замены переменных.
На каждый имидж (папку) генерится 2 тэга latest и по номеру сборки.

Для создания имиджа с новым тэгом необходимо сделать папку в /images и положить туда фалы генерации Dockerfile

Алгоритм генерации /.github/workfolws/build-images.yaml


