# EX-8-ADVANCED-ENCRYPTION-STANDARD ALGORITHM
## NAME : BASKAR.U
## REG.NO : 212223220013
# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
AES is based on a design principle known as a substitution–permutation.
AES does not use a Feistel network like DES, it uses variant of Rijndael.
It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.
AES operates on a 4 × 4 column-major order array of bytes, termed the state
# PROGRAM:
```c
 #include <stdio.h>
 Preview Code Blame Raw
 Sign in
#include <string.h>
 void xor_encrypt_decrypt(char *input, char *key) {
 int input_len = strlen(input);
 int key_len = strlen(key);
 for (int i = 0; i < input_len; i++) {
 input[i] = input[i] ^ key[i % key_len];
 }
 }
 int main() {
 printf("\n\n\n\n      
char url[] = "WELCOME";
 char key[] = "secretkey"; 
printf("Original text: %s\n", url);
 xor_encrypt_decrypt(url, key);
 printf("Encrypted text: %s\n", url);
 return 0;
 }
 ***** ADVANCED-ENCRYPTION-STANDARD-DES-ALGORITHM *
 xor_encrypt_decrypt(url, key);
 printf("Decrypted text: %s\n", url)
```
# OUTPUT:
![Screenshot 2025-04-24 232642](https://github.com/user-attachments/assets/ec52574a-fbeb-4a6f-923f-d1458385628c)

# RESULT:
 The expriment is successfully Executed.


