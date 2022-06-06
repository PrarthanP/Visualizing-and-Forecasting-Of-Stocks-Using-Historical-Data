# Visualizing and Forecasting Of Stocks Using Historical Data
The goal of the project is to accurately estimate the values of a basket of equities on the NSE/BSE. This study investigated and analysed a range of neural network prediction approaches, and ultimately chose the LSTM (Long Short-Term Memory, LSTM) neural network, based on the need for stock price prediction and the practical issues it encounters. The practicality of the procedure and the applicability of the model are then assessed, and a conclusion is reached after an in-depth examination of how to predict stock price using the LSTM. It has been discovered that historical data is particularly significant to investors when making investing decisions. Opening and closing prices have previously been employed as significant new financial market forecasters, but severe maxima and minima may provide extra information regarding future price behaviour.

# streamlit-multiapps
A simple framework in python to create multi page web application using streamlit.

# How to Run

1. Clone the repository:
```
$ git clone git@github.com:upraneelnihar/streamlit-multiapps
$ cd streamlit-multiapps
```

2. Install dependencies:
```
$ pip install -r requirements.txt
```

3. Start the application:
```
streamlit run app.py
```

# How to add new app

1. Add a new python file in `apps/`  folder with a function named `app`.

```
# apps/new_app.py

import streamlit as st

def app():
    st.title('New App')
```

2. Now add it to `app.py`

```
from apps import newapp # import your app modules here

app = MultiApp()

# Add all your application here
app.add_app("New App", newapp.app)
```

That's it your new app is added to your application and is live in default browser.
