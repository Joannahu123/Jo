---
layout: post
title: Big Idea 1.3 - Color Codes/Images/Base64
description:
categories: [Python]
author: Rhea Rajashekhar
---

# 🎨 Understanding Color Codes, Images, and Base64 Encoding

## 📌 Objectives:
By the end of this lesson, students will:
1. Understand how colors are represented using **RGB and Hex codes**.
2. Learn how digital images are stored as grids of pixels.
3. Understand **Base64 encoding** and its use in storing images.

---

## 🎨 1. What Are Color Codes?

### **RGB (Red, Green, Blue)**
Computers display colors using **RGB values**, where each color is a mix of:
- **Red** (`0-255`)
- **Green** (`0-255`)
- **Blue** (`0-255`)

**Examples:**
- `(255, 0, 0)` = 🔴 **Red**
- `(0, 255, 0)` = 🟢 **Green**
- `(0, 0, 255)` = 🔵 **Blue**

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
