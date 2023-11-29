# Doctor-Appointment-scheduling
The schedule_appointment function efficiently finds common time blocks for scheduling appointments between a doctor and a patient while considering their respective time constraints. This implementation leverages set operations to streamline the process.

Function Overview:
The function takes five parameters:
doctor_blocked_time: A list of time blocks during which the doctor is unavailable.
doctor_time_limits: A list representing the earliest and latest times the doctor is available for appointments.
patient_blocked_time: A list of time blocks during which the patient is unavailable.
patient_time_limits: A list representing the earliest and latest times the patient is available for appointments.
meeting_duration: An integer representing the desired duration of the appointment in minutes.
Implementation:

Time Block Calculation:
The function defines an inner function get_available_time_blocks to calculate the available time blocks for a person.
The datetime.strptime method is used to convert time strings into datetime objects for ease of comparison.
The available time blocks are determined by analyzing the gaps between blocked time intervals.

Output Formatting:
The final result is formatted to display the common time blocks in the required ['HH:MM', 'HH:MM'] format.
