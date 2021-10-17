
# Overview of Amazon review  Analysis:
The purpose of this analysis is to analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

## Results:
```
tools_filtered_df =df.filter(df.total_votes>=20 and df.product_category="tools")
```

This gives the results where the total votes is greater than 20 and product category is tools.

```
percent_is_not_vine_five_star=(five_star_is_not_vine/not_vine_total_reviews)*100
percent_is_not_vine_five_star
```

If they are not a vine member there is a 46% chance than the reviews are 5 star reviews.
Its probable not biased because they are an unpaid member

```
percent_is_vine_five_star=(five_star_is_vine/vine_total_reviews)*100
percent_is_vine_five_star
```

If they are a vine member there is a 57% chance than the reviews are 5 star reviews.
Its is still little biased but we have to account many other factors to conclude

 
## Summary:
* There is a slight bias for the vine program customers to give 5 star reviews as they constitue about 57% and 46% of them are non vine program people.
* There is a high chance that vine program people may get a lot of products to review where as non vine program people have to buy the product to give a review. So we might not  consider the averages as it is.