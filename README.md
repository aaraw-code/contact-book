# contact-book
store contact details 

contact = {}

while True:
    print("\nContact Book App")
    print("1. Create contact")
    print("2. View contact")
    print("3. update contact")
    print("4. Delete contact")
    print("5. Search contact")
    print("6. Count contact")
    print("7. Exit")


    user_input = input("Enter your choice: ")

    if user_input == "1":
        name = input("Enter your name: ")
        if name in contact:
            print(f"This {name} is already exist!")
        else:
                
            age = int(input("Enter age: "))
            email = input("Enter email: ")
            mobile = input("Enter mobile number: ")
                

            with open("demo.txt","a") as file:
                file.write(f" name {name}\n")
                file.write(f"email {email}\n")
                file.write(f"mobile no {mobile}\n")


        print("Your record has been saved succesfully!")
