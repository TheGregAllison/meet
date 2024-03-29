# Meet

## UI Screenshot:<br /><br /> <img width="651" alt="Screenshot 2024-02-04 at 10 09 25 PM" src="https://github.com/TheGregAllison/meet/assets/146021687/4e3c12a0-8cd0-4bba-a0e3-ab4095903c31">


## User Scenarios

### Filter Events by City:

**Scenario:** User filters events by a specific city
**Given** the user is on the Meet app home screen
**When** the user selects the "Filter" option and chooses a city from the available options
**Then** the app should display events specific to the selected city

---

### Show/Hide Event Details:

**Scenario:** Event are hidden by default.
**Given** the main page is open
**When** the app displays a list of event
**Then** the event details are hidden by default

**Scenario:** User shows event details
**Given** the user is viewing the list of events
**When** the user taps on a specific event
**Then** the app should display the details of that event

**Scenario:** User hides event details
**Given** the user is viewing the details of an event
**When** the user taps on the "Hide Details" option
**Then** the app should hide the event details and return to the event list

---

### Specify Number of Events:

**SCENARIO:** 32 events will be displayed to user by default
**Given** the user has not specified the number of events;
**When** the user views the events;
**Then** 32 events are shown by default.

**Scenario:** User sets the number of events to display
**Given** the user is on the Meet app home screen
**When** the user specifies the number of events to display
**Then** the app should show only the specified number of events

---

### Use the App When Offline:

**Scenario:** User accesses the app without an internet connection
**Given** the user has previously used the Meet app and data is stored locally
**When** the user opens the app without an internet connection
**Then** the app should display cached data and functionalities available offline

---

### Add an App Shortcut to the Home Screen:

**Scenario:** User adds Meet app shortcut to the home screen
**Given** the Meet app is installed on the device
**When** the user selects the option to add a shortcut to the home screen
**Then** the app should create a shortcut for easy access on the device's home screen

---

### Display Charts Visualizing Event Details:

**Scenario:** User views charts visualizing event details
**Given** the user is viewing the details of an event
**When** the user selects the "Charts" option
**Then** the app should display visual charts representing event-related data

## Serverless Functions

Serverless functions will handle many of the essential functions of the Meet App. AWS Lambda functions will generate authentication tokens, and handle users' access to public calendar events via the Google Calendar API.
