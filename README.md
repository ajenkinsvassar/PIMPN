# PIMPN
Python Integrated Miniscope Pipeline Notebook

Version: 0.8.1

This Colab Notebook has been designed to analyze calcium imaging and behavior videos directly on the cloud. It relies on a Dropbox API, CaImAn, which itself uses NormCorre for motion correction as well as Constrained Non-Negative Matrix Factorization (CNMF/CNMFE) for source extraction. Behavior video can be analyzed automatically using DeepLabCut and your own DeepPose model (currently working on making pre-trained models available).

Features
Fully automatic and unsupervised: once you found parameters that work well for your conditions, and trained deep learning models that suit your data (pre-trained models also available), you can run your analyzes in one click
Tailored for miniscope data: Registers miniscope timestamps and informations about your experiment (subject name, date of experiment), dedicated to multiple .avi files although works with other formats (hdf5, tiff).
Cloud based: Google Colab will temporarily allocate a virtual machine to perform the analysis job. No need to download data on your local computer, and save computing for other tasks! Analyzed data is transfered back to your cloud server.
Compatibility: the data generated by the analysis can be saved in a matlab file that is compatible with MiniscopeAnalysis, but also hdf5 files that can be organized the way you like.
DISCLAIMER PIMPIN relies on a powerful Dropbox API that allows to interact with your cloud repositories (dowload, upload, list or remove files). While it is design to facilitate access, downloads and uploads, beware of misuses. If you plan on sharing this notebook, do not forget to remove your Dropbox access token unless you wish to grant access to your data. You can also enter your gmail credentials to get notified when your analysis is done. Here again, don't forget to remove this info when sharing the notebook.

If you don't have a trained DLC model, here is a simple one trained on a black mouse, top view: https://www.dropbox.com/s/03k7w4kn1lys9m2/DeepLabCut.zip?dl=0 (UPDATED LINK)
The zip file also contains the training videos. These will be removed in the future to make the file lighter.

Copyright © Guillaume Etter 2019

This program is free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or any later version.

Contact: etterguillaume@gmail.com
