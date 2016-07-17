# ColourPicker

Generate a HSV Colour Wheel


After some thought it turns out that the wheel can be generated via 

point(x,y).setColor(HSV(getAngle(circle_center, point) / 360, getVectorDistance(circle_center, point) / circle_radius), 1)

![full ColourWheel](https://github.com/Cyberia--/ColourPicker/blob/master/Images/finishedColourBall.png)

After some experimentation, nice effects can be generated by modifying the saturation value

s = getVectorDistance(circle_center, point) 

![full ColourWheel](https://github.com/Cyberia--/ColourPicker/blob/master/Images/HSV_2.png)

s = getVectorDistance(circle_center, point) / circle.x - circle.y

![full ColourWheel](https://github.com/Cyberia--/ColourPicker/blob/master/Images/HSV_1.png)

s = getVectorDistance(circle_center, point) / 0.000001f // or any really small value

![full ColourWheel](https://github.com/Cyberia--/ColourPicker/blob/master/Images/HSV_3.png)
