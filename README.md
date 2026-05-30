# Student Result Management System..
#input student name
name = input("Enter student name: ")

# input number of subjects
subjects = int(input("Enter number of subjects:"))

total = 0

# loop for entering marks
for i in range(subjects):
    marks = float(input(f"Enter your subject marks {i+1}: "))
    total = total + marks

# Calculate average  
average = total / subjects 

# detemine grade
if average >= 80:
     grade = 'A'
elif average >= 70:
     grade = 'B'
elif average >= 60:
    grade = 'C'
elif average >= 50:
    grade = 'D'
else:
    grade ='F'

    #Display Results
print("\n ----STUDENT RESULTS-----")
print("Student Name:", name)
print("Total Marks:", total)
print("Average:", average)  
print("Grade:", grade)  
