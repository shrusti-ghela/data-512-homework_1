# data-512-homework_1

The goal of this assignment is to construct, analyze, and publish a dataset of monthly article traffic for a select set of pages from English Wikipedia from January 1, 2015 through September 30, 2022.  The purpose of the assignment is to develop and follow best practices for open scientific research.

Through this repo, we have been able to construct, analyze and publish this work collecting data through Pageviews API (details on access, license and use below), that provides access to desktop and mobile trafic data.

The Pageviews API documentation: https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews.

Additional information to the Wikimedia Foundation REST API terms of use: https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions

This is the link to the REST API: https://www.mediawiki.org/wiki/Wikimedia_REST_API

Global Rules Limit your clients to no more than 200 requests/s to this API. Each API endpoint's documentation may detail more specific usage limits. Set a unique User-Agent or Api-User-Agent header that allows us to contact you quickly. Email addresses or URLs of contact pages work well.

By using this API, you agree to Wikimedia's Terms of Use and Privacy Policy. Unless otherwise specified in the endpoint documentation below, content accessed via this API is licensed under the CC-BY-SA 3.0 and GFDL licenses, and you irrevocably agree to release modifications or additions made through this API under these licenses. See https://www.mediawiki.org/wiki/REST_API for background and details.

## Files in the repo

### data:

- dinosaur_genera.cleaned.SEPT.2022.csv : A CSV file conatining the list of Dinosaur pages from Wikipedia.
- dino_monthly_desktop_201501-202209.json : This file is obtained from the data_acquisition_and_data_analysis notebook and contains data on the monthly desktop page traffic.
- dino_monthly_mobile_201501-202209.json : This file is obtained from the data_acquisition_and_data_analysis notebook and contains data on the monthly mobile app and web traffic.
- dino_monthly_cumulative_201501-202209.json : This file is obtained from the data_acquisition_and_data_analysis notebook and contains data on the monthly cumulative (sum of all movile and all desktop) page traffic.

### results:

- maximum_minimum_average.png : Time series result for the articles that have the highest average page requests and the lowest average page requests for desktop access and mobile access.
- top_ten_peaks.png : Time series result for the top 10 article pages by largest (peak) page views over the entire time by access type.
- fewest_months.png : Time series result to show pages that have the fewest months of available data.

### code:

- data_acquisition_and_data_analysis.ipynb : In this notebook, the data is obtained using the pageviews API. The counts of pageviews are collected for a set of Dinosaur pages from Wikipedia and basic data visual analysis is performed to graph the Dinosaur subset as a timeseries for Desktop and Mobile access type.

