**Rick Gaston - Candidate for Analytics & Data Science Curriculum Specialist position - Take-Home Assignment** 
March 31, 2023

**Course Outline - Transformers**

**Course Learning Objectives:**
    1) LWBAT describe the functions of each key component of the transformer architecture
    2) LWBAT implement a transformer architecture with Tensorflow and Keras
    3) LWBAT train and test a transformer sequence-to-sequence model

Chapter 1 - Components of Transformer Architectures
    Lesson 1.1: Overview of Transformer Architectures
        - Learner will be able to (LWBAT) sketch an overview of a transformer architecture with all key components
        - New functions and terms: Transformer
    Lesson 1.2: Encoder and Decoder Blocks
        - LWBAT describe the functions of encoder and decoder blocks
        - LWBAT create classes in Keras to define an encoder block and a decoder block
        - New functions and terms: Encoder block, decoder block, classes for encoder and decoder blocks in Keras
    Lesson 1.3 Attention Layers
        - LWBAT describe the function of the attention layers
        - New functions and terms: Attention layer

Chapter 2 - Implementing Attention Layers
    Lesson 2.1: How Self-Attention Works
        - LWBAT calculate self-attention using vectors
        - LWBAT use matrices to implement self-attention
        - New functions and terms: Self-attention
    Lesson 2.2: Implement Base Attention Layer
        - LWBAT create a class for the base attention layer in Keras
        - New functions and terms: Class for base attention layer in Keras
    Lesson 2.3: Implement Cross Attention Layer
        - LWBAT create a class for the cross attention layer in Keras 
        - New functions and terms: Class for cross attention layer in Keras
    Lesson 2.4: Implement Global and Causal Self-Attention Layers
        - LWBAT create a class for the global self-attention layer in Keras
        - LWBAT create a class for the causal self-attention layer in Keras
        - New functions and terms: Classes for global and causal self-attention layers in Keras

Chapter 3 - Other Components of Transformer Architectures
    Lesson 3.1: Embedding Layer
        - LWBAT describe the function of the embedding layer
        - LWBAT create a class for the embedding layer in Keras
        - New functions and terms: Class for embedding layer in Keras
    Lesson 3.2: Residual Add & Norm Blocks
        - LWBAT describe the function of the residual add & norm blocks
        - LWBAT create a class for an add & norm block in Keras
        - New functions and terms: Class for add & norm blocks in Keras
    Lesson 3.3: Feed Forward Networks
        - LWBAT describe the function of the feed forward networks
        - LWBAT create a class for the feed forward networks in Keras
        - New functions and terms: Class for feed forward networks in Keras
    Lesson 3.4: Complete Transformer Model
        - LWBAT combine the encoder and decoder blocks, with a final linear layer, to create the transformer
        - New functions and terms: Class for transformer in Keras

Chapter 4 - Training and Evaluating Transformer Sequence-to-Sequence Models
    Lesson 4.1: Set Up Optimizer
        - LWBAT create the Adam optimizer with a custom learning rate scheduler for transformers
    Lesson 4.2: Set Up Loss and Metrics
        - LWBAT apply padding mask and cross-entropy to calculate loss
    Lesson 4.3: Train and Test Model
        - LWBAT train then test model using various text sequences for input and output
    Lesson 4.4: Use and Fine-Tune Pre-trained Transformer Models
        - LWBAT describe benefits of using pre-trained model
        - LWBAT preprocess text data
        - LWBAT select pre-trained model from Hugging Face based on task type
        - LWBAT use Hugging Face Trainer to fine-tune model
        - New functions and terms: Hugging Face Trainer
