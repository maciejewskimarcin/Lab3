# 1
import logging
from datetime import datetime

def get_logs(level):
    log_format = "%(levelname)s: %(asctime)s - %(message)s"
    logging.basicConfig(level=level, format=log_format, datefmt='%Y-%m-%d %H:%M:%S')
    logging.debug("Debug at {}".format(datetime.now()))
    logging.info("Info at {}".format(datetime.now()))
    logging.warning("Warning at {}".format(datetime.now()))
    logging.error("Error at {}".format(datetime.now()))
    logging.critical("Critical at {}".format(datetime.now()))


get_logs(logging.DEBUG)

# 2
import base64

def encrypt_decrypt_base64():
    while True:
        string = input("Wprowadź wiadomość do zaszyfrowania lub odszyfrowania: ")
        try:
            decoded_string = base64.b64decode(string).decode()
            print("Odszyfrowana wiadomość:",decoded_string)
        except:
            encoded_string = base64.b64encode(string.encode()).decode()
            print("Zaszyfrowana wiadomość:",encoded_string)
        again = input("Chcesz jeszcze raz? (y/n)")
        if again.lower() != "y":
            break

encrypt_decrypt_base64()

# 3
import random
import string

def generate_password():
    while True:
        characters = string.ascii_letters + string.digits + string.punctuation
        length = int(input("Podaj długość hasła (minimum 8 znaków): "))
        if length<8:
            print("Długość hasła to minimum 8 znaków")
        else:
            password = ''.join(random.choice(characters) for _ in range(length))
            print("Hasło: ",password)
            again = input("Jeszcze raz? (y/n)")
            if again.lower() != "y":
                break
    return password

generate_password()
