# Image-Cropping-with-Pillow
Crop a region of interest from an image using Pillow
from PIL import Image

image = Image.open('input.jpg')
left, top, right, bottom = 100, 100, 300, 300  # Define the region to crop
cropped_image = image.crop((left, top, right, bottom))

cropped_image.save('output.jpg')
