> Vigenere-Cipher
Encoding and Decoding messages with Vigenere Cipher


In this python algorithm, we are shifting the characters of the message using the key provided to encrypt and decrypt messages.

Can be used as a means of storing passwords on a computer using by many other users.

![image](https://user-images.githubusercontent.com/62197789/152675490-5254c034-4d7e-48e1-9d39-58c28b39c671.png)


Vigenere Cipher is a method of encrypting alphabetic text. It uses a simple form of polyalphabetic substitution. A polyalphabetic cipher is any cipher based on substitution, using multiple substitution alphabets. The encryption of the original text is done using the Vigenère square or Vigenère table.


The table consists of the alphabets written out 26 times in different rows, each alphabet shifted cyclically to the left compared to the previous alphabet, corresponding to the 26 possible Caesar Ciphers.


At different points in the encryption process, the cipher uses a different alphabet from one of the rows.


The alphabet used at each point depends on a repeating keyword.

=================================================================================================================================================================================

Example: 

Input : Plaintext :   PYTHON
             Keyword :  ABC
Output : Ciphertext :  PZVHPC
For generating key, the given keyword is repeated
in a circular manner until it matches the length of 
the plain text.
The keyword "ABC" generates the key "ABC"
The plain text is then encrypted using the process 
explained below.

=================================================================================================================================================================================

Encryption :

The first letter of the plaintext, P is paired with A, the first letter of the key. So use row P and column A of the Vigenère square. Similarly, for the second letter of the plaintext Y, the second letter of the key B is considered.So use row Y and column B of the Vigenère square. The rest of the plaintext is enciphered in a similar fashion. 

=================================================================================================================================================================================

Decryption :

Decryption is performed by going to the row in the table corresponding to the key, finding the position of the ciphertext letter in this row, and then using the column’s label as the plaintext.

=================================================================================================================================================================================
