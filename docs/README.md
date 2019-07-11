# Docker for API

You can build and run the docker using the following process:

Cloning
```console
git clone https://github.com/jqueguiner/blurring.git
```

Building Docker
```console
cd blurring && docker build -t blurring -f Dockerfile .
```

Running Docker
```console
echo "http://$(curl ifconfig.io):5000" && docker run -p 5000:5000 -d blurring
```

Calling the API
```console
curl -X POST "http://MY_SUPER_API_IP:5000/process" -H "accept: image/jpeg" -H "Content-Type: application/json" -d '{"locations":{"startY": 3840, "endY": 1376, "startX": 3378, "endX": 1838}}'
```
