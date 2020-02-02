# Nike Meme Generator

This little app uses PHP for file upload. The details are similar to the repository in [Asynchronous File Upload](https://github.com/teochewthunder/asynchronous-file-upload), except that we also include something to ascertain that the file uploaded is a valid image file.

The CSS is interpersed with PHP code variables which will use:
- *colinkaepernick.jpg* as the default image background
- **"Believe in something."** as the default first line.
- **"Even if it means sacrficing everything."** as the second line.
- **"Just Do It."** as the slogan.

Upon a POST, the form gets the new first line, second line and slogan. Then it processes the image file and stores it in the *uploads* directory. The div, id *memeContainer* will render the image in grayscale and position the words within.

*Note*
This does not work in Safari's earlier versions. While the upload performs just fine. the image is not rendered in grayscale.

## Fix
Added a div with a translucent black background to increase contrast.
