# app.py
import streamlit as st

st.title("Ma première application Streamlit")
st.write("Hello, Streamlit!")


import pandas as pd

# Création d'un DataFrame simple à partir d'un dictionnaire
data = {
    'Nom': ['Alice', 'Bob', 'Charlie', 'David'],
    'Âge': [25, 30, 22, 35],
    'Ville': ['Paris', 'New York', 'Berlin', 'Tokyo']
        }
df = pd.DataFrame(data)

st.line_chart(df)
