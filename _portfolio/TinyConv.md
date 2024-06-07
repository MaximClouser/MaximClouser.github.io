---
title: "Tiny but Mighty: Leveraging Pruning and Quantization in Audio
Neural Networks for Compact Device Efficiency"
excerpt: "Optimized a TinyConv FP32 Neural Network for audio processing, applying quantization and pruning for efficient MCU deployment to analyze the effects on model accuracy. <br/><img src='/images/TinyConv.png' width='350px'>"
collection: portfolio
---
*Completed during my ML Hardware and Systems course, Spring 2024*  

### Overview  
This study demonstrates the training and deployment of an audio processing neural network, TinyConv, on an Arduino Tiny Machine Learning Kit, focusing on efficient model operation in constrained environments. The process encompassed six main stages: preprocessing, model size estimation, training, model conversion, quantization, and pruning. Initially, audio was preprocessed to enhance neural network performance through techniques like Fast Fourier Transforms and Mel Spectrograms, aiding in effective feature extraction from audio signals.

The TinyConv model was optimized for microcontroller use and underwent quantization and pruning to reduce size and computational needs without significantly sacrificing accuracy. Two key techniques—quantization-aware training and pruning (both structured and unstructured)—were applied, enhancing the model's performance under limited computational resources.

In practical tests, the model demonstrated high accuracy in recognizing specific audio commands ("yes" and "no"), though it struggled with similar sounding words. Structured pruning allowed for considerable reduction in computational demands with a manageable decrease in accuracy, showing potential for deployment in scenarios requiring rapid response and minimal resource use. This project illustrates the balance between performance, efficiency, and accuracy, highlighting the potential of neural networks in embedded systems.

### Report and Code 
[View the full project code on GitHub](https://github.com/MaximClouser/ML-Hardware-and-Systems/tree/main/A2). 
<iframe src="/files/TinyConv.pdf" width="100%" height="500px">
    Sorry, your browser does not support PDFs. <a href="/files/TinyConv.pdf">Download PDF</a>
</iframe>