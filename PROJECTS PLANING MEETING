import pandas as pd
from datetime import datetime

# ---- INPUT DATA ----
meeting_title = "Project Planning Meeting"
date = "11-02-2026"
time = "10:00 AM"

participants_list = ["Sid", "Arjun", "Bhavani"]
agenda_list = ["Discuss roadmap", "Budget planning", "Assign tasks"]
decisions_list = ["Launch in March", "Increase marketing budget"]
actions_list = ["Sid to prepare report", "Arjun to finalize budget"]

prepared_by = "Sid"

# ---- CREATE STRUCTURED MINUTES ----
minutes = {
    "Meeting Title": meeting_title,
    "Date": date,
    "Time": time,
    "Participants": ", ".join(participants_list),
    "Agenda": ", ".join(agenda_list),
    "Decisions Taken": ", ".join(decisions_list),
    "Action Items": ", ".join(actions_list),
    "Prepared By": prepared_by,
    "Generated On": datetime.now().strftime("%d-%m-%Y %H:%M:%S")
}

# ---- CONVERT TO DATAFRAME ----
df = pd.DataFrame(list(minutes.items()), columns=["Field", "Details"])

print("\nMeeting Minutes Generated Successfully\n")
print(df)

# ---- SAVE AS CSV ----
df.to_csv("meeting_minutes.csv", index=False)

print("\nFile saved as meeting_minutes.csv")
