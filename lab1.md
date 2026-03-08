1. Determining the Correct Symmetric Key 

Three 128 -bit keys are given in HEX format: 

68544020247570407220244063724074 
54684020247570407220244063724074 
54684020247570407220244063727440 

The SHA -256 hash of the correct key is also provided: 

f28fe539655fd6f7275a09b7c3508a3f81573fc42827ce34ddf1ec8d5c2421c3 

The SHA -256 hash was calculated for each key and compared with the given  value. A match was found for the second key. 

Correct Symmetric Key: 

54684020247570407220244063724074 

2. AES -128 CBC Decryption 

Encrypted message (HEX): 

876b4e970c3516f333bcf5f16d546a87aaeea5588ead29d213557efc1903997e 

Initialization Vector (IV): 

656e6372797074696f6e496e74566563 

Algorithm: AES -128 CBC Using the identified symmetric key and the provided IV, the message was decrypted. 

Decrypted message 

Hello Blockchain! 

3. Generation of an asymmetric key pair 

An RSA asymmetric key pair was generated. 

Public Key 

-----BEGIN PUBLIC KEY -----

MIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAh2jtnm57LMsshwp86Uu7 

WcHMN6cMoevUN8IFUwpelJghkfFMIOBxmIzqS1rwq63ZUnIBpUAxU3xLmi5t6LTZ 

9JMy2UOoM4O77UufvuVETr395LQLtr5vva35B7ECJz5ywFYo8+o6p9gsG+4S4ilP 

U1EtOspCKaqr5gvGg1iHot3ZqE9qtUbPGOd1fwbggPA7Ttc9pMTmKOHJM0 I+kDn+ 

ILtwGyySpeB1QzSKr81h1XqZeU0GGUb1dcVUil3Iioe6dXsXCF27ut6dA0WX2VO0 

8FfwHsfOv5fuGqnCG6dx1pHXJMnxaxYPGA28gXkqgo5dcO86gcPvdmzQ0pioP3FE 

VwIDAQAB 

-----END PUBLIC KEY -----

The private key was used to create a digital signature. 4. Creating a Digital Signature 

The following algorithm was used to sign the message: 

SHA256withRSA 

Message to be signed: 

Hello Blockchain! 

The result is a digital signature generated using the private key. 

5. Explanation 

First, the SHA -256 hash was computed for each of the three proposed symmetric  keys. The resulting values were compared with the provided hash of the correct key. A match was found for the second key, which was then chosen as the correct symmetric key. After that, th e encrypted message was decrypted using the AES -128 algorithm in CBC mode. The discovered key and the provided initialization vector were used for decryption. As a result, the original message was obtained: “Hello Blockchain!” .