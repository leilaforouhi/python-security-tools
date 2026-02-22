import secret
import string

def create_password(length=16):
    characters = string.ascii_letters + string.digits + string.punctuation
    password = ''.join(secrets.choice(characters) for _ in range(length))
    return password

print(f"Your secure password: {create_password()}")
