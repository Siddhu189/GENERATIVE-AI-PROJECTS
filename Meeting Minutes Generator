# ==============================
# Meeting Minutes Generator
# ==============================

import pandas as pd
from datetime import datetime

print("MEETING MINUTES GENERATOR\n")

# User Inputs
meeting_title = input("Enter meeting title: ")
date = input("Enter meeting date (DD-MM-YYYY): ")
time = input("Enter meeting time: ")
participants = input("Enter participants (comma separated): ")
agenda = input("Enter agenda points (comma separated): ")
decisions = input("Enter decisions taken (comma separated): ")
action_items = input("Enter action items (comma separated): ")
prepared_by = input("Prepared by: ")

# Process Inputs
participants_list = [p.strip() for p in participants.split(",") if p.strip()]
agenda_list = [a.strip() for a in agenda.split(",") if a.strip()]
decisions_list = [d.strip() for d in decisions.split(",") if d.strip()]
actions_list = [a.strip() for a in action_items.split(",") if a.strip()]
