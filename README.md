# EX. NO: 1(A) : IMPLEMENTATION OF CAESAR CIPHER

## AIM:
To implement the simple substitution technique named Caesar cipher using C language.

## ALOGORITHM:

STEP-1: Read the plain text from the user.

STEP-2: Read the key value from the user.

STEP-3: If the key is positive then encrypt the text by adding the key with each character in the plain text.

STEP-4: Else subtract the key from the plain text.

STEP-5: Display the cipher text obtained above.

## PROGRAM:
```

#include <stdio.h>

int main() {
    char text[] = "POOJA", enc[100], dec[100];
    int key = 3, i;

    for (i = 0; text[i] != '\0'; i++)
        enc[i] = (text[i] - 'A' + key) % 26 + 'A';
    enc[i] = '\0';

    for (i = 0; enc[i] != '\0'; i++)
        dec[i] = (enc[i] - 'A' - key + 26) % 26 + 'A';
    dec[i] = '\0';

    printf("Enter the plain text: %s\n", text);
    printf("Enter the Key value: %d\n", key);
    printf("PLAIN TEXT: %s\n", text);
    printf("ENCRYPTED TEXT: %s\n", enc);
    printf("DECRYPTED TEXT: %s\n", dec);

    return 0;
}
```

## OUTPUT:
<img width="1920" height="1080" alt="output" src="https://github.com/user-attachments/assets/1b421c0b-159b-47f1-ae3d-6017b96d2326" />



## RESULT :
 Thus the implementation of ceasar cipher had been executed successfully.
