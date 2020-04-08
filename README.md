The Image Blurring API will help you blur multiple parts of the image of the provided picture.

Providing the image url as well as the location to blur to the API will returns the the picture with an image partly blurred.

- - -
EXAMPLE
![output](https://i.ibb.co/jb7xjH9/output.png)
- - -
INPUT

```json
{
  "url": "https://i.ibb.co/FqDSQF8/input.jpg",
  "locations": [
    {
      "startY": 700,
      "endY": 1500,
      "startX": 2000,
      "endX": 2600
    },
    {
      "startY": 1200,
      "endY": 1900,
      "startX": 3400,
      "endX": 4200
    }
  ]
}
```
- - -
EXECUTION
```bash
curl -X POST "https://api-market-place.ai.ovh.net/image-car-classification/detect" -H "accept: image/png" -H "X-OVH-Api-Key: XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX" -H "Content-Type: application/json" -d '{"url": "https://i.ibb.co/FqDSQF8/input.jpg", "locations": [{"startY": 700, "endY": 1500, "startX": 2000, "endX": 2600}, {"startY": 1200, "endY": 1900, "startX": 3400, "endX": 4200}]}' --output my_super_blurred_image.png
```
- - -

OUTPUT
Binary output png image

![output](https://i.ibb.co/pJ4tBQH/my-super-blurred-image.jpg)

---
please refer to swagger documentation for further technical details: [swagger documentation](https://market-place.ai.ovh.net/#!/apis/d6b58c18-c04c-40c8-b58c-18c04c00c806/pages/44924656-8f5f-4cc9-9246-568f5fccc96d)

* * *
<div>Icons made by <a href="https://www.flaticon.com/authors/smashicons" title="Smashicons">Smashicons</a> from <a href="https://www.flaticon.com/"                 title="Flaticon">www.flaticon.com</a> is licensed by <a href="http://creativecommons.org/licenses/by/3.0/"                 title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a></div>
