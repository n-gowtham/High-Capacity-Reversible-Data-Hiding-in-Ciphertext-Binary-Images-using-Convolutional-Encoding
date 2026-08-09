# High-Capacity-Reversible-Data-Hiding-in-Ciphertext-Binary-Images-using-Convolutional-Encoding

## Block Diagram
![image alt](https://github.com/n-gowtham/High-Capacity-Reversible-Data-Hiding-using-Convolutional-Encoding/blob/master/BlockDiagram.png)

## Description 
- Most of the Reversible Data Hiding (RDH) methods focus on grayscale or color images. But, binary images play an important role, such as digital signature and scanned confidential documents.
- Existing RDH methods for Binary Images are designed by exploiting histogram shifting, low-frequency patterns, visual cryptography etc.
- This project proposes a novel method of encoding/decoding marked ciphertext binary images which has following advantages:
    - The method is independent of image composition (does not depend on density / sparseness)
    - 100% recoverability is achieved (exact binary image can be re-constructed)
    - The embedding rate can be increased, up to a maximum limit determined by the dimensions of the encrypted image.
    - Provides flexibility against error correction if received images are noisy. 

## Code and Results
- Provided a framework where binary(/grayscale) image, secret text are taken as inputs and encoded image is produced (from block diagram). Then, viterbi decoder along with decryption is used at the receiver to recover the binary image and secret text.
- The results of the code are already saved inside the jupyter notebook named 'HighCapacityConvolutionalEncoder.ipynb'.
- Embedding rate of **87.5%** is achieved using 15:16 convolutional encoder. (which surpasses many algorithms in literature, refer to Fig.3 in https://ieeexplore.ieee.org/document/10947549)

## Key Learnings
- Implemented Otsu's thresholding algorithm to convert from grayscale image to binary image.
- Implemented Convolutional Encoding (along with puncture pattern) and Viterbi decoder in python.
