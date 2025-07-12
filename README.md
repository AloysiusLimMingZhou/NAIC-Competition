# NAIC-Competition

This is the AI Model that we have created to classify different kuih images in Malaysia. The model that we used is Vision Transformer, which is a cutting edge computer vision deep learning model that is able to analyze image more effective than modern Convolution Neural Networks. 

Some of its advantage includes better spatial relationship even with long distance relationship as its multi-head attention mechanism allows it to relate different patches of image. Moreover, the multi-head attention also allows the transformer to analyze all patches of an image simultaneously. 

Some techniques that we've implemented include using AdamW optimizer for better generalization through weight decay and faster convergence. Besides that, we have also used class weights to balance different number of training datasets per class. Furthermore, we have used learning rate scheduler like LambdaLR to slowly increase the value of learning rate from 0 through 5 warmup epochs. The other learning rate scheduler we have used is CosineAnnealingLR that helps decay the value of LR to minimum value over time. Lastly, we have hyperparameter tune our dropout rate, number of epochs, batch_size and implement early stopping to reduce overfitting on our model and determine the best performance for our model's prediction.

Overall, we have tested this model on our own training and testing dataset and the results of accuracy are hovering around 95.62% to 98.12%. The other metrics like precision, recall, F1-Score also fall around this line of values as well.
