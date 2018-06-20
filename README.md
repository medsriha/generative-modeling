# Generative-Modeling
Analytic approach to electricity disaggregation from simulated smart meter data using generative modeling

In this notebook, we'll develop a simple (though not that simple) approach to electricity disaggregation from simulated smart meter data. Electricity disaggregation is the task of taking an aggregate energy signal (such as the readings that come, once an hour, from an electricity meter at we house) and attempting to break down the end uses of this electricity: separating the signal into the components based upon cooling, heating, large appliances, lighting, etc. Studies have shown that providing this type of detailed breakdown and let consumers or building managers make better decisions about energy management, and also provides improved consumption forecasting approaches.

In this notebook, we'll use PyMC to develop a probabilistic model that will let we compute a simple breakdown of whole-home energy into three different categories: air conditioning (we'll consider data that only spans a summer month, so there won't be any heating component), appliances (devices that are on sporadically only when an occupant is home and awake), and baseload (devices that are always on, regardless of whether the occupant is home, away, or asleep).

Source: Practical Data Science 16588
