# Some Thoughts about my MAKEUP API VIGNETTE


## About what I did for the vignette and interesting findings...
I created a makeup API vignette with the purpose of exploring how to read in data using a function created for interacting with a specific API, 
as well as showing different types of data analyses that can be conducted on the data obtained.

I built a few functions to interact with 2 API endpoints: makeup product brand and product type.
After data was returned, it went through some data cleaning and manipulation steps to form an analysis-ready data frame. 

The second half of this vignette focused on exploratory data analysis (EDA). 
I used table, summarize and ggplot functions to generate contingency table, numerical summaries of makeup price and rating, and different plots for data visualization.

I found this vignette is actually handy for my future makeup shopping if they continually update the API with newly released items. 
I can search makeup products by brand and type, also compare their price and rating with the price and rating summaries from the same type products.

I did learn a few interesting facts such as, the most popular and well known product of a brand may have lower rating compared with other items.
Some cheap items were rated much better than expensive ones, with this concept, I will save some money from cutting down high end products.

## Some thoughts about the process...
I think the data source is a bit limited, it has only 2 categorical and 2 numerical columns that can be used for analysis. 
I would be much happier if it has more numerical variables such as weight, that way I can calculte the unit price.

From a programmer perspective, I am so new to R that I wish my R skill could be 1/10 as good as my SAS skill.
Due to not familiar with the syntax, and those 2 software opperate differently, my R code is not efficient and well structured as I would like it to be.
I hope after using it more often, my R skill could catch up.

## Links... 
My final vignette is located [here](https://github.com/ViviFeathers/558Basic/blob/main/README.html), please download this html file and read thought the functions and EAD I created (the scatter plots do not show up in github because they are stored in a list, you will see them after download the html file).
You can also look into my [repo](https://github.com/ViviFeathers/558Basic/tree/main) for more information.
