# cifar100 with keras


While the training loss is decreasing, the validation loss has increased in the 14th epoch
then it has decreased and the gap has widened a little. The epoch they are closest to here is the 5th epoch.

![Screen Shot 2021-08-31 at 12 28 15 AM (1)](https://user-images.githubusercontent.com/7634028/133727323-d8f97b41-a7d2-4aa0-af8a-be51cdd4e97b.png)


Validation accuracy also decreased, but training accuracy was less. There are many local minimums but the network managed to exceed it.

![Screen Shot 2021-08-31 at 12 28 10 AM (1)](https://user-images.githubusercontent.com/7634028/133729249-e87aa00e-12f4-44d2-bde9-6ccb950f9359.png)

# ImageDataGenerator
Zoom_range and harizontal_flip are used for ImageDataGenerator in the model.
zoom_range: Range for random zoom

horizontal_flip: Randomly flip inputs horizontally
In the model, there have been hard ups and downs in the graphics using ImageDataGenerator
val_acc:0.4767 

![Screen Shot 2021-08-31 at 12 28 24 AM](https://user-images.githubusercontent.com/7634028/133729394-771a184d-8aa1-4558-bda4-23814f2f465d.png)


![Screen Shot 2021-08-31 at 12 28 31 AM](https://user-images.githubusercontent.com/7634028/133729429-1ab2eab2-c166-4ce0-97c9-4a7d6f8a457f.png)


# DROPOUT

Two dropouts are used in the model. The first dropout value is 0.15. It is after the 2nd convolution.
The second dropout value is 0.25. It is after the 4th convolution.
Val_acc:0.3100.
well, dropout has increased the success of the network in this model.

![Screen Shot 2021-08-31 at 1 03 05 AM](https://user-images.githubusercontent.com/7634028/133729632-30ddc96e-7cf3-41c7-9767-e8e6e812bca8.png)

The val_acc value of the network has increased without being stuck to the local minimums.

![Screen Shot 2021-08-31 at 1 03 10 AM](https://user-images.githubusercontent.com/7634028/133729690-daa6d867-c02c-40bb-8a08-4b40b8106a6d.png)




