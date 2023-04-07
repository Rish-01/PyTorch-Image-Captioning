# PyTorch-Image-Captioning :camera: :pen:

This project uses a ResNet152 convolutional neural network (CNN) as an encoder and a long short-term memory (LSTM) recurrent neural network as a decoder to generate captions for images. The model is trained on the Microsoft Common Objects in Context (MS COCO) dataset.

## Architecture

The encoder consists of a ResNet152 CNN followed by a linear layer and batch normalization. The CNN is pretrained on the ImageNet dataset, and its final fully connected layer is removed.

The decoder consists of an LSTM network followed by a linear layer to generate the final output. The LSTM takes the encoded image features from the encoder and a sequence of previously generated words as input to predict the next word in the caption.

## :clipboard: To-Do List
- [x] Read papers on Image Captioning (ongoing)
- [ ] Define a custom Dataloader for MS COCO dataset
- [ ] Build the LSTM decoder
- [ ] Build the Training loop
- [ ] Evaluate the Model
