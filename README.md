# health-management
Hey everyone , I am new in git hub I don't know how to used it even properly 🤣 anyway joke aside here I uploading my first project  its name is HEALTH MANAGEMENT . IF someone who is working in small clinic or in a gym as trainer and you want to track data of your customer or patient here is a project its just a basic project. First use it and try it if you want to use it then I can contact me here is my email id-vishnu12911tomar@gmail.com you  can email me so I can update it according to your wish thank you 
Here is code:
Run it in your device 
def getdate():
    import datetime
    return datetime.datetime.now()
# #health management
b=input("what is your name=")
print("welcome to health management software",b.upper())
print("since, its under developing so you are able to enter report of 3 patients only")
patient1=input("enter patient1 name=")
patient2=input("enter patient2 name=")
patient3=input("enter patient3 name=")
choose_patient=input("enter your patient name that with you want to continue\n""write patient name here=")
data=input("what do you want to do about that patient\n1.exercise\n2.diet\n write here=")
operation=input("what do you want to do \n1.enter data\n2.read previous data\n type here your wish" +b.upper()+"=")
if choose_patient==patient1 and data=="exercise" and operation=="enter data":
    print("you are entering exercise done by",patient1)
    file_name=input("enter file name here=")
    i=input("press Y to continue and any other key to exit=")
    while i=="y":
        file_pointer=open(file_name,"a")
        exercise=input("enter exercise that "+patient1.upper()+"did today=")
        file_pointer.write(str([str(getdate())])+exercise+"\n")
        i = input("press Y to continue and any other key to exit=")
        file_pointer.close()
elif choose_patient==patient1 and data=="diet"and operation=="enter data":
    print("you are entering diet done by",patient1)
    file_name=input("enter file name here=")
    i=input("press Y to continue and any other key to exit")
    while i=="y":
        file_pointer=open(file_name,"a")
        diet=input("enter diet that "+patient1.upper()+"did today=")
        file_pointer.write(str([str(getdate())])+diet+"\n")
        i = input("press Y to continue and any other key to exit=")
        file_pointer.close()
        #patient2:
elif choose_patient==patient2 and data=="exercise"and operation=="enter data":
    print("you are entering exercise done by",patient2.upper())
    file_name=input("enter file name here=")
    i=input("press Y to continue and any other key to exit=")
    while i=="y":
        file_pointer=open(file_name,"a")
        exercise=input("enter exercise that "+patient2.upper()+"did today=")
        file_pointer.write(str([str(getdate())])+exercise+"\n")
        i = input("press Y to continue and any other key to exit=")
        file_pointer.close()
elif choose_patient==patient2 and data=="diet"and operation=="enter data":
    print("you are entering diet done by",patient2.upper())
    file_name=input("enter file name here=")
    i=input("press Y to continue and any other key to exit=")
    while i=="y":
        file_pointer=open(file_name,"a")
        diet=input("enter diet that "+patient2.upper()+"did today=")
        file_pointer.write(str([str(getdate())])+diet+"\n")
        i = input("press Y to continue and any other key to exit=")
        file_pointer.close()
#patient3::
elif choose_patient==patient3 and data=="exercise"and operation=="enter data":
    print("you are entering exercise done by",patient3.upper())
    file_name=input("enter file name here=")
    i=input("press Y to continue and any other key to exit=")
    while i=="y":
        file_pointer=open(file_name,"a")
        exercise=input("enter exercise that "+patient3.upper()+"did today=")
        file_pointer.write(str([str(getdate())])+exercise+"\n")
        i = input("press Y to continue and any other key to exit=")
        file_pointer.close()
elif choose_patient==patient3 and data=="diet"and operation=="enter data":
    print("you are entering diet done by",patient3.upper())
    file_name=input("enter file name here=")
    i=input("press Y to continue and any other key to exit=")
    while i=="y":
        file_pointer=open(file_name,"a")
        diet=input("enter diet that "+patient3.upper()+"did today=")
        file_pointer.write(str([str(getdate())])+diet+"\n")
        i = input("press Y to continue and any other key to exit=")
        file_pointer.close()
elif choose_patient==patient1 or patient2 or patient3 and data=="diet"or "exercise"and operation=="read previous data":
    print("you are reading ",data.upper(),"done by",choose_patient.upper())
    file_name = input("enter file name here=")
    file_pointer = open(file_name, "rt")
    print("here are ",data.upper(),"_","done by",choose_patient.upper())
    print(file_pointer.read())
    file_pointer.close()
