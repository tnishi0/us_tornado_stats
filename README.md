# Is there evidence of climate change in the US tornado statistics?

In [a National Geographic's online educational article](https://education.nationalgeographic.org/resource/tornadoes-and-climate-change), they say that, "when you remove small tornadoes from the record, the data does not suggest any long-term increase in tornado frequency." So, I used data from [Storm Events Database (by the National Centers of Environmental Information)](https://www.ncdc.noaa.gov/stormevents/) to confirm this:

* [Data collection](data_collection.ipynb): Using the pandas, BeautifulSoup, and requests modules in Python, I downloaded all the data files containing anunual storm statistics and extracted the tornado data.
* [Data cleaning](data_cleaning.ipynb): Using pandas, matplotlib, and numpy, I cleaned the tornado data.  In particular, I had to handle missing information on tornado strengths.
* [Analysis](): ***


Notes:
* "a closer look at the data shows the increase is only in the weakest category, EF0. There's been no increase in stronger twisters, and maybe even a slight decrease in EF4s and EF5s." (from [Tornadoes and Global Warming: Is There a Connection?](https://education.nationalgeographic.org/resource/tornadoes-and-global-warming-there-connection))
* Can we model the time between tornados with a statistical distribution, like exponential distribution?  Can we do inter-event time embedding?
