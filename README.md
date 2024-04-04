
## GAN-training


To train simply run  `python3 train_loss_gan.py`. For training with different configuration and model simply modify the configuration in train_loss_gan.py

`Trainer = init_train("configs/StyleGAN_256.json",dataloader_train, dataloader_test)`

The main modification to the StyleGAN model can be found in `/EC523_Project_G/notebooks/GAN_anime/losses.py` where we incorporated customized loss function to achieve the goal of our project.

We also modified `/EC523_Project_G/notebooks/GAN_anime/trainer.py` to fit the specific structure of our datasets. 

For debugging purposes we also provided a ipynb file you can find it here `/EC523_Project_G/notebooks/GAN_anime/test_training.ipynb`. 



We also support using scc resources for training GAN model. If you would like to train using scc's GPU simply submit job by running `qsub job.sh`. 

## Credits

This training code was created based on `https://github.com/maximkm/StyleGAN-anime`. We would like to thank Maxim Nikolaev for making the code for GAN models publicly available. If you use would like to use the code in this repository, please cite the original repository.