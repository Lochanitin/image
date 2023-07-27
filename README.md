# image
pip V
pip install opencv-python
import cv2
my_image = cv2.imread("cat-551554_640.jpg")
my_image.shape
SHow_image method
def show_image(image):
    cv2.imshow('Image Window',image)
    cv2.waitKey(0)
    cv2.destroyAllWindows()
    show_image(my_image)
    Invert the grey scale image
inverted_image = 255 - grey_image
show_image(inverted_image)
inverted_image = 255 - grey_image
show_image(inverted_image)
Blur the inverted Image
blurred = cv2.GaussianBlur(inverted_image, (21, 21), 0)
inverted_blurred = 255 - blurred
show_image(inverted_blurred)
pencil SKetch
pencil_sketch = cv2.divide(grey_image, inverted_blurred, scale = 256.0)
show_image(pencil_sketch)
cv2.imshow("Original Image",my_image)
cv2.imshow("Pencil Sketch",pencil_sketch)
cv2.waitKey(0)
-1
