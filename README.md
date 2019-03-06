# reactjsavatarpreview
Facebook like, avatar / profile picture component. Resize, crop and rotate your uploaded image using a clear user interface.


https://reactjsexample.com/content/images/2017/09/Facebook-like.gif

Live Demo
https://react-avatar-editor.netlify.com/



Usage
import React from 'react'
import AvatarEditor from 'react-avatar-editor'

class MyEditor extends React.Component {
  render () {
    return (
      <AvatarEditor
        image="http://example.com/initialimage.jpg"
        width={250}
        height={250}
        border={50}
        color={[255, 255, 255, 0.6]} // RGBA
        scale={1.2}
        rotate={0}
      />
    )
  }
}

export default MyEditor



Accessing the cropping rectangle
Sometimes you will need to get the cropping rectangle (the coordinates of the area of the image to keep),
for example in case you intend to perform the actual cropping server-side.

getCroppingRect() returns an object with four properties: x, y, width and height;
all relative to the image size (that is, comprised between 0 and 1). It is a method of AvatarEditor elements,
like getImage().
