# Image-Segmentation-and-Compression

## Segmented the image into regions with the homogeneous visual appearance or which corresponds to objects
## Used K-Means clustering algorithm to segment the image into clusters of a palette of K colors and performed lossy data compression 

# Observations:
> - To store all colors,
> - we need 8 bit * 3 = 24bit, to represent (r, g, b)
> - for N pixels, it results into 24*N
> - but now we're using logK bits only to represent k colors, so it totals to
> - 24K (to map k colors with (r, g, b) values) + log2(K) N
> - which is less than the former.

# Explanation:
> - For our sample image, there are 200 * 183 pixels
> - normally it will be 10,54,080 bits
> - but using 10 clusters, it will be 1,21,752 bits
> - which is way more lesser than the former one
