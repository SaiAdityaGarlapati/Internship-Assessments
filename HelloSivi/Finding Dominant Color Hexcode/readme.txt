Step1: read image data using cv2.imread() function from OpenCV as cv2.

Step2-Converting BGR to RGB: image color channel is generally in Blue-Green-Red format.
But we want Red-Green-Blue as our image color channel,
so we convert it to RGB channel using cv2.cvtcolor() function.

Step3-Image Data Reshaping:
There are 3-D parameters in our image data: row number X column number X color channel number.
But, we won’t need row and column information separately. Besides, it is hard to deal with 3-D Matrix that’s
why we reshape() image and make it 2-D Matrix data. This was the preparation part for images and
now we are ready to go on with clustering.

step3-Kmeans Clustering:
Since we will import K-Means from top of our code, we can easily use it by only giving n_clusters,
which represents cluster number originally. After that we will use fit() function to apply K-Means
Clustering algorithm on our pre-processed image data and result will come back to clt objects.

Step5-Find Histogram and Plot Colors:
We use find_histogram() function to limit the number of histograms to the desired number of clusters.
You can find the full details about find_histogram() and plot_colors2() function in this article below.

As we don’t want to find histogram for all pixel, and all the color palette, so we would like to limit it
to the desired number of clusters. The plot_colors2() function will prepare a bar, and put colors on this bar.

Step6-creating a Mathematical set of dominant colors
Download the plotted image and read it again. use pillow package to fetch pixel RGB values.
since pillow package has all the pixel values there is a lot of redundancy. so create a set from list.
then using colormap package fetch the hexcodes from RGB colors
