**ADNet**
======

## Description
Attention-based DenseNet Architecture is a useful architecture for potentially solving a number of problems in seismology, including but not limited to, seismic data processing, interpolation, imaging, inversion, complex forward/inverse mapping, etc.

Firstly, the multi-dimensional data is divided into several overlapped patches. Secondly, the ADNet network inputs patches to the encoder to extract the significant latent features, while the decoder tries to combine these extracted features for making a decision depending on the purpose. Besides, the SE network is used to scale the extracted features from the encoder and decoder. Thirdly, the SE output of the encoder is concatenated with the SE output of the decoder to obtain high-order features and guide the network to extract the most significant information related to the seismic signals and discard the others. The ADNet was originally used in Saad et al., for seismic data enhancement. There are many other applications to be explored.

## Reference
Saad, Omar M., Yapo Abolé Serge Innocent Oboué, Min Bai, Lotfy Samy, Liuqing Yang, and Yangkang Chen. "Self-attention deep image prior network for unsupervised 3-D seismic data enhancement." IEEE Transactions on Geoscience and Remote Sensing 60 (2021): 1-14.

BibTeX:

        @article{saad2021self,
          title={Self-attention deep image prior network for unsupervised 3-D seismic data enhancement},
          author={Saad, Omar M and Obou{\'e}, Yapo Abol{\'e} Serge Innocent and Bai, Min and Samy, Lotfy and Yang, Liuqing and Chen, Yangkang},
          journal={IEEE Transactions on Geoscience and Remote Sensing},
          volume={60},
          pages={1--14},
          year={2021},
          publisher={IEEE}
        }

-----------
## Example
1- Run Step1 to create the patches.

2- Run Step2 to denoise the 3D noisy data.

3- Run Step3 to read the output patches and reconstruct the data.

4- Run SConstruct using the command "scons view" to plot the results.


-----------
## Copyright
    The ADNet developing team, 2021-present
-----------

## License
    MIT license
    
-----------
## Contact
    Regarding any questions, bugs, developments, collaborations, please contact  
    Yangkang Chen
    chenyk2016@gmail.com


 

