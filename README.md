# Multi_API_Handler_Routes

- This lib allows you to manage multiple APIs, as well as routing logic for directing requests to the appropriate endpoints.

## install with Poetry

```bash
poetry add git+https://github.com/Vortex5Root/Multi_API_Handler_Routes.git
```

# Usage

```python
from fastapi import FastAPI

from muilt_api_handler_routes.Routes.Configs  import ConfigsModel
from muilt_api_handler_routes.Routes.Skeleton import Skeleton

app = FastAPI()

app.include_router(Wallet(),    prefix="/v1/muiltapi")
app.include_router(ConfigModel(),  prefix="/v1/muiltapi")
app.include_router(Skeletons(),    prefix="/v1/muiltapi")
app.include_router(Virtual_Bound(),    prefix="/v1/muiltapi")
```


## Conclusion
The Library is used to manage multiple APIs, as well as routing logic for directing requests to the appropriate endpoints.

## License
[![MIT](icons/license40.png)](https://choosealicense.com/licenses/mit/)
