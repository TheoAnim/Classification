# Dry Beans Classification
Classification and Price Prediction of Dry Beans Using Different Methods
Background
In a recent paper, Koklu et al. explored the possibility of using morphometric measurements on seven commonly cultivated white beans to develop an automated (or at least machine assisted) method for separating the white beans when presented at market.

Using certified dry bean seeds in Turkey is around 10% (Bolat et al., 2017). Dry bean cultivation in Turkey and Asian countries usually in the form of populations containing mixed species of seeds. Also, there is not much certified seed planting area (Varankaya and Ceyhan, 2012). Since different populations which contain different genotypes are cultivated, the final products contain different species of seeds. Thus, when the dry bean seeds obtained from population cultivation are released to the market without being separated by species, the market value decreases immensely (Varankaya and Ceyhan, 2012). -Murat Koklu, Ilker Ali Ozkan, Multiclass classification of dry beans using computer vision and machine learning techniques, Computers and Electronics in Agriculture, Volume 174, 2020,

For this project you have a slightly different task- you are expected to develop an automated method that predicts the value of a harvest from a ‘population cultivation’ from a single farm that has been presented at market. For each of the different varieties of white beans, you will be given the price per pound and the average number of seeds per pound.

You will be expected to take into account the differing costs of a mistake when you classify the seed varieties.

Data Resources and Structure
For this project you will be given a training sample of beans that are classified into 6 varieties of white beans- at a hypothetical (ie. made up by me!) local market price per lb in USD.

Bombay ( $5.56/lb)
Cali ( $6.02/lb)
Dermason ( $1.98/lb)
Horoz ( $2.43/lb)
Seker ( $2.72/lb)
Sira ( $5.40/lb)
Seed weight in grams (average gram per seed) Seker 0.49 grams/seed Bombay 1.92 grams/seed Cali 0.61 grams/seed Horoz 0.52 grams/seed Sira 0.38 grams/seed Dermason 0.28 grams/seed

(Note that there are ~453.592 grams per pound)

In the paper by Koklu and Ozkan there is a seventh variety (Barbunya) that we are ignoring for this task.

The column Labels of the training data are as follows. Please see the provide papers for additional details.

Area: Area (\(A\)): The area of a bean zone and the number of pixels within its boundaries. \[A=\sum_{r,c \in R} 1,\] where \(r\), \(c\) is the size of the bean region.
Perimeter (\(P\)): Bean circumference is defined as the length of its border.
MajorAxisLength (Major axis length (\(L\))): The distance between the ends of the longest line that can be drawn from a bean.
MinorAxisLength (Minor axis length (\(l\))): The longest line that can be drawn from the bean while standing perpendicular to the main axis.
Eccentricity (\(Ec\)): Eccentricity of the ellipse having the same moments as the region.
ConvexArea (Convex Area (\(C\))): Number of pixels in the smallest convex polygon that can contain the area of a bean seed.
Extent (\(Ex\)): The ratio of the pixels in the bounding box to the bean area. \[ Ex=\frac{A}{A_b},\] where \(A_b\) is the Area of a bounding rectangle.
Class: One of the six bean types/varieties (BOMBAY, CALI, DERMASON, HOROZ, SEKER, SIRA)
