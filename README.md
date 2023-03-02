## ItemsAPI
### Fortnite Cosmetics Visualization

I wanted to see the different amounts of rarities type and when different items were released throughout Fortnite. 
For the api, I used https://dash.fortnite-api.com/

The url I called was very simple and didn't require any extra parameters. I later cleaned and visualized the data. 

- The api

The api usually needs a key to access and retrieve data, but since the url was almost the base url for cosmetics, it can be requested without an API key. If any modifications or different parameters want to be selected, a key might be needed. The response is in json form. 

- Required packages

I imported requests, pandas, and json for this assignment. 

- Processing the data

I used pandas dataframes. I needed to clean the data so I removed columns that I wouldn't need. I mostly removed columns like urls, or extra tracking tags and other unneeded data. I used str.contain as a condition when it came to replacing strings. Since I wanted to plot by qualitative value, especially for item rarities, I turned the entire dataframe into string values so it would be easier to use the str.contain condition. I also replaced the messy timestamps with cleaner year values that would look better.

- Visualizing the data

I used a bar chart to visualize the data. I added x and y labels, and a title as well. The chart was from greatest to least amounts. There were two charts created, one for the rarities, and one for the annual amount of items released.

- Conclusions

After viewing the data, I was surprised that the amount of Epic rarity items were almost the same as uncommon. I figured that Epic Games does this as a marketing technique, and release many items at a misleading high rarity, just so they can sell it for higher profits. I also noticed that the years 2020-2022 had a stable similar amount of items released.
