import streamlit as st

# App title
st.title("Yarn Count Calculator")

# Input fields for yarn length and weight
yarn_length = st.number_input("Enter yarn length (in cm):", min_value=0.0, step=1.0, format="%.2f")
yarn_weight = st.number_input("Enter yarn weight (in grams):", min_value=0.0, step=1.0, format="%.2f")

# Ensure inputs are valid before calculating
if yarn_length > 0 and yarn_weight > 0:
    # Calculate yarn count
    yarn_count = (yarn_length * 453.6) / (yarn_weight * 2.54 * 36 * 840)
    st.success(f"The calculated yarn count is: {yarn_count:.2f}")
elif yarn_length == 0 or yarn_weight == 0:
    st.info("Enter both values to calculate the yarn count.")
else:
    st.warning("Please enter positive numbers only.")
