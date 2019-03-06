# reactjsavatarpreview
Facebook like, avatar / profile picture component. Resize, crop and rotate your uploaded image using a clear user interface.


https://reactjsexample.com/content/images/2017/09/Facebook-like.gif

Live Demo
https://react-avatar-editor.netlify.com/



Accessing the cropping rectangle
Sometimes you will need to get the cropping rectangle (the coordinates of the area of the image to keep),
for example in case you intend to perform the actual cropping server-side.

getCroppingRect() returns an object with four properties: x, y, width and height;
all relative to the image size (that is, comprised between 0 and 1). It is a method of AvatarEditor elements,
like getImage().
