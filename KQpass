import random

# alphabet for encryption
alphabet = {
    "A": "1b_", "B": "C7!", "C": "1v^", "D": "5d*", "E": "4e&", "F": "1w@", "G": "6v!",
    "H": "2Z&", "I": "1f^", "J": "4A%", "K": "2*n", "L": "4m}", "M": "u5-", "N": "6t_",
    "O": "2Q$", "P": "6g#", "Q": "2y@", "R": "0o!", "S": "6h<", "T": "K1>", "U": "3g?",
    "V": "9o=", "W": "1R~,", "X": "2b.", "Y": "1o^", "Z": "5S*", " ": "5y'"
    }
# dictionary for encryption
words = ["apple", "anime", "hand", "fruit", "human", "kid", "gold", "physics", "house",
         "people", "code", "program", "math", "go", "hello", "man", "men", "woman", "age",
         "mathematics", "history", "one", "word", "ten", "equation", "function", "chemistry",
         "cryptography", "algorithm", "variable", "digit", "integer", "dark", "light", "electro",
         "programming", "coding", "mouse", "click", "error", "dog", "cat", "computer",
         "mass", "energy", "eye", "stand", "buddha", "sword", "key", "hard", "car",
         "school", "univercity", "you", "he", "she", "it", "character", "computer science",
         "data science", "analysis", "health", "hospital", "arm", "brain", "right",
         "true", "false", "plus", "minus", "game", "ball", "manga", "event", "if",
         "else", "joke", "sheep", "ship", "pig", "tank", "country", "number", "abillity",
         "god", "talent", "genius", "two", "language", "gay", "science", "book", "algebra",
         "geometry", "statistics", "logic", "probability", "text", "introduction"]

# function for creating password
def create_password():
    word = random.choice(words)
    word = word.upper()
    password = ""
    for i in range(len(word)):
        add_int = str(random.randint(0, 9))
        if word[i] in alphabet:
            password += alphabet[word[i]] + add_int
    
    return password

# function for checking password
def check_password(password):
    while len(password) > 20 or len(password) < 12:
        if len(password) > 20:
            password = password[:20]
        elif len(password) < 12:
            password += str(random.randint(0, 9))
    return password

# process of program
while True:
    user_input = input("Press Enter for generate password or q for exit \n")
    if user_input.lower() == "q":
        exit()
    
    password = create_password()
    password = check_password(password)
    print(password, "\n")
