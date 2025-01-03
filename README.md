# Cheapskate Scraper

This is a simple Python script to scrape grocery prices from Woolworths.

It is dreaful - mostly because I was too lazy to ACTUALLY parse the resultant HTML & just lazily ripped the text from the `wc-product-tile` elements without considering any edge cases and then did some bullshit string manipulation

I am unsure EXACTLY how many products I am missing but, a cursory glance at [the bakery page](https://www.woolworths.com.au/shop/browse/bakery) and the consequent .csv file from scraping it will says... probably more than a few.

This is mostly because of this line in all the scripts

```Python
if len(l) != 2:
    continue
```

but, this is just a starting point and I intend to improve on it when the actual Cheapskate application is done. I'll have to hand label all of the macronutrient information now which... yeah...