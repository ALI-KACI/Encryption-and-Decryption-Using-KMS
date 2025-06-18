Perform KMS Encryption and Decryption
   - Create a file with the name note.txt(reference: 6-Create file note.txt.png)

`echo “Welcome to our lab are you ready??” > note.txt`
`
   - Execute AWS configuration.(reference: 7-AWS configuration.png)
`aws configure`
   - Encrypt the text file.(reference: 8-Encryption.png)
`aws kms encrypt --key-id <replace-key-id> --plaintext fileb://note.txt --output text --query CiphertextBlob | base64 --decode > encryptednote.txt`

   - View the statement.(reference: 9-Ecryption view.png)
`cat encryptednote.txt`
   - Decrypt the Encrypted file.(reference: 10-Decryption.png)
`aws kms decrypt --ciphertext-blob fileb://encryptednote.txt --output text --query Plaintext | base64 --decode > decryptednote.txt`
   - View the statement(Clear text).(reference: 11-Clear Text.png)
`cat decryptedsecret.txt`
   - Re-Encrypt the text file.(reference: 12-Re-Encryption.png)
`aws kms encrypt --key-id <replace-key-id> --plaintext fileb://decryptedsecret.txt --output text --query CiphertextBlob > newencryptedsecret.txt`
   - View the statement(after Re-Encryption)(reference: 13-Re-Encryption view.png)
`cat newencryptedsecret.txt`

  
