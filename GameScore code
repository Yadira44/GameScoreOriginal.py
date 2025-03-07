# GSC code
# calculate game score for a pitcher using Bill James version

# start the game

import streamlit as st

# Streamlit app title
st.title("Pitcher Game Score Calculator (Bill James)")

# Input fields using Streamlit
pitcher_name = st.text_input("Pitcher's Name: ")
outs_recorded = st.number_input("Enter how many outs the pitcher recorded: ", min_value=0, step=1)
hits_fourth = st.number_input("Enter how many innings were completed after the fourth: ", min_value=0, step=1)
number_strikeouts = st.number_input("Enter how many strikeouts they accumulated: ", min_value=0, step=1)
hits_allowed = st.number_input("Enter the number of hits they allowed: ", min_value=0, step=1)
earned_runs = st.number_input("Enter how many earned runs they allowed: ", min_value=0, step=1)
unearned_runs = st.number_input("Enter how many unearned runs they allowed: ", min_value=0, step=1)
bb_allowed = st.number_input("Enter how many walks (BB) were allowed: ", min_value=0, step=1)

# formula for game score total
Game_Score_Total = 50 + (outs_recorded * 1) + (number_strikeouts * 1) + (hits_fourth * 2) - (bb_allowed * 1) - (hits_allowed * 2) - (earned_runs * 4) - (unearned_runs)

# Calculate and print the total
if st.button("Calculate Game Score"):
    st.success(f"{pitcher_name}'s Game Score: {Game_Score_Total}")
