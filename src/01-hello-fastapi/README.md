## Run the live server

`$ uvicorn src.01-hello-fastapi.main:app --reload`

- `--reload`: make the server restart after code changes

## Available URLs
- [http://127.0.0.1:8000](http://127.0.0.1:8000): `root`'s message
- [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs): Docs
- [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc): API Docs
- [http://127.0.0.1:8000/items/any-string](http://127.0.0.1:8000/items/any-string): Return any-string
    - Note: The data validation is performed under the hood by [Pydantic](https://pydantic-docs.helpmanual.io/).
- [http://127.0.0.1:8000/models/model-name](http://127.0.0.1:8000/models/resnet): Model names in Enum only valid
    - See documentation
