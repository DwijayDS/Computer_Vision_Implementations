# Finding dominant Colors In and Image

## K-Means

K-Means can efficiently differentiate colors (Implement color segmentation) and with advanced methods K-Means is highly efficient. But, K-Means being a machine learning algorithm, it  may not be deterministic (We might not get correct result everytime). To make K-means more deterministic, we run K_means multiple times, but this leads to increased runtime.
    
The leftmost image shown following is the original image  and the following images were reconstructed using number of colors equal to 1, 2, 3, 4, 5, 6, 7 and 8 respectively.
    
<p float="left">
<img src="./K_means_color_segmentation/batman.png" width="100" height="100" title="Original Image" />
<img src="./K_means_color_segmentation/Result_images/1_Colors_batman.png" width="100" height="100" title="1 Color" />
<img src="./K_means_color_segmentation/Result_images/2_Colors_batman.png" width="100" height="100" title="2 Color" />
<img src="./K_means_color_segmentation/Result_images/3_Colors_batman.png" width="100" height="100" title="3 Color" />
<img src="./K_means_color_segmentation/Result_images/4_Colors_batman.png" width="100" height="100" title="4 Color" />
<img src="./K_means_color_segmentation/Result_images/5_Colors_batman.png" width="100" height="100" title="5 Color" />
<img src="./K_means_color_segmentation/Result_images/6_Colors_batman.png" width="100" height="100" title="6 Color" />
<img src="./K_means_color_segmentation/Result_images/7_Colors_batman.png" width="100" height="100" title="7 Color" />
<img src="./K_means_color_segmentation/Result_images/8_Colors_batman.png" width="100" height="100" title="8 Color" />
</p
    
    
K-means is the fastest and efficient way to implement color segmentation when the difference between total number of colors in images and number of clusters in k_means is small. As this difference increases, Kmeans become less and less efficient. The Kmeans model was trained using random 1000 samples from the image and the amount of data used would also affect the performance. To improve the performance of Kmeans, we can use better clustering algorithms like GMM. Further we go on to implement GM and Heirarchical clustering using Eigenvectors.



## Gaussian Mixture Models

Lets try a probabilitic clustering approach and see how it works. we implement GMM and the results are shown below

The leftmost image shown following is the original image  and the following images were reconstructed using number of colors equal to 1, 2, 3, 4, 5, 6, 7 and 8 respectively.
    
<p float="left">
<img src="./K_means_color_segmentation/batman.png" width="100" height="100" title="Original Image" />
<img src="./GMM_color_segmentation/Result_images/1_Colors_batman.png" width="100" height="100" title="1 Color" />
<img src="./GMM_color_segmentation/Result_images/2_Colors_batman.png" width="100" height="100" title="2 Color" />
<img src="./GMM_color_segmentation/Result_images/3_Colors_batman.png" width="100" height="100" title="3 Color" />
<img src="./GMM_color_segmentation/Result_images/4_Colors_batman.png" width="100" height="100" title="4 Color" />
<img src="./GMM_color_segmentation/Result_images/5_Colors_batman.png" width="100" height="100" title="5 Color" />
<img src="./GMM_color_segmentation/Result_images/6_Colors_batman.png" width="100" height="100" title="6 Color" />
<img src="./GMM_color_segmentation/Result_images/7_Colors_batman.png" width="100" height="100" title="7 Color" />
<img src="./GMM_color_segmentation/Result_images/8_Colors_batman.png" width="100" height="100" title="8 Color" />
</p

It can be seen that with less number of color components, GMM results are not as accurate, but the results are amazing
