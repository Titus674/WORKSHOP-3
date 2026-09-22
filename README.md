# Canny Edge Detection

Sturdy Canny Edge Detectionis a fun project that adds sunglasses to photos using image processing.

Welcome to Sturdy Octo Disco, a fun and creative project designed to overlay sunglasses on individual passport photos! This repository demonstrates how to use image processing techniques to create a playful transformation, making ordinary photos look extraordinary. Whether you're a beginner exploring computer vision or just looking for a quirky project to try, this is for you!

## Features:
- Detects the face in an image.
- Places a stylish sunglass overlay perfectly on the face.
- Works seamlessly with individual passport-size photos.
- Customizable for different sunglasses styles or photo types.

## Technologies Used:

Python
OpenCV for image processing
Numpy for array manipulations
## How to Use:
1. Clone this repository.
2. Add your passport-sized photo to the `images` folder.
3. Run the script to see your "cool" transformation!

## Applications:
- Learning basic image processing techniques.
- Adding flair to your photos for fun.
- Practicing computer vision workflows.

## program
```

import cv2
import matplotlib.pyplot as plt
img = cv2.imread("ws03.jpg")
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
edges = cv2.Canny(gray, 100, 200)
plt.figure(figsize=(10, 5))
plt.subplot(1, 2, 1)
plt.imshow(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
plt.title("Original Image")
plt.axis("off")
plt.subplot(1, 2, 2)
plt.imshow(edges, cmap="gray")
plt.title("Canny Edges")
plt.axis("off")
plt.show()

import cv2
import matplotlib.pyplot as plt
img = cv2.imread("ws03.jpg")
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
edges = cv2.Canny(gray, 100, 200)
plt.imshow(edges, cmap="gray")
plt.title("Detected Edges using Canny Algorithm")
plt.axis("off")
plt.show()

import cv2
import matplotlib.pyplot as plt
img = cv2.imread("ws03.jpg")
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
edges1 = cv2.Canny(gray, 50, 100)
edges2 = cv2.Canny(gray, 100, 200)
edges3 = cv2.Canny(gray, 150, 300)
plt.figure(figsize=(12, 8))
plt.subplot(2, 2, 1)
plt.imshow(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
plt.title("Original Image")
plt.axis("off")
plt.subplot(2, 2, 2)
plt.imshow(edges1, cmap="gray")
plt.title("Canny: 50, 100")
plt.axis("off")
plt.subplot(2, 2, 3)
plt.imshow(edges2, cmap="gray")
plt.title("Canny: 100, 200")
plt.axis("off")
plt.subplot(2, 2, 4)
plt.imshow(edges3, cmap="gray")
plt.title("Canny: 150, 300")
plt.axis("off")
plt.tight_layout()
plt.show()


```

### output:

<img width="1008" height="303" alt="image" src="https://github.com/user-attachments/assets/3b7926d2-9966-4e01-8f13-2e08307b3faa" />



<img width="717" height="413" alt="image" src="https://github.com/user-attachments/assets/5f7293d7-df74-4bce-acfd-e25e0a5ae875" />


<img width="1386" height="873" alt="image" src="https://github.com/user-attachments/assets/4ee9f0bf-9786-4fac-b830-fc7f1b609a72" />



## result:
successfully runned.
