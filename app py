import streamlit as st
import pandas as pd

st.title("Arduino LED Monitoring System")

led_on = st.checkbox("Turn LED ON")

if led_on:
st.success("LED ACTIVATED")
st.write("LED Status: ON")
st.metric("Arduino Pin", "D8")
else:
st.info("SYSTEM STANDBY")
st.write("LED Status: OFF")
st.metric("Arduino Pin", "D8")

data = pd.DataFrame({
"LED State": ["OFF", "ON"],
"LED Status": ["Not Lighting", "Lighting"]
})

st.subheader("LED State Comparison")
st.dataframe(data, use_container_width=True)
