# Hospital-Management-System

In the Hospital Management System JDBC Project, three core classes—Doctor, Patient, and Driver—work together to handle the core functionalities of managing appointments, doctor availability, and patient records. Here's an overview of each class:

  1. Doctor Class
Attributes:
doctorID: Unique identifier for each doctor.
name: Name of the doctor.
specialization: Medical specialty (e.g., cardiologist, dermatologist).
availability: Status indicating whether the doctor is available for appointments.
Methods:
getDoctorDetails(): Retrieves and displays the doctor’s information.
checkAvailability(): Checks if the doctor is available for appointments.
updateAvailability(boolean status): Updates the availability status of the doctor.

  2. Patient Class
Attributes:
patientID: Unique identifier for each patient.
name: Name of the patient.
age: Age of the patient.
appointmentDate: Date and time of the patient’s appointment.
doctorID: ID of the doctor assigned to the patient.
Methods:
addPatient(): Allows the addition of a new patient to the system.
viewPatientDetails(): Displays the details of the patient, including the doctor they are assigned to.
bookAppointment(int doctorID, String appointmentDate): Books an appointment with a specific doctor.

  3. Driver Class
Functionality:
This class serves as the entry point to the system. It interacts with the Doctor and Patient classes, manages the database connections using JDBC, and facilitates the interaction between the patient and doctor.
Methods:
main(): The main method where users can perform actions like viewing doctors, checking availability, adding new patients, and booking appointments.
connectToDatabase(): Establishes the JDBC connection to the hospital database.
executeQueries(): Executes SQL queries to perform actions like retrieving doctor availability, adding patient records, and updating appointments.
  
  4. Overall System Flow
The Patient can search for available Doctors.
The Driver class connects to the database using JDBC to retrieve doctor availability.
The patient can then book an appointment with a selected doctor.
The system can also add new patients and manage existing patient records.
This project integrates JDBC to connect with a hospital management database, ensuring seamless data retrieval and storage for both doctors and patients.
