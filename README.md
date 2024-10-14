Secret Code Generator

This project is a simple command-line application for encoding and decoding messages using a Caesar Cipher. The Caesar Cipher is a basic encryption technique where each letter in the message is shifted by a specific number of positions in the alphabet. This program allows users to encode messages, decode them back to their original form, or exit the program.

Features

Encode a Message: Enter a message and shift value to encode it with the Caesar Cipher.

Decode a Message: Enter an encoded message and the original shift value to decode it back to its original form.

Input Validation: Prompts the user to re-enter the shift value if an invalid (non-integer) value is provided.


How to Use

1. Run the program.


2. Choose one of the following options:

1: Encode a message.

2: Decode a message.

3: Exit the program.



3. Follow the prompts to input our message and shift value.


4. The program will display the encoded or decoded message as per your choice.



Functions

encode_message(message, shift)

Purpose: Encodes a message using the Caesar Cipher by shifting each letter by a specified number of positions.

Parameters:

message (str): The message to encode.

shift (int): The number of positions to shift each letter.


Returns: A string representing the encoded message.

Details:

Each uppercase letter is shifted within the uppercase alphabet.

Each lowercase letter is shifted within the lowercase alphabet.

Non-letter characters remain unchanged.



decode_message(encoded_message, shift)

Purpose: Decodes a message encoded with the Caesar Cipher by reversing the shift on each letter.

Parameters:

encoded_message (str): The message to decode.

shift (int): The number of positions each letter was originally shifted.


Returns: A string representing the decoded message.

Details:

Each uppercase letter is reversed within the uppercase alphabet.

Each lowercase letter is reversed within the lowercase alphabet.

Non-letter characters remain unchanged.



secret_code_generator()

Purpose: Handles user interaction with the program through a menu interface.

Details:

Continuously displays a menu with three options: encoding, decoding, or exiting.

Based on the user's choice:

If encoding, prompts for a message and shift value, then displays the encoded message.

If decoding, prompts for an encoded message and shift value, then displays the decoded message.

If exiting, terminates the program.


Checks for valid integer input for the shift value and prompts the user to re-enter if invalid input is detected.



Main Execution Block

if _name_ == "_main_":
    secret_code_generator()
