Deep learning (DL) techniques are increasingly being utilized in MRI processing, showing significant effectiveness in tasks such as image reconstruction, segmentation, and super-resolution. These methods leverage large datasets and advanced algorithms to predict and mitigate electromagnetic interference (EMI). By learning complex patterns of interference, DL models can adaptively filter out noise, providing a flexible and scalable approach to EMI elimination. However, supervised learning, which is commonly applied for ULF MRI EMI reduction, has some notable drawbacks. It typically requires a substantial amount of ground truth data for training and is highly sensitive to domain shift issues, where the model's performance degrades when applied to data from different distributions. 


This project (named SUPERCLEAN) proposed a novel self supervised learning technique that addresses these challenges. 
This approach aims to reduce the dependency on large training datasets and improve robustness against domain shifts, 
ensuring more reliable EMI mitigation in ULF MRI systems. 
![low field scanner](./scanner.jpeg) 


Neural networks trained on extensive MRI data, 
including both nuclear magnetic resonance (NMR) signals and EMI signatures, can accurately distinguish between true MRI signals and interference, 
thereby enhancing the quality of MRI images. The following figure is the network architecture of SUPERCLEAN.

![Model Framwork](./SUPERCLEAN-framework.png)  

The following images shows the noise suppression results comparing to original images and images after reconstruction pipeline.
![Alt 1](./ML_Denoising_RS027.png)  ![Alt 2](./ML_Denoising_RS052.png)  ![Alt 3](./ML_Denoising_RS067.png) 
![Alt 1](./ML_Denoising_RS073.png)  ![Alt 2](./ML_Denoising_RS075.png)  ![Alt 3](./ML_Denoising_RS076.png) 
![Alt 2](./SUPERCLEAN_RS027.png)  ![Alt 3](./SUPERCLEAN_RS052.png) ![Alt 3](./phantom.png) 
