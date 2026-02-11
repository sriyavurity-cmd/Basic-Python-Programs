11/02/25

# **PLACEMENT TRAINING- Technical (PYTHON)** 



###### **1-Perform a basic account operation like withdraw , deposit. Initialize the balance with 5000. Take user input based on choice. Perform withdraw, deposit, use switch case.** 

###### **Input: choose what you want to do**

###### **withdraw**

###### **2. deposit** 

###### **3. display balance** 

###### **4. exit** 



\# Initialize balance

balance = 5000



while True:

&nbsp;   print("\\nChoose what you want to do:")

&nbsp;   print("1. Withdraw")

&nbsp;   print("2. Deposit")

&nbsp;   print("3. Display Balance")

&nbsp;   print("4. Exit")



&nbsp;   choice = int(input("Enter your choice (1-4): "))



&nbsp;   match choice:

&nbsp;       case 1:

&nbsp;           amount = float(input("Enter amount to withdraw: "))

&nbsp;           if amount <= balance:

&nbsp;               balance -= amount

&nbsp;               print("Withdrawal successful.")

&nbsp;               print("Remaining Balance:", balance)

&nbsp;           else:

&nbsp;               print("Insufficient balance!")



&nbsp;       case 2:

&nbsp;           amount = float(input("Enter amount to deposit: "))

&nbsp;           balance += amount

&nbsp;           print("Deposit successful.")

&nbsp;           print("Updated Balance:", balance)



&nbsp;       case 3:

&nbsp;           print("Current Balance:", balance)



&nbsp;       case 4:

&nbsp;           print("Thank you! Exiting program.")

&nbsp;           break



&nbsp;       case \_:

&nbsp;           print("Invalid choice! Please select between 1-4.")

*OUTPUT:* 

*Choose what you want to do:*

*1. Withdraw*

*2. Deposit*

*3. Display Balance*

*4. Exit*

*Enter your choice (1-4): 1*

*Enter amount to withdraw: 1000*

*Withdrawal successful.*

*Remaining Balance: 4000.0*



*Choose what you want to do:*

*1. Withdraw*

*2. Deposit*

*3. Display Balance*

*4. Exit*

*Enter your choice (1-4): 2*

*Enter amount to deposit: 3000*

*Deposit successful.*

*Updated Balance: 7000.0*



*Choose what you want to do:*

*1. Withdraw*

*2. Deposit*

*3. Display Balance*

*4. Exit*

*Enter your choice (1-4): 4*

*Thank you! Exiting program.*





###### <b>2-Use for loop and generate the following output</b>

###### <b>1</b>

###### <b>1 2</b>

###### <b>1 2 3</b>



for i in range(1, 4):

&nbsp;   for j in range(1, i + 1):

&nbsp;       print(j, end="   ")

&nbsp;   print()



*OUTPUT:*

*1*

*1 2*

*1 2 3*



###### 3-**Use for loop and generate the following output**

######  **\*\*\*\***

######  **\*A\*\***

######  **\*AB\*\***

######  **\*ABC**



for i in range(4):

&nbsp;   print("\*", end="")

print()



letters = "ABC"



for i in range(3):

&nbsp;   print("\*", end="")

&nbsp;   for j in range(i + 1):

&nbsp;       print(letters\[j], end="")

&nbsp;   for k in range(2 - i):

&nbsp;       print("\*", end="")

&nbsp;   print()



*OUTPUT:*

*\*\*\*\**

*\*A\*\**

*\*AB\*\**

*\*ABC*



###### 

###### **4-Write a program to generate the multiplication table of a given number up to a user-defined limit. The program should prompt the user to enter the table number and the limit. Use a for loop to display the multiplication table and a while loop to allow the user to repeat the process. After displaying each table, the program should ask the user whether they want to continue. If the user enters yes, the program should repeat; otherwise, it should terminate.** 



choice = "yes"



while choice.lower() == "yes":

&nbsp;   num = int(input("Enter table number: "))

&nbsp;   limit = int(input("Enter limit: "))



&nbsp;   # Using FOR loop to generate table

&nbsp;   for i in range(1, limit + 1):

&nbsp;       print(num, "\*", i, "=", num \* i)



&nbsp;   choice = input("Do you want to continue? (yes/no): ")









*OUTPUT:*



*Enter table number: 5*

