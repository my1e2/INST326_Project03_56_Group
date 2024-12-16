# INST326_Project03_56_Group
Project 3
**Features Breakdown**
1. Caregiver Management:
Add Caregiver: Adds a new caregiver to the list with details like name, phone, email, pay rate, and weekly hours.
Update Caregiver: Select an existing caregiver from the list and update their details.
Delete Caregiver: Remove a selected caregiver from the list.
2. Availability Management:
Set Availability: Allows you to select a caregiver and set their availability for the week. Options include "Preferred", "Available", or "Unavailable" for each shift (AM and PM) of every day.
3. Schedule Generation:
Generate Schedule: Automatically generates a weekly care schedule. Preferred caregivers are prioritized, and the schedule is saved as an HTML file that can be shared.
4. Payroll Management:
Payroll Report: Displays a payroll report for all caregivers, showing weekly and monthly pay. The report can be saved as an HTML file.
5. Hours Update:
Update Hours: Allows you to modify the hours worked for a selected caregiver.
**Code Structure**

Classes:
Person: Base class for storing basic information like name, phone, and email.

Caregiver: Inherits from Person, adding attributes for pay rate, availability, and hours worked. Includes methods for updating details, setting availability, and calculating pay.

CaregiverManager: Manages the Tkinter interface, caregiving operations, and GUI elements.
Methods:

add_caregiver(): Adds a caregiver to the list.

update_caregiver(): Updates details of a selected caregiver.

delete_caregiver(): Deletes a selected caregiver.

availability_window(): Opens a window to set caregiver availability.

generate_schedule(): Generates a care schedule based on caregiver availability.

payroll_report(): Generates and displays a payroll report.

update_hours(): Updates the hours worked for a selected caregiver.

License

This project is licensed under the MIT License - see the LICENSE file for details.
