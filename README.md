# Image-processing-on-Lung-CT-images
Algorithm for Lung tissue segmentation and Lung lesion segmentation and comparing accuracy with manually created masks

1.	To create an algorithm for Automatic Segmentation of Lung tissue on CT – Images. Check the accuracy of your algorithm by comparing with Manual Segmentation of lung.

Codes in "Lung Tissue Segmentation - Active Contour..."
Active contour with defined thresholds is used to create a mask on the lung. Post processing is done (imfill and erosion)

2.  To compare with a manually segmented image of lung.

Codes in "Comparing output with manual ROI..."
Active contour with defined thresholds is used to create a mask on the lung. Post processing is done (imfill and erosion)
Manual ROI defined to take into consideration, both the lungs in case of unconnected compunents.
Post processing done by erosion
Dice and Jaccacrd Indices are calculated and compared.

3.  To plot Maximum and minimum intensity projection.

Codes in "Minimum and Maximum Intensity projection"
Maximum and minimum intensity projections.
Maximum intensity gives the projection of the bronchioles as they are of higher intensity compared to the alveoli
Minimum intensity projection is to give the alveolar regions with no bronchioles/bronci. 
These two help study two different components and also would give insights to various abnormalities.

4.	Create an algorithm to segment lesion and compare the accuracy with manually segmented portion.

Codes in "Lung Lesion Segmentation (Region Growing) ... "
Lung Lesion segmentation done using region growing. We take 2 user defined seedpoints and apply region growing algorithm on the lesion areas. 2 seed points were taken as the test case had 2 disconnected lesions.
Manual ROI masks are created for the 2 lesion regions to compare our segmentation algorithm accuracy.
Dice and Jaccard indices are calculated for the 2 segmentations and overlapped and displayed using imshowpair.

All the algorithms work with fairly good accuracy.
