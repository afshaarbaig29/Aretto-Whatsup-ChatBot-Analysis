# Aretto WhatsApp ChatBot Analysis

## Overview
An end-to-end data analytics project analysing WhatsApp chat 
transcripts exported from Freshsales CRM for Aretto — a kids' 
footwear brand. The dataset covers 589 conversations over 
18–24 Feb 2024 and is heavily qualitative, requiring 
significant data cleaning before analysis.

## Business Questions Answered
1. What are the most common words customers use when they 
   initiate a conversation?
2. What time of day do customers reach out to the brand?
3. Which bot menu options do customers interact with the most?

## Tools Used
- Microsoft Power Query — data cleaning and transformation
- Power BI Desktop — dashboard and visualisations
- DAX — measures and calculations

## Data Cleaning Steps
- Extracted plain text from JSON-structured message_parts column
- Stripped HTML tags from bot outbound messages
- Removed system events (status changes, private notes, away messages)
- Converted UTC timestamps to IST (UTC +5:30)
- Classified messages by sender type (Customer / Bot / Agent)
- Built separate query tables per exploration

## Key Findings
- **Sizing is the #1 customer concern** — "size" appeared 516 
  times, with foot, shoe, and cms also in the top 10. Over 60% 
  of customer language is size-related.
- **Peak contact hours are 10–11 AM and 9–10 PM IST** — 
  suggesting a mid-morning browsing pattern and post-bedtime 
  parent shopping behaviour.
- **Bot size guidance options dominate interactions** — "Tell 
  me more about Aretto Size" was clicked 174 times, nearly 3× 
  more than any other option. 50% of bot interactions were 
  freeform replies indicating the menu needs redesign.

## Files
- `Aretto_ChatBot_Analysis.pbix` — Power BI dashboard file
- `Assignment_Chat_Transcript_Report.xlsx` — raw data source
