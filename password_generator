import string
import random

RED = "\033[91m"
LIGHT_GREEN = "\033[38;5;114m"
GREEN = "\033[92m"  
RESET = "\033[0m"

length = input("How long you want your password to be? (atleast 8) : ")

lower_case = list(string.ascii_lowercase)
upper_case = list(string.ascii_uppercase)
numbers = list(string.digits)
punctuations = list(string.punctuation)

while(True):
    
    try:
        char_len = int(length)
        if char_len < 8:
            print(f"{RED}Your number should be atleast 8 !!{RESET}")
            length = input(f"Please enter your number again: ")
        else:
            break
    except:
        print(f"{RED}Please enter numbers only.{RESET}")
        length = input(f"How long you want your password to be? (atleast 8): ")

random.shuffle(lower_case)
random.shuffle(upper_case)
random.shuffle(numbers)
random.shuffle(punctuations)

char_count = round(char_len * 30/100)
symb_count = round(char_len * 20/100)

password = []

for x in range(char_count):
    password.append(lower_case[x])
    password.append(upper_case[x])

for x in range(symb_count):
    password.append(numbers[x])
    password.append(punctuations[x])

random.shuffle(password)

strong_password = "".join(password)
print(f"{LIGHT_GREEN}Strong Password:{RESET} {GREEN}{strong_password}{RESET}")