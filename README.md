import random
import string

print("====================================")
print("        PASSWORD GENERATOR")
print("====================================")

# Get password length from the user
length = int(input("Enter the password length: "))

# Characters that can be used
characters = string.ascii_letters + string.digits + string.punctuation

# Generate the password
password = ""

for i in range(length):
    password += random.choice(characters)

# Display the password
print("\nGenerated Password:", password)

print("\nPassword generated successfully!")
