# ass-4-
task 1
filename = "simple.txt"

with open(filename, 'r') as file:
    print(f"Content of {filename}:")
    for line in file:
        print(line.strip()) 
task 2
filename = "simple.txt"

user_input = input("Enter text or a number to write in the file : ")

with open(filename, 'w') as file:
    file.write(user_input + "\n")
    print(f"Data successfully written to '{filename}'.")

user_input1 = input("Enter additional content to append : ")

with open(filename, 'a') as file:
    file.write(user_input1 + "\n") 
    
with open(filename, 'r') as file:
    final_content = file.read()

    print(f"\nFinal content of '{filename}':")
    print(final_content.strip()) 
