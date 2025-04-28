---
layout: post
title: Big Idea 1.3 - Color Codes/Images/Base64
description:
categories: [Python]
author: Rhea Rajashekhar
---
# :lower_left_paintbrush: Understanding Color Codes, Images, and Base64 Encoding
## :pushpin: Objectives:
By the end of this lesson, students will:
1. Understand how colors are represented using **RGB and Hex codes**.
2. Learn how digital images are stored as grids of pixels.
3. Understand **Base64 encoding** and its use in storing images.
---
## :art: 1. What Are Color Codes?
### **RGB (Red, Green, Blue)**
Computers display colors using **RGB values**, where each color is a mix of:
- Red (`0-255`)
- Green (`0-255`)
- Blue (`0-255`)
Example:
- `(255, 0, 0)` = :red_circle: **Red**
- `(0, 255, 0)` = :large_green_circle: **Green**
- `(0, 0, 255)` = :large_blue_circle: **Blue**
Let's visualize RGB values using Python:
```python
import matplotlib.pyplot as plt
import numpy as np
# Define colors
colors = {"Red": (1, 0, 0), "Green": (0, 1, 0), "Blue": (0, 0, 1)}
# Plot colors
fig, ax = plt.subplots(figsize=(6, 2))
for i, (color_name, rgb) in enumerate(colors.items()):
    ax.add_patch(plt.Rectangle((i, 0), 1, 1, color=rgb))
    ax.text(i + 0.5, 0.5, color_name, va="center", ha="center", fontsize=12, color="white")
ax.set_xlim(0, 3)
ax.set_ylim(0, 1)
ax.axis("off")
plt.show()
# Hex Codes
Hex codes are just RGB values written in hexadecimal (base-16).
Example: `#FF0000` = :red_circle: Red, `#00FF00` = :large_green_circle: Green, `#0000FF` = :large_blue_circle: Blue
Try entering an RGB value and converting it to a hex code:
```python
def rgb_to_hex(r, g, b):
    return f"#{r:02X}{g:02X}{b:02X}"
# Example: Convert RGB (128, 0, 128) to hex (Purple)
rgb_to_hex(128, 0, 128)
# :frame_with_picture: 2. How Images Work
Images are grids of pixels, where each pixel has a color.
## :mag: Pixel Grid Example
Let's generate a tiny image to show how pixels work.
```python
import numpy as np
import matplotlib.pyplot as plt
pixel_data = np.array([
    [[255, 0, 0], [0, 255, 0], [0, 0, 255]],  # Row of Red, Green, Blue pixels
    [[255, 255, 0], [0, 255, 255], [255, 0, 255]],  # Row of Yellow, Cyan, Magenta
    [[0, 0, 0], [128, 128, 128], [255, 255, 255]]   # Row of Black, Gray, White
], dtype=np.uint8)
plt.imshow(pixel_data)
plt.axis("off")
plt.show()
# :1234: 3. Base64 Encoding for Images
## What is Base64?
Base64 converts binary data (like images) into text so it can be embedded into websites.
:large_green_circle: **Why use it?** Saves storage and avoids separate image files.
:red_circle: **Downside?** Increases file size.
---
## Convert an Image to Base64
Run this Python script to encode an image:
```python
import base64
# Load an image and convert to Base64
with open("example.png", "rb") as img_file:
    base64_string = base64.b64encode(img_file.read()).decode()
print("Base64 Output (first 100 chars):", base64_string[:100], "...")
# Decode Base64 back into an Image
```python
# Convert Base64 back to an image
img_data = base64.b64decode(base64_string)
# Save the decoded image
with open("decoded_image.png", "wb") as img_file:
    img_file.write(img_data)
print("Image successfully decoded and saved as 'decoded_image.png'")
# :trophy: Final Challenge
Decode this Base64 string and see what it represents:
```makefile
U1NFIEJhc2U2NCBlbmNvZGluZyBpcyB1c2VkIGZvciBzdG9yaW5nIGltYWdlcyBvbiB3ZWJzaXRlcy4=