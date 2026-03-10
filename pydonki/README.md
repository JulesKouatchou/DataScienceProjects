## pydonki: DONKI CME Analysis Dashboard

`pydonki` is a Python tool (run through a Streamlit dashboard) 
that performs web scraping to access 
the CCMC Space Weather Database Of Notifications, Knowledge, Information 
([DONKI](https://ccmc.gsfc.nasa.gov/tools/DONKI/)),
parse the content and extract [Coronal Mass Ejection](https://www.jpl.nasa.gov/nmp/st5/SCIENCE/cme.html) (CME) activities over a specified date range. 
The collected data is processed for analysis and visualization. 
Some of the features of the tool are:
- Ability to gather CME data over an arbitrary date range.
- Computations of statistics.
- Ability to perform data filtering based on month, year, speed, measuring technique, instrument used, etc.
- Selection of the type of graphs (histogram, pie chart, line plot, scatter plot, polar plot, etc.) to produce.
- Ability to perform additional web scraping (to extract visualizations from other sources) on specific CME activities (on a particular day) of interest.


The tool is used by scientists to automatically obtain the CME data, do data filtering, generate statistics and create interactive visualization.
