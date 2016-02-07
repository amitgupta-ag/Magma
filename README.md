# Magma
TwoFish ENcryption and Decryption Algorithm implemented on Magma
In cryptography, Twofish is a symmetric key block cipher with a block size of 128 bits and key sizes up to 256 bits. It was one of the five finalists of the Advanced Encryption Standard contest, but it was not selected for standardization. Twofish is related to the earlier block cipher Blowfish.

Twofish's distinctive features are the use of pre-computed key-dependent S-boxes, and a relatively complex key schedule. 
One half of an n-bit key is used as the actual encryption key and the other half of the n-bit key is used to modify the encryption algorithm (key-dependent S-boxes). 
Twofish borrows some elements from other designs; for example, the pseudo-Hadamard transform (PHT) from the SAFER family of ciphers. 
Twofish has a Feistel structure like DES.

Twofish was designed by Bruce Schneier, John Kelsey, Doug Whiting, David Wagner, Chris Hall, and Niels Ferguson; 
the "extended Twofish team" who met to perform further cryptanalysis of Twofish and other AES contest entrants included Stefan Lucks, Tadayoshi Kohno, and Mike Stay.

The Twofish cipher has not been patented and the reference implementation has been placed in the public domain. 
As a result, the Twofish algorithm is free for anyone to use without any restrictions whatsoever.

This file is in .txt format. But to run the code on Magma (http://magma.maths.usyd.edu.au/magma/download/), you don't really need a file format. you can just run the file object.


======================================================================================================================

INSTRUCTIONS TO RUN FOR AN ARRAY OF PLAIN TEXTS::
======================================================================================================================

➢	load “TwoFish.txt”;
➢	PT:= ["80000000000000000000000000000000","40000000000000000000000000000000","20000000000000000000000000000000","10000000000000000000000000000000","08000000000000000000000000000000","04000000000000000000000000000000","02000000000000000000000000000000","01000000000000000000000000000000","00800000000000000000000000000000","00400000000000000000000000000000"]
➢	K128:= "00000000000000000000000000000000";
➢	K192:= "000000000000000000000000000000000000000000000000";
➢	K256:= "0000000000000000000000000000000000000000000000000000000000000000";
➢	EncriptArrayOfPlaintext(K128,PT);
➢	EncriptArrayOfPlaintext(K192,PT);
➢	EncriptArrayOfPlaintext(K256,PT);

======================================================================================================================

INSTRUCTIONS TO RUN FOR A SINGLE ENCRYPTION::
======================================================================================================================

➢	K:="00000000000000000000000000000000";
➢	P:="80000000000000000000000000000000";
➢	TwoFish_Encryption(K,P);

======================================================================================================================

INSTRUCTIONS TO RUN DECRIPTION OF SINGLE CIPHER::
======================================================================================================================

➢	K:="0000000000000000000000000000000000000000000000000000000000000000";
➢	C:="630075C7563CDBACDFEADB781CC9467C";
➢	Twofish_Decryption(K,C);