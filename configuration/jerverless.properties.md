# jerverless.properties file

This file stores configuration details about your serverless function.

| Property  | Value  | Default
|---|---|---|
| `exec`  | Command which will be executed after the HTTP call. It can be any console command depending on OS. eg: `python myfunction.py param`| empty |
| `port` | The port for exposing the HTTP server endpont | `8080` | 
| `cors` | A boolean value to enable CORS support for all incoming requests. | `false` | 
| `type` | The response type or the `Content-Type` value in the response header | `text/plain` | 

## A sample config file

```
exec = python helloworld.py
port = 8080
cors = true
```
