# anamoly_detection_using_h2oIsaloationforest

The original KDD Cup 1999 dataset from UCI machine learning repository contains 41 attributes (34 continuous, and 7 categorical), however, they are reduced to 4 attributes (service, duration, src_bytes, dst_bytes) as these attributes are regarded as the most basic attributes (see kddcup.names), where only ‘service’ is categorical. Using the ‘service’ attribute, the data is divided into {http, smtp, ftp, ftp_data, others} subsets. Here, only ‘http’ service data is used. Since the continuous attribute values are concentrated around ‘0’, we transformed each value into a value far from ‘0’, by y = log(x + 0.1). The original data set has 3,925,651 class (80.1%) out of 4,898,431 records. A smaller set is forged by having only 3,377 class (0.35%) of 976,157 records, where attribute ‘logged_in’ is positive. From this forged dataset 567,497 ‘http’ service data is used to construct the http (KDDCUP99) dataset.

Description: X = Multi-dimensional point data, y = labels (1 = outliers, 0 = inliers)

http://odds.cs.stonybrook.edu/http-kddcup99-dataset/
