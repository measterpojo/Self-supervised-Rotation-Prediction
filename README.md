# Self-supervised-Rotation-Prediction
enable the model to learn meaningful and generalizable visual representations of images without requiring labeled data

Self-supervised learning: refers to a deep learning approach in which a model is initially trained on unlabeled data. During this process, the data generates its own labels, which are then utilized as ground truths in future training iterations.


When you rotate an image by 90 degrees (or any other angle you choose, like 0°, 180°, or 270°), you assign a corresponding label to indicate the applied rotation. For example:

0° rotation → Label: 0

90° rotation → Label: 1

180° rotation → Label: 2

270° rotation → Label: 3

During training, the model learns to predict these labels based on the visual patterns it observes in the rotated images. Here's a simplified step-by-step process:

Apply Rotation:

Rotate the image by a random angle (e.g., 90°).

Assign Label:

Add the corresponding label to the image (e.g., 1 for 90°).

Train the Model:

Use these labeled images (original + rotated) to train a model to predict the rotation angle.

Learn Features:

The model, by solving this rotation prediction task, learns valuable features like edges, orientation, and spatial relationships, which can later transfer to other tasks.
