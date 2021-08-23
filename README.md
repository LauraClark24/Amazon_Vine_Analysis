# Amazon Vine Analysis
## Overview
This analysis is designed to look at a set of review data and assess whether there is a more positive opinion coming from reviews that were encouraged by paying the reviewers. By taking publicly available review data from Amazon, we will be able to do analysis on two sets of data, divided by whether or not the review came from the Vine program that pays users to leave a review.
## Results
The Amazon dataset for books that I did my analysis on seems like it may have been an outlier. After the requested filtering, there were no reviews there the Vine feature indicated that they were indeed from the Vine program. 

![0FilteredYes](https://user-images.githubusercontent.com/83182353/130381952-54dfe321-edb6-4ce8-952c-1385d9809655.png)

By going back to the nonfiltered set, I managed to find two reviews in the entire dataset that were paid for. They may have had too few helpful votes for most to consider, but the ration of helpful to total votes fit our parameters and they were my only potential data points, so I decided to run with this set anyways.

![yesesUsed](https://user-images.githubusercontent.com/83182353/130381979-fd5e4929-6561-4121-b4a7-69b10e1447bf.png)
![yesCount](https://user-images.githubusercontent.com/83182353/130382003-53a0d300-3c19-4388-a0b0-426b11aff9f2.png)

I promptly wrote up the code, even thou it was just as simple (to more so) to do these calculations in my head. 50% of the reviews and 66% of the votes were five star, and the remaining 50% of the reviews and 33% of the votes were four star. 

![yesPercent](https://user-images.githubusercontent.com/83182353/130381991-34f2d0de-e552-427e-a626-eef8d4038f72.png)

Non-Vine reviews had more normal numbers, with the filtered down set returning over 400,000 reviews to be assessed. With more than 2 million times as many votes in this data set than in the yes dataset, this has a much more reasonable confidence level.

![noCount](https://user-images.githubusercontent.com/83182353/130382081-6117ade2-0554-480d-bcd3-5beb3f8197f9.png)

These non-Vine reviews had over 240,000 5 star reviews, so even given the large data set, that is an impressive 60% of all the reviews that this dataset includes. 4 star is the next largest with 60,000, setting it at a significantly smaller 15%.

![noPercent](https://user-images.githubusercontent.com/83182353/130382112-0b43a39c-f41a-417a-962f-d46f63afeab3.png)

## Summary
 All conclusions about the reviews in the Vine program are more strongly guesswork than any analyst should be comfortable with presenting, so I will try to keep them to a minimum.  Given the book reviews had a majority, ¾ of all reviews, at 4 or 5 star without being a part of the Vine program, it makes sense that almost no one was willing to buy reviews rather than wait for free ones while spending the money on advertising of something else that would tie directly to profits. Given that there were only two reviews from the Vine program and the fact that they lined up with the two scores that had the largest percentage of non-Vine reviews, there were not enough information to prove a statistically significant difference in the results. I would recommend looking at a dataset that has, hopefully, nearly as many reviews from the Vine program as not in order to be able to have a decent level of confidence for or against a difference in the outcomes of reviews from these two datasets. To this end, do not consider the digital video games dataset from Amazon as it has no reviews from the Vine program. 
