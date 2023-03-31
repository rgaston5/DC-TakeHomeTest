**Exercise in Lesson 2.3 of the Transformer Architectures Course**

**Learning Objective Assessment:**
    - LWBAT create a class for the cross attention layer in Keras

**Background Context**
We've just created a base class containing the component attention layers, so that each attention layer
can now be implemented as a subclass of this base class - we'll begin with the cross attention layer here in this exercise!

We'll ask you first here to provide the code line to define the CrossAttention block as a subclass of the BaseAttention class, so it inherits everything from the BaseAttention class. Thus every attention layer will include a multi-head attention (mha) block, as well as an add & norm block, as defined in the BaseAttention class.

Remember that in this attention mechanism the query works similarly to a "fuzzy" Python dictionary, where the attention layer looks for the dictionary keys that match the query most closely, and returns the combined values for those keys, with weightings based on how well the query matches each key.


**Instructions**
    - (LEARNER TASK 1) In the first line here, define the CrossAttention layer as a subclass of the BaseAttention class. 
    - (LEARNER TASK 2) Invoke the mha layer with the target sequence x as the query, and the context sequence for both the key and the value. The attention output returned by the mha should be stored for use in the add step below. Set returned_attention_scores to True, and store the attention scores returned for later use.
    - (LEARNER TASK 3) Perform the layer normalization function in the base attention class, using the output of the add step above.
      This should also return the modified tensor, as in the add step. 


```
# Define the CrossAttention class as a subclass of the BaseAttention class.
(LEARNER TASK 1)
  def call(self, x, context):

    # Invoke the mha layer with the target sequence x as the query, and using the context sequence for both the key and the value.
    # Attention outputs from mha are stored for later. 
    (LEARNER TASK 2)

    # Store the attention scores returned from mha for later.
    self.last_attn_scores = attn_scores

    # Perform the add function of the Add & Norm block, aka the residual connection, using the attention outputs from the mha block.
    x = self.add([x, attn_output])

    # Perform the layer normalization function from the base attention class, using the output of the add step above. 
    # This also returns the modified tensor, as in the add step.
    (LEARNER TASK 3)

    # Return the modified tensor
    return x


```