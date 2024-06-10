# HandwrittingAuthorIdentifier

This project aims to identify the user based on the image of the handwritten character. But, identification from different characters may be less straightforward intuitively and require a lot of researches and architecture experimenting.

## Our Approach

We are less confident in constructing a singular neural network computer vision model that is able to identify the writing style of the user given images from different character and users. Hence, we propose a two-step model for the user identification from the input handwritten character image:

1. Identify the character using [Computer Vision](https://www.ibm.com/topics/computer-vision) techniques
2. Identify the user that wrote that character

In our proposed model, our input image will go through the processing stage to convert image into 2d arrays, then recognize the character of that image first, only then identify this character is written by who by comparing it with other user’s image for this character.

## [Soft Computing](https://link.springer.com/journal/500) Techniques

In the mentioned first step, we used neural networks tuned using evolutionary computing methods to classify the images in the dataset into 36 classes, identifying the characters from the range of 0 - 9 and A - Z. Then, in the second step, we will be using 2 different Fuzzy Rule Bases into our Fuzzy System to identify the author for each characters.

In the mentioned second step, we will get the recognized character from the first step, and use it to identify the author of this handwriting. With this, our Fuzzy System will only need to differentiate this image with the other image of the same character by different users.

---

To read more about the project and its report, please refer to [this link](https://github.com/LimJY03/HandwrittingAuthorIdentifier/blob/main/ProjectReport.pdf).
