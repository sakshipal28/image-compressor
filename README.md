# image-compressor
Python script to compress and convert images to JPG

from PIL import Image

# Replace with your actual file name
input_image = "photo.jpg"
output_image = "compressed_image.jpg"

# Open and convert to RGB
img = Image.open(input_image).convert("RGB")

# Save with compression
img.save(output_image, "JPEG", optimize=True, quality=50)

print("✅ Converted and compressed image saved as:", output_image)




