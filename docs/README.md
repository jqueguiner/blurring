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
curl -X POST "http://MY_SUPER_API_IP:5000/process" -H "accept: image/jpeg" -H "Content-Type: application/json" -d '{"url": "https://i.ibb.co/FqDSQF8/input.jpg", "locations": [{"startY": 700, "endY": 1500, "startX": 2000, "endX": 2600}, {"startY": 1200, "endY": 1900, "startX": 3400, "endX": 4200}]}' --output my_super_blurred_image.png
```
