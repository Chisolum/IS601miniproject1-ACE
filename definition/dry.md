## Don't Repeat Yourself    


Don't repeat yourself (DRY, or sometimes do not repeat yourself) is a principle of software development aimed at reducing repetition of software patterns, replacing it with abstractions or using data normalization to avoid redundancy. The Don’t Repeat Yourself (DRY) principle states that duplication in logic should be eliminated via abstraction; duplication in process should be eliminated via automation. Adding additional, unnecessary code to a codebase increases the amount of work required to extend and maintain the software in the future.  Duplicate code adds to technical debt.  Whether the duplication stems from Copy Paste Programming or poor understanding of how to apply abstraction, it decreases the quality of the code.   

A simple example  

To calculate the BMI of five subjects. Here is how we could do it in Python:    

># Subject data = [weight_kg, height_m]
>subject1 = [80, 1.62]
>subject2 = [69, 1.53]
>subject3 = [80, 1.66]
>subject4 = [80, 1.79]
>subject5 = [72, 1.60]

>bmi_subject1 = int(subject1[0] / subject1[1]**2)
>print("bmi {} = {}".format('subject1', bmi_subject1))

>bmi_subject2 = int(subject2[0] / subject2[1]**2)
>print("bmi {} = {}".format('subject2', bmi_subject2))

>bmi_subject3 = int(subject3[0] / subject3[1]**2)
>print("bmi {} = {}".format('subject3', bmi_subject3))

>bmi_subject4 = int(subject4[0] / subject4[1]**2)
>print("bmi {} = {}".format('subject4', bmi_subject4))

>bmi_subject5 = int(subject5[0] / subject5[1]**2)
>print("bmi {} = {}".format('subject5', bmi_subject5))
>The code produces the expected output:
>bmi subject1 = 30
>bmi subject2 = 29
>bmi subject3 = 29
>bmi subject4 = 24
>bmi subject5 = 28

   

While the above code works, it required a lot of typing, retyping and cut-and-pasting. It is a good idea to adhere to the DRY principle when writing computer code: don’t repeat yourself.  The code can be made more reliable code by using functions in Python.  The code below followed the dry principle by using a for loop to reduce additional repetition in the code, using a list of lists to hold the subjects’ data. Each internal list holds the data for a subject, and the subject number along with their weight and height was added. The code now uses a for loop to call bmi_calc() function for each subject. Overall, the code is shorter, easier to read, and easier to maintain.    

>def bmi_calc(sub_num, weight_kg, height_m):
 >   """Calculate BMI from weight in kg and height in meters"""
 >   bmi = int(weight_kg / height_m**2)
 >   subject = 'subject' + str(sub_num)
 >   print("bmi {} = {}".format(subject, bmi))

># Subject data = [weight_kg, height_m]
>subjects =[[1, 80, 1.62], # subject1
           [2, 69, 1.53], # subject2
           [3, 80, 1.66], # subject3
           [4, 80, 1.79], # subject4
           [5, 72, 1.60]] # subject5

>for sub in subjects:
    bmi_calc(sub[0], sub[1], sub[2])  

