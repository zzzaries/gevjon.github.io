---
layout: post
title: Exploration on Long Short Term Model (LSTM)
categories: [Technical]
tags: [Neural Network, Machine Learning]
---

Upon working on a project to predict the future sells of on-shelf products, our team implemented a Light Gradient Boosting Model (LGBM) and reached an $$ R^2 $$ score of 0.7 for average weekly forecast. \\
(Project detail: [unmanned shelf](http://www.feng1.com) with [SF-Express](http://www.sf-express.com/us/en/))

Considering this is a time series model, I'm thinking about adding a Long Short Term Model (LSTM) layer onto it. So this blog will share my exploration on the LSTM model, including its theory, practices and take aways.

~~~ python
import pandas as pd
import numpy as np

data = pd.read_csv("...")
~~~
