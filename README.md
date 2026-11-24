# ARIN121-Assignment3-TravelPlanner

ARIN121 Assignment 3 – Travel Planner

A travel planning assistant built as a system prompt (system-prompt.md) and tested in Google AI Studio Playground. It helps travellers plan a trip and then revise the plan through a short back-and-forth conversation.

What the planner can do

Main menu The planner opens with a menu when you haven't said what you want to do. You can pick an activity by number, by name, or by just saying what you need. Type menu at any time to come back to it.

1. Plan a new trip

Asks up to 3 short clarifying questions (with example answers) if the destination or trip length is missing or too broad.
Checks which place you mean if the name is ambiguous (for example, Kingston, Ontario or Kingston, Jamaica).
Shows a short trip summary and waits for you to confirm it.
Builds a day-by-day itinerary (morning, afternoon, evening).
Shows estimated costs with the currency and a total if you give a budget, and suggests a cheaper option if it goes over.
Adds a "Rainy-day option:" for outdoor activities and mentions the usual weather for your dates.
Only answers travel-related requests.

2. Revise my travel plan (new) A multi-turn activity for changing a plan you already have.

The planner uses the itinerary from the conversation, or asks you to paste yours.
It asks what you want to change (for example, less walking, more indoor activities, lower cost) and why.
It suggests changes to only the affected parts, shown as old → new with a reason.
It asks whether the changes work for you and keeps adjusting based on your answer.
When you're happy, it shows the full updated plan and returns to the menu.
How to use it
Paste system-prompt.md into the System Instructions in Google AI Studio.
Start with a general message such as "Hi, can you help me?" to see the menu.
Reply 1 or 2, or describe what you need, for example "I want to plan a trip to Lisbon" or "Can you make my plan less tiring?".
To switch activities, just say so ("Actually, let's fix my existing plan instead"). The planner keeps details you've already given, like destination, travellers and budget.
Say "done" or "menu" to stop an activity.
Version history
main first contained the final Assignment 2 prompt unchanged (commit "Preserve Assignment 2 starting prompt").
The menu and the Revise my travel plan activity were developed on the conversational-features branch and merged into main through a pull request.
