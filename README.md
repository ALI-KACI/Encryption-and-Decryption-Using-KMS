# Encryption-and-Decryption-Using-KMS

## Purpose of the Hands on

Create AWS KMS key for encrypting data at rest and performing server-side encryption. AWS KMS addresses this by storing customer master keys, which can directly perform encryption or generate unique symmetric data keys. These data keys, whether 128 or 256 bits, are encrypted using the customer master key.

## Architecture

![Architecture for KMS Key](https://github.com/user-attachments/assets/e2b8ceb1-20b7-4e2c-815b-a6d32005d975)






### Step-by-Step Implementation
1. Create User Group(reference: 1-Create User Group.png)
   - Attach <b>KMS_Policy</b> permissions.
2. Create two Users(reference: 2-Create two Users.png)  
   - One for Encryption and the second for Decryption 
   - Add Users to group.
   - Get Access key and Secret Access key.
3. Create a KMS key.(reference: 3-Create a KMS key.png)
   - Define a key administrative permissions(The first user)
   - Define a key usage permissions(The second user)
   - Key Policy(JSON policy)
4. Launch an EC2 Instance.(reference: 4-Launch an EC2 Instance.png)
5. SSH into the EC2 Instance via SSH client.(reference: 5-SSH client.png)
6. Perform KMS Encryption and Decryption
   - Create a file with the name note.txt(reference: 6-Create file note.txt.png)
   - Execute AWS configuration.(reference: 7-AWS configuration.png)
   - Encrypt the text file.(reference: 8-Encryption.png)
   - View the statement.(reference: 9-Ecryption view.png)
   - Decrypt the Encrypted file.(reference: 10-Decryption.png)
   - View the statement(Clear text).(reference: 11-Clear Text.png)
   - Re-Encrypt the text file.(reference: 12-Re-Encryption.png)
   - View the statement(after Re-Encryption)(reference: 13-Re-Encryption view.png)
  

 
    

> *Lab originally from: [Whizlabs - Encryption and Decryption Using KMS](https://www.whizlabs.com/labs/encryption-and-decryption-using-kms/))*



