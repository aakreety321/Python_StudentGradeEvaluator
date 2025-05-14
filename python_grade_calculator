 Predefined password
predefined_password = "loginsystem123"

# Number of login attempts
attempt=3
taken_attempt=0
access_granted = False
asking_user = 0

for taken_attempt in range(attempt):
    password=input("Enter the password")
    if password != predefined_password:
        left_attempt = attempt-(taken_attempt+1)
        print(f"Access denied. You have {left_attempt} attempts left.")
    else:
        access_granted= True
        break
if access_granted == False:
    print("You have used all your atttempts.")

else:
    # initializing an empty list to store subjects
    subjects = []
    for i in range(5):
        subject_name = input(f"Enter the name of subject {i + 1}: ")
        subjects.append(subject_name)
    for iteration in range(3):
        print(f"\n Attempt {iteration + 1}:")
        marks = []
        for subject in subjects:
            while True:
                try:
                    mark = float(input(f"Enter marks obtained in {subject}: "))
                    if 0 <= mark <= 100:
                        marks.append(mark)
                        break
                    else:
                        print("Please enter a valid mark between 0 and 100.")
                except ValueError:
                    print("Invalid input. Please enter a numeric value.")
        
        # Calculate percentage
        total_marks_obtained = sum(marks)
        percentage = (total_marks_obtained / 500) * 100
        
        # Calculate grade
        if percentage >= 90:
            grade = "A+"
            Remarks = " Outstanding, you did a great."
        elif percentage >= 80:
            grade = "A"
            Remarks = " Excellent, you should work a bit hard. "
        elif percentage >= 70:
            grade = "B+"
            Remarks = " Very good, you can achieve more with little hardwork. "
        elif percentage >= 60:
            grade = "B"
            Remarks = "Good, you must work hard. "
        elif percentage >= 50:
            grade = "C"
            Remarks = "Satisfactory, you have to focus more on studies"
        elif percentage >= 40:
            grade = "D"
            Remarks = " Acceptable, you should work too much on your studies. "
        else:
            grade = "E"
            Remarks = " Failed. "
        
        # Displaying results
        print(f"Percentage: {percentage:.2f}%")
        print(f"Grade: {grade}")
        print(f"Remark: {Remarks}")

    # buy package for using it
    print("\nPlease buy premium package for more result calculations.")
