# covidni_dashboard

The [CovidNI dashboard](https://obrienjoey.github.io/covidni_dashboard/) summarizes a range of data regarding the development of the Covid 19 pandemic with Northern Ireland. 

This includes summaries of cases, deaths, and hospitilizations arising from the virus since March 2019. Further local information is also provided at the electoral level and indeed the HSC trust level for inpatients.

Examples visuals from the dashboard can be seen below

![Optional Text](img/inpatient.PNG = 600x400)

** Data **

The data used in this analysis is updated daily via an additional repository found [here](https://github.com/obrienjoey/covid19northernireland).

** Dashboard Deployment **

The dashboard is implemented using the `R` programming language, in particular the following packages are utilized

1. flexdashboard
2. plotly & mapview
3. dplyr
4. DT

In terms of deployment, there is a two step process. First of all the **covid19northernireland** repo collects updated data daily, the dashboard is then updated each day at 23:00 to incorporate this latest data via an external server from the .yaml script found in the workflows folder.
