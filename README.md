# Workflow Layout

<img width="1304" height="571" alt="image" src="https://github.com/user-attachments/assets/73df6c15-7976-4bd1-b3cb-f97784e14025" />

This workflow is meant to roughly simulate a log risk analysis and the actions that should be taken.
</br>This workflow automatically pulls logs from Splunk, a SIEM platform, and uses Google Gemini which gives a “risk score” assessing how serious an action must be taken, if any, according to what the security logs show. If the score is low, it simply archives the analysis. If the risk score is slightly concerning, an entry is made in Google Sheets as a form of ticketing for security personnel to address when they can. And if the risk score is high, and email is sent using Gmail directly to the Security personnel. This is all done automatically with no human interaction; it simply takes the click of a button.

</br>Below is each node explained in a little more detail about what is happening.

### Device Used
- N8N Software (locally installed)
- Google Gemini API
- Google Gmail API
- Google Drive/Sheets API

## Node Details
