# Define the term “hashing”.
hashing refers to the process of converting sensitive data, like passwords, into a fixed-length string using a specific algorithm. This transformed string, known as a hash value, is employed for security purposes. Spring offers tools to facilitate secure practices, particularly in Spring Security for user authentication. Hashing involves selecting an algorithm and using it to convert data, with the resulting hash stored for verification rather than the original information. This safeguards sensitive data, making it computationally difficult to retrieve even if a database is compromised.

# Explain to a non-technical friend what a hash function does to a password.

Imagine a hash function like a special kind of machine that takes something you want to keep safe, like a password, and turns it into a secret code.

Here's how it works:

Input: You give the machine your password.

Magic Process: The machine performs some fancy calculations on your password, turning it into a completely different set of characters. It's like a secret recipe that only the machine knows.

Output: What comes out of the machine is a unique, jumbled-up code. This code doesn't look anything like your original password.

# What does it mean to ‘salt’ a password?

Salting" a password is a security practice used to enhance the protection of stored passwords. It involves adding random data, known as a "salt," to the original password before it's hashed.
 # What piece of information would a hacker need to access in order to find the ‘salt’ string for your passwords?

To find the "salt" string associated with a user's password, a hacker would typically need to gain unauthorized access to the database where the passwords are stored. The salt is typically stored alongside the hashed password in the database, so if the hacker can somehow access this information, they would also have access to the corresponding salt.

# How does the Blowfish block cipher handle the increased computation speed of new computers?
The Blowfish block cipher, as utilized in jBCrypt, adapts to the increasing speed of computers through a parameter called "log_rounds". This parameter controls the computational complexity of the algorithm by determining the number of iterations. As "log_rounds" increases, so does the number of iterations, making the hashing process more computationally intensive. This adaptive feature frustrates attempts to crack passwords by leveraging fast hardware. In essence, it ensures that even with advancements in computing power, the security of password hashing is maintained.


# What are the issue with the two most commong password hashes for Java (“Java password hash” and “Java password encryption”)?
The two most commonly found approaches for password hashing in Java, often obtained through searches for "Java password hash" and "Java password encryption," have notable security issues:

Unsalted Hashing:

One of the common approaches involves using an unsalted hash. This means that the password is hashed without the addition of a unique random value (salt).
Problem: Without salting, identical passwords will produce the same hash. This allows attackers to perform a reverse lookup using precomputed tables (like rainbow tables) to discover passwords. It's a significant security vulnerability.
Reversible Encryption:

Another approach advises reversible encryption of passwords.
Problem: Reversible encryption means that there is a way to decrypt the password back to its original form. This is a major security risk. In the event of a security breach, encrypted passwords can be potentially decrypted, exposing user credentials.