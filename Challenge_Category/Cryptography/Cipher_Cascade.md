# Cipher Cascade 
> **Category:** Cryptography

**Flag format:** ``CSCUU{some_text}``

## Challenge Description:

Welcome to the Mystery Challenge. Your task is to decode it and determine the next steps.Welcome to the Mystery Challenge. Your task is to decode it and determine the next steps.

**Encrypted Text:** UjNWeUlGTjViblFnZG1ZNklGQkdVRWhJZTBvemVYbHdNSHB5WDBjd1gxQnNiek5GWDBZemNHaGxkbWRzWDFCNWFHOWZTRWg5


---

## Approach:

First, I carefully read the problem. It contains an encrypted text that looks like Base64.  
I went to a Base64 decoder and decoded the text once.  

![First Decode Screenshot](../Image_Folder/cipher_cascade_1.jpg)

  
**The decoded result was:** ``R3VyIFN5bnQgdmY6IFBGUEhIe0ozeXlwMHpyX0cwX1BsbzNFX0YzcGhldmdsX1B5aG9fSEh9``
This output also looked like Base64, so I decoded it again.



![Second Decode Screenshot](../Image_Folder/cipher_cascade_2.jpg)
**The second decoded result was:**  ``Gur Synt vf: PFPHH{J3yyp0zr_G0_Plo3E_F3phevgl_Pyho_HH}``


Although the question gave a hint, I still verified the cipher type using [dCode Cipher Identifier](https://www.dcode.fr/cipher-identifier).  


It confirmed the cipher is ROT13.  
![Cipher Identifier Screenshot](../Image_Folder/cipher_cascade_3.jpg)

So, I applied ROT13 decryption. 

![Final Decode Screenshot](../Image_Folder/cipher_cascade_4.jpg)

Yay! By decoding layer after layer, we successfully found the flag.

**The final decrypted flag was:**  

