Exploration by Daniel Friedman, Halle Ritter, Orlando Torres & Kailin Xie.

Tech stack:
- Python
- Pandas
- Matplotlib

We wanted to look into MTA turnstile data and see patterns in ridership. We knew this would be a particularly challenging
dataset to work with; there are many anomalies and issues with the physical turnstiles that caused the data to be much 
different than expected.

The data source for the initial data exploration was the MTA turnstile data available from 
http://web.mta.info/developers/turnstile.html . We drew data from October 2014 through October 2017, encompassing over
 300 different subway stations initially with over 2000 turnstiles.

The initial format of the data reported subway entrances and exits as a running total over four-hour windows, per 
station, per day, per individual turnstile. We took five one-week slices of all the records - roughly equally spaced over
 3 years. We turned the running total into a per-day total by turnstile, and then summed the turnstiles over each 
 station. We then identified a few examples of stations with notable increasing or decreasing ridership trends, and 
 presented them as time-series graphs. Only 189 stations for which data existed at all periods over our analysis are 
 mentioned in our analysis.

**Stations with Declining Ridership from October 2014 - October 2017**

1. Prospect Park
2. Hoyt St.
3. 79th St.
4. 33rd St.

**Stations with Increasing Ridership from October 2014 - October 2017**
 
1. Metropolitan Ave.
2. Woodhaven Blvd.
3. 36th St.
4. 34th St. - Herald Sq.

While this was a fun data exploration, I don't think we'll be diving any deeper into this dataset.