---
title: "Dynamic, Contrast-Enhanced, Abdominal MR Image Reconstruction (2020-2021)"
description: "Learning the Regularization in DCE-MR Image Reconstruction for Functional Imaging of Kidneys."
---

I was the lead developer of the open source reconstruction library PyGRASP, designing the core structure for temporally regularized iterative compressed sensing reconstruction of DCE-MRI using golden-angle radial k-space sampling. After my postdoc, my amazing lab at Boston Children’s Hospital and Harvard Medical School did a tremendous job—cleaning up, containerizing, and publicly releasing the library—making the Python-based PyGRASP package accessible and easy to deploy with fast, high-quality dynamic MRI reconstruction using PyTorch. [[GitHub]](https://github.com/quin-med-harvard-edu/pyGRASP/)

I developed regularization learning project end-to-end, introducing a physiologically inspired, low-dimensional representation combined with a Deep Image Prior (DIP)-based reconstruction method to recover dynamic MRI sequences from radially under-sampled k-space data. Implemented entirely in Python using PyTorch, the approach outperforms traditional compressed sensing techniques like GRASP and NUFT by preserving temporal features in the aorta and kidney regions, enhancing image quality, and improving kidney filtration rate estimation—all without the need for large supervised training datasets. [[Github]](http://github.com/quin-med-harvard-edu/kidney-LR-DCEMRI/)

![Kidney Rec](/files/proj_1/kidney.gif)
---
![Aorta Rec](/files/proj_1/aorta.gif)
**Figure:** Top and bottom rows show reconstructions of aorta and kidney slices, respectively. The first column displays deep-image-prior results, while columns 2–6 show temporal TV-regularized compressed sensing reconstructions with increasing regularization. 

