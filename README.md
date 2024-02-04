# Python programming language
# Output-of-a-letter-by-value
# The first option:
the_english_alphabet = ['A', 'B', 'C', 'D', 'E', 'F', 'G',
                        'H', 'I', 'J', 'K', 'L', 'M', 'N',
                        'O', 'P', 'Q', 'R', 'S', 'T', 'U',
                        'V', 'W', 'X', 'Y', 'Z']

print("The English alphabet...Go", *the_english_alphabet, sep='->')

while True:
    print('\n')
    enter_value: int = int(input("Enter value from 1 to 26: "))
    if 0 < enter_value <= 26:
        print('The letter of the alphabet: ',
              the_english_alphabet[enter_value-1] +
              the_english_alphabet[enter_value-1].lower(), '\n')
    else:
        print("Incorrect value! Repeat again!")

# The second option:
while True:
    enter_value: int = int(input('Enter value: '))
    if 0 < enter_value <= 26:
        print('Your letter:', (chr(ord('A') + enter_value - 1) +
                               chr(ord('a') + enter_value - 1)))
    else:
        print("Incorrect value! Repeat again!")
