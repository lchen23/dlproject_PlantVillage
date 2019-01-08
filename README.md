<img src='plant_image.jpg'>

# A convolutional neural network based plant disease detection system

## Introduction
   Our life depends on plants as much as oxygen. Modern agricultural technologies allow us to grow crops in large quantities to sustain a steady food supply for a growing population in the world. However, plant diseases remain a major threat to this supply by significantly decreasing crop production. The situation is particularly dire for the 500 million smallholder farmers in the world, whose livelihoods depend on the well-being of their crops. 
  
   An early detection of plant disease followed by appropriate treatments can not only protect the infected plant but also prevent the disease from spreading. Usually, this detection or diagnosis is achieved by plant experts with extensive knowledge and practical experience. Moreover, these experts must continuously monitor the plants to avoid disease spreading, an expensive, difficult and time-consuming task for the experts. Automation of the plant diseases detection and identification process for plant protection therefore can create great social benefits as well as economic values.
  
   With the proliferation of smartphones around the globe today, if equipped with advanced computer vision softwares, there is a great opportunity to turn the smartphone into an cost-effective disease diagnostics tool, detecting diseases from cellphone images of plant leaves. This project is built towards reaching this goal.
   
   In the jupyter notebook of this project, I trained a Convolutional Neural Network (CNN) based machine learning model that can detect plant diseases with 99.5% accuracy, using the Pytorch framework and fastai library. To train the model, I use the Plant Village dataset contains plant leaf images of 38 different disease classes and one background class from Stanford's DAGS dataset of background images.
   
   ## Instructions
All the steps for installing and importing required packages (with versions specified), downloading the dataset, training and evaluating the model were described in detail in the jupyter notebook. To reproduce those results, one just need to re-run all the code cells in sequence.

To further improve the model performance, one can try to change the following parameters:
* model architectures : `arch=resnet34` 
* learning rates : `lr=np.array([1e-4,1e-3,1e-2])*0.8`.
* number of training epochs : `learn.fit(lr, 3, cycle_len=2, cycle_mult=2, best_save_name='resnet34_best')`
