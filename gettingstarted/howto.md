## On Machine (or VM)

1. Download **jar**
```
 $ curl --ssl -L https://github.com/jerverless/jerverless/releases/download/v0.1.0/org.jerverless-0.1.0.jar > jerverless.jar
```

2. Create `jerverless.properties`
```
exec = python helloworld.py
port = 8080
cors = true
```
3. Create your program (eg:- `helloworld.py`)

```python
name = raw_input()
print "Hello %s!" % name
```
4. Start server!

```
 $ java -jar org.jerverless-0.1.0.jar 
```

5. Test it!

```
 $ curl -d Jerverless http://localhost:8080/function
```

Or simply use [template](https://github.com/jerverless/jerverless/examples) and jump to last step! 

## Docker

1. On your local machine, clone this repo and go to an examples directory of choice (eg: python): 

```
 $ git clone https://github.com/jerverless/jerverless.git
 $ cd jerverless/examples/python
```

2. Create the docker image:

```
 $ docker build --no-cache -t jerverless-py .
```

3. Run the app:

```
 $ docker run -it -p 8080:8080 jerverless-py
```

4. Navigate to 'https://localhost:8080/function' in your browser.

## Kubernetes

1. Create docker image for your function and push to dockerhub

2. Add docker image name to `.yml` deployment

