# Facial-Recognition---Attendance-system

The basic model of how  this project works is that if a person's face is recognized by the camera (it needs to be stored in the database
with respective name and ID to be recognized) , attendance of the person will be added with name and ID to a CSV file (not containing
duplicates). If face is not recognized, there are no changes made in the csv file and the face is detected as unknown. The project 
consists of three files namely face_dataset.py, face_training.py and face_ recognition.py . 

This project can be run on your local machines by doing the steps mentioned below: -  


Step 1: Open the face_recognition.py and check the names array. Append your name in the array. Your ID will thus be the corresponding index
of your name in the array.  

Step 2: Run face_dataset.py . It will ask for an ID, input the ID associated with your name. The program will capture multiple images of you
through the Webcam and your face will be added to the dataset.  

Step 3: Run face_training.py . It generates a trainer.yml file.  

Step 4: Run face_recognition.py . Your face will be recognized and it will add a record (name, ID) in two csv files. First one is called
attendance.csv which contains records equivalent to how many times the face was detected. Another file called FinalAttendance.csv contains
records without duplication and is the final file which is to be looked at for the attendance.
