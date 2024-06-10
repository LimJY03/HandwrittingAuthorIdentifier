# HandwritingAuthorIdentifier

This project aims to identify the user based on the image of the handwritten character. However, identification from different characters may be less straightforward intuitively and require a lot of research and architectural experimenting.

## Our Approach

We are less confident in constructing a singular neural network model for [computer vision](https://www.ibm.com/topics/computer-vision) that is able to identify the writing style of the user from images of different characters and users. Hence, we propose a two-step model for the user identification from the input handwritten character image:

1. Identify the character using computer vision techniques
2. Identify the user that wrote that character using feature classification

In our proposed model, our input image will go through the processing stage to convert the image into 2d arrays, then recognize the character of that image first, only then identify who wrote this character by comparing it with other users’ images for this character.

## [Soft Computing](https://link.springer.com/journal/500) Techniques

In the mentioned first step, we used neural networks tuned using [evolutionary computing](https://direct.mit.edu/evco) methods to classify the images in the dataset into 36 classes, identifying the characters from the range of 0 - 9 and A - Z. Then, in the second step, we will be using 2 different Fuzzy Rule Bases in our [Fuzzy System](https://www.mathworks.com/help/fuzzy/what-is-fuzzy-logic.html) to identify the author for each character.

In the mentioned second step, we will get the recognized character from the first step, and use it to identify the author of this handwriting. With this, our Fuzzy System will only need to differentiate this image from the other images of the same character by different users.

---

To read more about the project and its report, please refer to [this link](https://github.com/LimJY03/HandwrittingAuthorIdentifier/blob/main/ProjectReport.pdf).