*Enter limit: 15*

*5 \* 1 = 5*

*5 \* 2 = 10*

*5 \* 3 = 15*

*5 \* 4 = 20*

*5 \* 5 = 25*

*5 \* 6 = 30*

*5 \* 7 = 35*

*5 \* 8 = 40*

*5 \* 9 = 45*

*5 \* 10 = 50*

*5 \* 11 = 55*

*5 \* 12 = 60*

*5 \* 13 = 65*

*5 \* 14 = 70*

*5 \* 15 = 75*

*Do you want to continue? (yes/no): YES*

*Enter table number: 4*

*Enter limit: 20*

*4 \* 1 = 4*

*4 \* 2 = 8*

*4 \* 3 = 12*

*4 \* 4 = 16*

*4 \* 5 = 20*

*4 \* 6 = 24*

*4 \* 7 = 28*

*4 \* 8 = 32*

*4 \* 9 = 36*

*4 \* 10 = 40*

*4 \* 11 = 44*

*4 \* 12 = 48*

*4 \* 13 = 52*

*4 \* 14 = 56*

*4 \* 15 = 60*

*4 \* 16 = 64*

*4 \* 17 = 68*

*4 \* 18 = 72*

*4 \* 19 = 76*

*4 \* 20 = 80*

*Do you want to continue? (yes/no):no*





   

###### <b>5.ex: 3</b>

num=3



if num>0 and num<20:

&nbsp; print ("number between 0 and 20")

if 10<num<20:

&nbsp; print ("number between 10 and 20")



*OUTPUT:* 

*number between 0 and 20*



###### <b>5.ex:12</b>



num=12



if num>0 and num<20:

&nbsp; print ("number between 0 and 20")

if 10<num<20:

&nbsp; print ("number between 10 and 20")



*OUTPUT:*

*number between 0 and 20*

*number between 10 and 20*



###### <b>6. Takes a size number from user, Uses condition chaining (if–elif–else),Displays whether the size is Small (38), Medium (40), or Large (42)</b>



size = int(input("Enter the size (38 / 40 / 42): "))



if size == 38:

&nbsp;   print("Small Size Selected")

elif size == 40:

&nbsp;   print("Medium Size Selected")

elif size == 42:

&nbsp;   print("Large Size Selected")

else:

&nbsp;   print("Invalid Size Entered")



*OUTPUT:* 

*Enter the size (38 / 40 / 42): 40*

*Medium Size Selected*



<b>7.Once upon a time in the city of Mysore, there lived a young programmer named Arjun. He</b>

<b>was known for curiosity in solving problems with creative coding solutions. One day, Arjun</b>

<b>received an urgent message from the town's mayor. The problem was simple yet crucial: the</b>

<b>system needed to handle book IDs entered by librarians as integers but store them as floats for</b>

<b>better data management and future scalability. Determined to help, Arjun ensured that each</b>

<b>book ID was correctly converted and stored.</b>



x = int(input("Enter the integer: "))

print("The floating point:",float(x))



*OUTPUT:*

*Enter the integer: 55*

*The floating point: 55.0*



<b>8.In the enchanted village, there lived a brilliant coder named Samara. She was known for her</b>

<b>talent in weaving spells with her code, solving problems that seemed almost impossible to</b>

<b>others. Accepting the challenge, Samara set up her coding station under the village's great</b>

<b>wisdom tree, where the air was filled with the whispers of past knowledge. She knew she had</b>

<b>to write a script that could take a string input, convert it into an integer, and then display both</b>

<b>the original string and the converted integer for validation</b>



x = input("Enter the string: ")

print(x)

print("The integer point:",int(x))



*OUTPUT:*

*Enter the string: 3*

*3*

*The integer point: 3*



###### <b>9.Swap the values of two variables using the operators. Print the values before and after the swap.</b>



P = int( input("Please enter value for P: "))

Q = int( input("Please enter value for Q: "))

\# To swap the value of two variables

\# we will user third variable which is a temporary variable

temp\_1 = P

P = Q

Q = temp\_1

print ("The Value of P after swapping: ", P)

print ("The Value of Q after swapping: ", Q)





*OUTPUT:*

*Please enter value for P: 5*

*Please enter value for Q: 7*

*The Value of P after swapping:  7*

*The Value of Q after swapping:  5*



