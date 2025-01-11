# Decrypting
<h2>Activity overview</h2>

Previously, you learned about cryptography and how encryption and decryption can be used to secure information online. You were also introduced to the Caesar cipher, one of the earliest cryptographic algorithms used to protect people’s privacy.

As a security analyst, it’s important that you understand the role of encryption to secure data online and that you’re familiar with the right security controls to do so.

In this lab activity, you’ll be guided through some basic cryptographic activities using Linux commands to decrypt files and reveal hidden messages.
<h2>Scenario</h2>

In this scenario, all of the files in your home directory have been encrypted. You’ll need to use Linux commands to break the Caesar cipher and decrypt the files so that you can read the hidden messages they contain.

Here’s how you’ll do this task: First, you’ll explore the contents of the home directory and read the contents of a file. Next, you’ll find a hidden file and decrypt the Caesar cipher it contains. Finally, you’ll decrypt the encrypted data file to recover your data and reveal the hidden message.

<h2>Task 1. Read the contents of a file</h2>
The lab starts in your home directory, /home/analyst, as the current working directory.

In this task, you need to explore the contents of your home directory and read the contents of a file to get further instructions.

1.Use the ls command to list the files in the current working directory.

![image](https://github.com/user-attachments/assets/d1824871-26b5-4b9b-b7a6-bf061e8d539d)

Two files, Q1.encrypted and README.txt, and a subdirectory, caesar, are listed:
The README.txt file contains an important message with instructions you need to follow.

2.Use the cat command to list the contents of the README.txt file.

![image](https://github.com/user-attachments/assets/cd8d98af-7d7a-46ae-a6f4-83d29b8cbb7b)

The message in the README.txt file advises that the caesar subdirectory contains a hidden file.

In the next task, you’ll need to find the hidden file and solve the Caesar cipher that protects it. The file contains instructions on how to recover your data.

<h2>Task 2. Find a hidden file</h2>
In this task, you need to find a hidden file in your home directory and decrypt the Caesar cipher it contains. This task will enable you to complete the next task.

1.First, use the cd command to change to the caesar subdirectory of your home directory:

![image](https://github.com/user-attachments/assets/c55daff4-cf19-404f-8efc-67a3e7752782)

2.Use the ls -a command to list all files, including hidden files, in your home directory.

![image](https://github.com/user-attachments/assets/946a0d38-de46-4f11-b090-a70cc8756cb2)

Hidden files in Linux can be identified by their name starting with a period (.).

3.Use the cat command to list the contents of the .leftShift3 file.

![image](https://github.com/user-attachments/assets/24d7d5cb-557f-4179-a04f-db099b50c2af)

The message in the .leftShift3 file appears to be scrambled. This is because the data has been encrypted using a Caesar cipher. This cipher can be solved by shifting each alphabet character to the left or right by a fixed number of spaces. In this example, the shift is three letters to the left. Thus "d" stands for "a", and "e" stands for "b".

4.You can decrypt the Caesar cipher in the .leftshift3 file by using the following command:

![image](https://github.com/user-attachments/assets/48a48d1a-3dc3-4bd4-857f-3f71376e5268)

5.Now, return to your home directory before completing the next task:

![image](https://github.com/user-attachments/assets/429b1baa-f25a-4ac8-a61a-ed3406fad98e)

<h2>Task 3. Decrypt a file</h2>

Now that you have solved the Caesar cipher, in this task you need to use the command revealed in .leftshift3 to decrypt a file and recover your data so you can read the message it contains.

1.Use the exact command revealed in the previous task to decrypt the encrypted file:

![image](https://github.com/user-attachments/assets/da88c936-226c-42e1-a7ff-b1cd1fc37151)

2.Use the ls command to list the contents of your current working directory again.

![image](https://github.com/user-attachments/assets/2af474a1-32e5-42c2-9f4f-bdc9c822714e)

The new file Q1.recovered in the directory listing is the decrypted file and contains a message.

3.Use the cat command to list the contents of the Q1.recovered file.

![image](https://github.com/user-attachments/assets/539052e0-6b64-40b7-9947-8fecba14fcdd)
