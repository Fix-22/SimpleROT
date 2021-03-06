# SimpleROT
A basic library made with Python, useful for encrypting strings or files with ROT cipher.

### Installation
```
pip install SimpleROT
```

## Get Started
Get started using ROT13 and ROTby methods.

### Use ROT13 Method
### String
How to encrypt a string with ROT13 cipher using SimpleROT library:
```Python
from SimpleROT import ROT

roted_string = ROT.ROT13("Hello World!")

print(roted_string) # This line prints on the console "Uryyb Jbeyq!"
```
### File
How to encrypt a file with ROT13 cipher using SimpleROT library:

### File: "test.txt"
On the "test.txt" file the text is:
```
hello
```
### File: "test.py"
```Python
from SimpleROT import ROT_file

txt_file = "test.txt"

roted_file = ROT_file.ROT13_file(txt_file)

print(roted_file) # This line returns "File 'test.txt' successfully encrypted"
```
### File: "test.txt"
Now the "test.txt" text is:
```
uryyb
```

### Use ROTby Method
### String
#### Encrypt
How to encrypt a string with ROTby method using SimpleROT library:
```Python
from SimpleROT import ROT

encrypted_string = ROT.ROTby_encrypt("Hello World!", 22) # Passing the number of letters to rotate as the second parameter

print(encrypted_string) # This line prints on the console "Dahhk Sknhz!"
```

#### Decrypt
How to decrypt a string with ROTby method using SimpleROT library:
```Python
from SimpleROT import ROT

decrypted_string = ROT.ROTby_decrypt("Dahhk Sknhz!", 22) # Passing the same number of letters to rotate as the second parameter

print(decrypted_string) # This line prints on the console "Hello World!"
```

### File
#### Encrypt
How to encrypt a file with ROTby method using SimpleROT library:

### File: "test.txt"
On the "test.txt" file the text is:
```
hello
```
### File: "test.py"
```Python
from SimpleROT import ROT_file

txt_file = "test.txt"

encrypted_file = ROT_file.ROTby_encrypt_file(txt_file, 22)

print(encrypted_file) # This line returns "File 'test.txt' successfully encrypted"
```
### File: "test.txt"
Now the "test.txt" text is:
```
uryyb
```
#### Decrypt
How to decrypt a file with ROTby method using SimpleROT library:

### File: "test.txt"
On the "test.txt" file the text is:
```
uryyb
```
### File: "test.py"
```Python
from SimpleROT import ROT_file

txt_file = "test.txt"

decrypted_file = ROT_file.ROTby_decrypt_file(txt_file, 22)

print(decrypted_file) # This line returns "File 'test.txt' successfully decrypted"
```
### File: "test.txt"
Now the "test.txt" text is:
```
hello
```
