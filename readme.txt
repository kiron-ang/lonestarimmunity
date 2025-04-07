Hi, Dr. Wilkerson!

Attached are two PNG files, one for digital viewing and one for print viewing. The colors for the digital image were derived from the primary color palette of the Texas Department of Transportation: https://www.txdot.gov/about/brand-guidelines/visual-identity/colors.html. The specific HEX codes for blue, white, and red result in a palette that should remain comprehensible to human viewers with different optical conditions. Additionally, I also followed the Department's recommendation that red only be used as an accent; white and blue take up the majority of the plot.

To create a print-friendly version, I first tried converting the image to grayscale using opencv-python:

import cv2
image = cv2.imread("digital-viewing.png"))
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
cv2.imwrite("print-viewing.png", gray_image)

However, I was not satisfied, because it was difficult to distinguish the colors. So, my final image for print viewing was derived by extracting only the green channel from the image:

import cv2
image = cv2.imread("digital-viewing.png")
green_channel = image[:, :, 1] 
cv2.imwrite("print-viewing.png", green_channel)

Note that "0" is blue, "1" is green, and "2" is red. I believe this is the most appropriate filter because the three colors are distinct in this gray version, similar to the colors in the version for digital viewing. Thank you for your time and evaluation.

Sincerely,

Kiron Ang
