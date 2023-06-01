# Random-Password-Generator
Random Password Generator
import random
import string

def generate_random_password(length):
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(random.choice(characters) for _ in range(length))
    return password

# Example Usage
password_length = 10
random_password = generate_random_password(password_length)
print("Randomly Generated Password:", random_password)
