# color_converter
1. I used the "color" library to extract the RGB values ​​of a color. Since these values ​​were initially between 0 and 1, I multiplied each component by 255 to bring them to a scale of 0 to 255. Then, to obtain the normalized TSL (Hue, Saturation, Brightness) values, I multiplied the first element by 360 degrees and the other two by 100 to express them as a percentage. I also included the hexadecimal of the color, which I retrieved as a user-supplied variable in the function, and grouped all these values ​​into a dictionary.

2. Then I displayed the result of this function.

3. As for converting from hex to RGB, I then transformed the RGB to HSV (Hue, Saturation, Value) color space. I added 180 degrees to the hue value (the first element in that space, with values ​​ranging from 0 to 1) to get the complementary color. Then I took the other two values ​​from the HSV and converted them to hexadecimal using the "color" library.
