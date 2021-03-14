---
date: 2021-03-01T10:00:57-04:00
description: "A simple web application that collects data for the top 100 cryptocurrencies."
featured_image: "/images/project_3_cryptocurrencies_image.jpg"
title: "Project 3: Cryptocurrencies"
---

* libraries: streamlit, PIL, pandas, base 64, matplotlib, BeautifulSoup, requests, json

Cryptocurrencies are currently on the rise. However due to their volatile nature the price can change by a large margin in a small amount of time.

This project uses BeautifulSoup4 to scrap data for up to 100 cryptocurrencies from coinmarketcap.com.
The data is then processed using pandas to display a data frame of relevant information (which can also be saved as an csv file).
Users can then choose a number of cryptocurrencies they are interested in, to generate a plot of percentage change over a chosen time period using matplotlib.

{{< figure src="/images/project_3_cryptocurrencies_screenshot.png" >}}

[Link to GitHub Repository](https://github.com/bdoellinger/03_Cryptocurrencies)

[Run application directly with Heroku](https://bd-project-03-cryptocurrencies.herokuapp.com/)
(if application isn't currently active on the server, starting might take a while)
