---
date: 2021-03-01T10:00:56-04:00
description: "A web application that collects data for the Standard & Poor´s 500."
featured_image: "/images/project_4_SP500_image.png"
title: "Project 4: Standard & Poor´s 500 Stock Prices"
---

* libraries: streamlit, pandas, base 64, matplotlib, yfinance

This project uses pandas to scrap a list of the Standard and Poor's 500 companies.
The data frame can be sorted and filtered (and saved as a csv file).
The user can specify a number of S&P 500 companies they are interested in, to get detailed year to date information on stock closing price and volume from yahoo finance (using the yfinance module).

{{< figure src="/images/project_4_SP500_screenshot.png" >}}

[Link to GitHub Repository](https://github.com/bdoellinger/)

[Run application directly with Heroku](https://bd-project-04-sp500-stockprice.herokuapp.com/)
(if application isn't currently active on the server, starting might take a while)
