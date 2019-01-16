# jerverless.properties file

This file stores configuration details about your serverless function.

| Property  | Value  | Default
|---|---|---|
| `/<context>`  | Command which will be executed after the HTTP call. It can be any console command depending on OS. eg: `python myfunction.py param`. `<context>` should always begin with the character `/`. For an instance, `/foo = <command>` will be triggered with an incoming request to `http://localhost:8080/foo` | null |
| `port` | The port for exposing the HTTP server endpont | `8080` | 
| `cors` | A boolean value to enable CORS support for all incoming requests. | `false` | 
| `type` | The response type or the `Content-Type` value in the response header | `text/plain` | 

## A sample config file

```
/function1 = python helloworld.py
/function2 = python helloworld.py --param
port = 8080
cors = true
```
