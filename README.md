# myClock
![image](https://user-images.githubusercontent.com/34626538/111064134-4b71fb80-84aa-11eb-9fa6-2053ed961670.png)

Everyone knows what a clock is so this is just a simple piece using basic HTML, CSS and simple JS. The usage of this clock is pretty simple: just measuring and displaying the time with clock hands.  

Main Concepts

HTML
For this piece, I have used Div to apply CSS using classes and JS using id

CSS
Properties highlighted for this piece:
Box-shadow: It adds shadows around the element and the achievement to an inner shadow within the clock is given by the inset value.

::before selector: this property is used to insert something before the content. In this piece, the content property is used with empty strings due it is not necessary adding any content.

Z-index: the dot has to be brought to the front so this property will bring it adding a positive value. 

JavaScript
document.querySelector(): this method is used to return the element with the id specified. In this case, it will return the id for ‘hour’, ‘minute’, ‘second’. 

setInterval(): this method is part of the timing events (setTimeout & setInterval). This method repeats a given function at every given time-interval. 

newDate(): this method will be defined into the function mentioned above. Within the function, a variable will be declared equal to newDate() so it will allow returning hours, minutes and seconds: variable.getHours(), variable.getMinutes(), variable.getSeconds()

Also, hours will be multiplicated by 30 because 360 for hands rotation / 30 = 12 (hr) and minutes & seconds 360 / 6 = 60 (mins & secs).

Style.transform: it’s used to rotate hours, minutes and seconds and they'll be equal using ‘rotateZ’ into a  template literals. Therefore, it will allow the hands clock to rotate around the z-axis without deforming it.
 
In addition, hours, minutes and seconds will embed expressions into the string literal. 
