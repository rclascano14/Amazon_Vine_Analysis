# Amazon_Vine_Analysis
`Entering the world of big data as I perform ETL on a dataset from Amazon`

## Resources
- Google Colab
- PostgreSQL
- AWS/RDS
- Data: US Apparel Dataset (https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt)

## Overview of Analysis
I have learned what constitutes "Big Data" recently and what plays into it. One such thing is PySpark, which is commonly used to handle this Big Data. In conjunction with PySpark, I am using cloud services to store ample amount of data remotely, using AWS. With the knowledge of these tools at hand, I am tasked with analyzing Amazon reviews by members of the paid and unpaid Vine programs. I will use PySpark to perform the ETL process to extract/transform a selected dataset of my choice from the US Apparel Dataset. Then this dataset will be connected to an AWS RDS instance and then, finally loaded into pgAdmin. Once this is completed, I will use PySpark to test for bias among these reviews and show these results in this README. 

## Results

- How many Vine reviews and non-Vine reviews were there?
<img width="443" alt="Module 16 Picture 1" src="https://user-images.githubusercontent.com/95828604/163760763-83058dc8-d8dd-4897-9fb8-3ddbfffafb1e.png">

<img width="439" alt="Module 16 Picture 2" src="https://user-images.githubusercontent.com/95828604/163760772-b854aa63-e62c-473f-9e91-e66320d414bb.png">

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
<img width="709" alt="Module 16 Picture 3" src="https://user-images.githubusercontent.com/95828604/163760796-a4256325-d08f-4230-9806-52b6a71360eb.png">

<img width="746" alt="Module 16 Picture 4" src="https://user-images.githubusercontent.com/95828604/163760808-429446bc-40da-4892-aec0-746b523e67c7.png">

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
<img width="738" alt="Module 16 Picture 5" src="https://user-images.githubusercontent.com/95828604/163760830-f5968135-8497-45e8-8d3b-603e378a628d.png">

<img width="767" alt="Module 16 Picture 6" src="https://user-images.githubusercontent.com/95828604/163760839-f08d0b2a-9747-447c-9e56-ae5ce7290f54.png">

## Summary

In summation, there does not appear to be a positivity bias in the Vine program. For Paid members, 45.5% of reviews were 5 star and for Unpaid members, 52.3% of reviews were 5 star. With such a small disparity between the two percentages, it is clear that there is little to no bias between either paid or unpaid members, as they both result in roughly half of its reviews leaving 5 star reviews. To further prove my point and for further analysis, I would look into the Mean, Median and Mode of reviews for both paid and unpaid. This would allow us to see the distribution of reviews to provide insight as to whether any positivity bias exists or does not exist. 
