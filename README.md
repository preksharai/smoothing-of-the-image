# smoothing-of-the-image
import numpy
import cv2
img = cv2.imread('03a294eb67326695d85c459a555654b1(1).jpg')
blur1 = cv2.GaussianBlur(img,(5,5),0)
blur2 = cv2.blur(img,(5,5))
blur3 = cv2.medianBlur(img,5)
cv2.imshow('image',blur3)
cv2.imshow('original',img)
cv2.waitKey(0)
cv2.destroyAllWindows()

