Demo repo for https://github.com/astral-sh/uv/issues/13490. See https://github.com/astral-sh/uv/issues/13490#issuecomment-2889718521 for details.


```sh
UV_CONFIG_FILE=custom-uv.toml uv add polars
```

```sh
UV_CONFIG_FILE=custom-uv.toml uv sync --refresh --no-cache
```

Polars is retrieved from the default PyPi index, implicitly injected by the presene of a `uv.toml` config file. See `uv.lock`.