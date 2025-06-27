# CDSA
CDSA - Effective Sparse Tracking with Convolution-based Discriminative Sparse Appearance Model
Hi! You are welcome to visit here! This repository is used to release the code of a novel sparse tracking method called the Convolution-based Discriminative Sparse Appearance Model (CDSA), which has been submitted to the Journal of Visual Communication and Image Representation (JVCIR).

To address the limitations of existing sparse appearance models, we introduces a novel Convolution-based Discriminative Sparse Appearance (CDSA) model that exploits the hierarchical layout information and discriminative information of useful local patches for effective sparse tracking. In the CDSA model, we first sample a set of foreground and background local patches from within and around the tracking target region to construct a Discriminative Sparse Dictionary (DSD). By imposing sparsity constraints on these local patches, the learned dictionary not only highlights the differences among foreground patches but also emphasizes the distinctions between foreground and background patches. Each basis vector of the dictionary is then used as a sparse filter to convolve the input image, capturing the hierarchical layout information of relevant foreground patches. Finally, the results of all convolutions are combined to produce the hierarchical features of the tracking target. Additionally, based on the proposed CDSA model, we develop a CDSA-based sparse tracking algorithm within the particle filter framework to achieve effective sparse tracking. To evaluate the performance of our proposed method, extensive experiments have been conducted on two widely used datasets. The results demonstrate that the CDSA-based sparse tracking algorithm is more effective than existing sparse trackers in dealing with external interference. 

# Experimental Datasets
* **Online Tracking Benchmark (OTB)** [1]. (http://cvlab.hanyang.ac.kr/tracker_benchmark/index.html). The OTB100 dataset contains 100 fully sequences annotated by 11 challenging factors, including background clutter, deformation, illumination variation, low resolution, motion blur, fast motion, out-of-plane rotation, occlusion, in-plane rotation, out-of-view and scale variation issues.

* **Unmanned Aerial Vehicle tracking benchmark (UAV123@10_fps)** [2]. (https://cemse.kaust.edu.sa/ivul/uav123). The UAV123@10_fps dataset is a tracking benchmark for lowaltitude unmanned aerial vehicle (UAV) target tracking, and each sequence is annotated by 12 attributes, including aspect ratio change, background clutter, camera motion, fast motion, full occlusion, illumination variation, low resolution, out-ofview, partial occlusion, similar object, scale variation, and viewpoint change.
 
References:

[1] Yi Wu, Jongwoo Lim, Ming-Hsuan Yang: Object Tracking Benchmark. IEEE Trans. Pattern Anal. Mach. Intell. 37(9): 1834-1848 (2015). https://doi.org/10.1109/TPAMI.2014.2388226

[2] Matthias Mueller, Neil Smith, Bernard Ghanem: A Benchmark and Simulator for UAV Tracking. ECCV (1) 2016: 445-461. https://doi.org/10.1007/978-3-319-46448-0_27


# Quick start
Download the two datasets above (including all sequences) and the toolkit, place the entire CDSA folder and downloaded sequences in the specified directory (see the toolkit instructions for details), and run the toolkit.
