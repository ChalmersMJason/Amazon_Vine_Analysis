# Amazon_Vine_Analysis
Module 16 Challenge

## Overview
This analysis was done to provide insight on the Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review. By utiliIng an ETL process, AWS RDS, and Pyspark, this analysis was prepared to determine if ther eis a bias toward favorable reviews from Vine members. 

## Results

* The below images show the methods used to determine how many Vine and non-Vine reviews there were in the chosen dataset. Results revealed 285 paid (Vine) reviews & 31545 unpaid (non-Vine) reviews. 

![image](https://user-images.githubusercontent.com/85259984/143304054-653a9973-b4cb-44e4-8367-9c523d350d9b.png)
![image](https://user-images.githubusercontent.com/85259984/143304091-ac966ca8-1b54-4402-a315-2c8e76d8b637.png)
![image](https://user-images.githubusercontent.com/85259984/143304144-5e1966b0-e842-4954-90b4-67c74d0da76b.png)

* 164 Vine reviews were 5 stars and 14,614 non-vine were 5-stars. Methods to determine this can be seen below

![image](https://user-images.githubusercontent.com/85259984/143304533-17077099-1476-42c7-9ede-0be54aa06b4f.png)

* On Vine reviews, 57% gave 5-stars. Compare this to 46% on non-Vine reviews. 

![image](https://user-images.githubusercontent.com/85259984/143304666-830ee1de-5a95-41d6-827d-4f126ac43e45.png)

## Summary
The results of this analysis do reveal a positivity bias on Vine reviews. 5-Star reviews are +11% as common in Vine reviews vs non-paid reviews. This suggests that paying customers to leave reviews can lead to less reliable feedback on the product. From a company's standpoint, it suggests that paying customers to leave reviews on a product will lead to more positive image of the product based on review sections. 

Another analysis that could be done for this is to look at the % of 4 OR 5 star reviews. Given the small sample size of Vine reviews, defining "positive" reviews as 4 or 5 can be more insightful than just looking at 5 stars. This can be doen with the below code:

![image](https://user-images.githubusercontent.com/85259984/143305378-8f96f2f6-7e82-4a85-942f-83f3d829296a.png)

The results of this method reveal an even larger bias of positivity when paying the customers for reviews. 
