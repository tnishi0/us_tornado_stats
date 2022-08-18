# Is There Evidence of Climate Change in the US Tornado Statistics?

[Intro, TO BE EDITED!] Refer to the assignment in the Coursera course in which I analyzed data on tornados in Midwestern states and observed overall increase in the number of tornados over the last several decades.

I came upon two National Geographic online educational articles ([_Tornadoes and Climate Change_](https://education.nationalgeographic.org/resource/tornadoes-and-climate-change) and [_Tornadoes and Global Warming: Is There a Connection?_](https://education.nationalgeographic.org/resource/tornadoes-and-global-warming-there-connection)), which discuss impact of climate change on tornados in the US and makes a few claims trends in tornado statistics.  I will try to visualize and validate some of these claims.  For this purpose, I will use the data from [Storm Events Database](https://www.ncdc.noaa.gov/stormevents/) (by the National Centers of Environmental Information).  Using the pandas, BeautifulSoup, and requests modules in Python, I downloaded all the data files containing anunual storm statistics and extracted the tornado data ([data_collection.ipynb](data_collection.ipynb)).  Then, I did preliminary exploration and cleaned the data ([data_cleaning.ipynb](data_cleaning.ipynb)).  In particular, I had to handle missing information on tornado strengths.  Using the cleaned data, I examined the validity of the following specific claims from the National Geographic articles:
* "... when you remove small tornadoes from the record, the data does not suggest any long-term increase in tornado frequency." (from [_Tornadoes and Climate Change_](https://education.nationalgeographic.org/resource/tornadoes-and-climate-change)) and/or "... a closer look at the data shows the increase is only in the weakest category, EF0. There's been no increase in stronger twisters, and maybe even a slight decrease in EF4s and EF5s." (from [_Tornadoes and Global Warming: Is There a Connection?_](https://education.nationalgeographic.org/resource/tornadoes-and-global-warming-there-connection))
* In [an assignment](Coursera_Assignment_4_Nishikawa.pdf) for the Coursera course [_Applied Plotting, Charting & Data Representation in Python_](https://www.coursera.org/learn/python-plotting?), I observed an inreasing trend in the number of tornadoes in the midwestern states.  But when I filtered out those tornadoes with strength 0, the trend disappeared ([Jupyter notebook](/analysis_midwestern.ipynb)).
* "Research has shown that there are fewer days with at least onetornado but more days with over thirty, even as the total number of tornadoes per year has remained relatively stable." (from [_Tornadoes and Climate Change_](https://education.nationalgeographic.org/resource/tornadoes-and-climate-change))
* "The number oftornadoes in the states that make up Tornado Alley are falling, while tornado events have been on therise in the states of Mississippi, Alabama, Arkansas, Missouri, Illinois, Indiana, Tennessee, and Kentucky." (from [_Tornadoes and Climate Change_](https://education.nationalgeographic.org/resource/tornadoes-and-climate-change))

TEMPORARY NOTES:
* [Tornado Dashboard: Exploring Three Decades of Violent Storms](https://education.nationalgeographic.org/resource/tornado-dashboard-exploring-three-decades-violent-storms); see also [the dashboard at esri site](https://storymaps.esri.com/stories/tornadoes/).
* Can we model the time between tornados with a statistical distribution, like exponential distribution?  Can we do inter-event time embedding?
