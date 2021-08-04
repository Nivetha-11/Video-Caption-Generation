# Video-Caption-Generation-

The project's specific  goal  is  to  create  a  prototype  that  automatically  generates  a  caption  that provides a brief description ofthe contents of video frames.Firstly,we aim to pass a video of fourseconds to detect the images' visual and spatial information (video frames) and  generate  set  off image  vectors from  the  Convolution  Neural  Network  (CNN) model.Secondly, text data was prepared by cleaning the description and generating the set of vocabulary.Finally, image vectors obtained from CNN are passed through the Recurrent  Neural  Network  (RNN)and LongShort-TermMemory  (LSTM)to generate a sequence  of meaningful  captions.The ExperimentalResearch Methodology will be carried out in this researchproject. By doing this research, we tend to produce an innovative prototype that helps generate captions, which can be later be used in many real-life applications.
 
 ## Dataset Details:
 
 1)Task Type: Caption Generation
 
 2) Database Link: https://www.csc.kth.se/cvap/actions/
 
 3) Training dataset: 420 videos
 
 4) Validation dataset: 90 videos

 5) Test dataset: 90 videos

 6) The dataset is divided into 70% for training, 15% for testing and 15% for training. 
 
 <img width="675" alt="Screen Shot 2021-08-04 at 4 10 00 pm" src="https://user-images.githubusercontent.com/57209945/128130687-17189844-53bc-423d-8c57-1ff97d28751d.png">
 
 ## Architecture and Model details: 
 
 <img width="896" alt="Screen Shot 2021-08-04 at 4 13 22 pm" src="https://user-images.githubusercontent.com/57209945/128131000-0a47702a-7d00-467f-aef1-63b0caddcb42.png">

##Defining and fitting the model::
    
  The prototypeof our model has been defined bythree differentsections: 
    
   a.Image Feature Extractor: We have designed our prototype with a pre-trained VGG-16 model. Pre-processing of images was done using the VGG-16 model,where the features extracted from the images will be used as an inputto the model.
    
   b.Sequence Processor: This layer focuses on the word embedding layer where we handle text data inputusing LongShort-Term Memory(LSTM) which is incorporated in the recurrent neural network layer.
    
   c.Decoder: Both the output from the Image featureextractor and Sequenceprocessor tends to providea fixed-length vectorwhich isthen combined andprocessed by a dense layer to make final predictions.
    
   <img width="635" alt="Screen Shot 2021-08-04 at 4 17 19 pm" src="https://user-images.githubusercontent.com/57209945/128131378-63ddc50c-393d-4b22-924c-62e90a8c2014.png">
    
   <img width="766" alt="Screen Shot 2021-08-04 at 4 17 39 pm" src="https://user-images.githubusercontent.com/57209945/128131417-f0c7b529-5930-41fa-8ae3-7cce45a96bc4.png">


    

## Code and Impeementation details: 
https://colab.research.google.com/drive/1v7Xt3lRVaODaeDl49wPDOY1oKmb5NcgQ?authuser=3
