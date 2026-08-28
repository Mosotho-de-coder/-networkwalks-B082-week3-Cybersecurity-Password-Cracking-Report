**PASSWORD CRACKING REPORT**

Ethical Hacking & Cybersecurity | Batch B082

| **Password cracker Name <br>(Cybersecurity Professional)** | Mosotho Thatho                                                              |
| ---------------------------------------------------------- | --------------------------------------------------------------------------- |
| **Program/Batch**                                          | B082-Networkwalks                                                           |
| **Date**                                                   | 28 August 2026                                                              |
| **Modules completed**                                      | Password Cracking with JTR<br><br>Password Cracking with Networkwalks Tools |
| **Clients/Target**                                         | 3 PDF locked files                                                          |

# **Introduction**

The practical of this week focused on password recovery from three password protected PDF files. I worked with two different approaches: John the Ripper through its Johnny graphical interface, and the Networkwalks Hash Calculator and Password Cracker.

The exercise gave me an opportunity to work with hashes, wordlists and password recovery tools in a controlled training environment. I also learned that different tools and wordlists can produce different results, so being able to troubleshoot and try an appropriate alternative is an important part of the process.

# **Objectives**

- Install and configure John the Ripper and Johnny on a Windows PC.
- Extract the hash values from the three locked PDF files.
- Use Johnny to load the saved hashes and perform the assigned password-recovery attacks.
- Use the Networkwalks Hash Calculator to generate hash values for the PDF files.
- Use the Networkwalks Password Cracker with its built-in wordlist.
- Use a custom wordlist when the built-in wordlist did not produce a match.
- Verify each recovered password by opening the corresponding PDF file.
- Document the process and results with screenshots.

# **Tools used**

| **Tools/Resources**           | **purpose**                                                                    |
| ----------------------------- | ------------------------------------------------------------------------------ |
| Windows PC                    | Computer used to perform the practical.                                        |
| John The Ripper (JTR)         | Password-recovery tool used with the extracted PDF hashes.                     |
| Johny The Ripper              | Graphical interface used to run John the Ripper.                               |
| Networkwalks Hash Calculator  | Generated hash values from the PDF files.                                      |
| Networkwalks Password Cracker | Attempted password recovery using available wordlists.                         |
| Online Hash Crack             | Used during the first method to obtain the PDF hash values.                    |
| Locked PDF files              | Training files used for the password-recovery exercise.                        |
| Custom Wordlist               | Used when the built-in Networkwalks wordlist did not find a matching password. |

# **Method 1: Password Cracking with John & Johnny the Ripper**

## **Installation and Configuration**

I first downloaded John the Ripper and Johnny and installed the required software on my Windows PC. After installing Johnny, I configured its execution path to point to the John executable inside the John the Ripper installation. This allowed Johnny to use John as the password-recovery engine.

The screenshot below shows the execution-path configuration used during the setup.


## **Extracting the PDF Hashes**

After setting up Johnny, I used the online PDF hash extraction tool to process each of the three locked PDF files. The purpose of this step was to obtain the hash value needed by John the Ripper.

I saved each extracted hash in a separate text file so that it could be loaded into Johnny for the next stage.

Finding hash of the document I uploaded the files in the online hash crack website. The following screenshot shows the hash value of the first pdf file:


## **Running the Password-Recovery Attack**

I then opened each of the saved hash files in Johnny and started the assigned attack. Once a password was recovered, I recorded the result and used it to test whether the corresponding PDF could be opened.

PDF File 1 – Recovered Password: For PDF file 1:


PDF File 2 – Recovered Password: For PDF file 2:


PDF File 3 – Recovered Password: For PDF file 3:


# **Method 2: Password Cracking with Networkwalks Tools**

For the second method, I used the Networkwalks Hash Calculator at and Password Cracker. The process was different from the first method because the hash was generated directly through the Networkwalks tool and then tested against the available wordlists.

## **Generating the Hash with the Networkwalks Hash Calculator**

I uploaded each locked PDF to the Networkwalks Hash Calculator. The tool generated a hash value for each file, which I then copied and pasted that hash number in the Networkwalks Password Cracker.

The screenshot below shows the networkwalks hash calculator tool and I uploaded one of the pdf files to find pdf hash:


## **Testing the Built-in Wordlist**

I first tried the built-in wordlist provided by the Networkwalks Password Cracker. For the first PDF, the built-in list did not contain a matching password. This was a useful result because it showed that a password-recovery attempt can fail simply because the required password is not present in the wordlist being tested.

Networkwalks password cracker could not find a matching password on its build-in wordlist, this is shown in the screenshot below:


## **Using a Custom Wordlist**

The Networkwalks Password Cracker also provides an option to upload a user's own wordlist. I used this option for the first PDF after the built-in list failed to find a match.

The custom wordlist produced a matching password for the first PDF. For the second and third PDF files, the built-in wordlist was sufficient to find matching passwords.

PDF File 1 – Custom Wordlist Result: First pdf file:


PDF File 2 – Built-in Wordlist Result: The second pdf file:


PDF File 3 – Built-in Wordlist Result: Third pdf file


# **Results and Verification**

Both methods were successful. I was able to recover passwords for all three training PDF files. I did not consider a password recovered until I had used it to open the corresponding PDF successfully.

PDF File 1 – Opened Successfully: For PDF file 1:


PDF File 2 – Opened Successfully: For PDF file 2:


PDF File 3 – Opened Successfully: For PDF file 3:


# **Challenges Encountered and How I Solved Them**

The main challenge I encountered was with the Networkwalks Password Cracker. When I first used its built-in wordlist for the first PDF, the tool could not find a matching password.

Instead of stopping there, I checked the available options and found that the tool allowed me to upload my own wordlist. I supplied a custom wordlist and ran the password-recovery attempt again. This time a matching password was found, which I then verified by opening the PDF.

This was a useful part of the exercise because it showed me that the success of a wordlist-based password recovery attempt depends heavily on the contents of the wordlist.

# **What I Learned**

- I learned how password-protected PDF files can be represented by hash values for password recovery testing.
- I learned how Johnny can provide a graphical way of working with John the Ripper.
- I learned how to extract a PDF hash and prepare it as input for a password recovery tool.
- I learned that a built-in wordlist may not always contain the password being tested.
- I learned how to use a custom wordlist when the first approach did not produce a match.
- I learned the importance of verifying a recovered password by actually opening the protected file.
- I also gained more confidence in troubleshooting when the expected result was not obtained on the first attempt.

# **Ethical and Responsible Use**

This practical was completed as part of the Networkwalks Ethical Hacking & Cybersecurity training program using the three locked PDF files provided for the exercise. The password-recovery techniques described in this report were used for authorized educational purposes only. These techniques should only be applied to files or systems where the user has permission to perform the testing.

# **Conclusion**

This week's practical gave me hands-on experience with PDF password recovery using two different approaches. I successfully worked with John the Ripper and Johnny, as well as the Networkwalks Hash Calculator and Password Cracker.

The most valuable part for me was troubleshooting the first Networkwalks Password Cracker attempt. When the built-in wordlist did not contain the required password, I used a custom wordlist and was able to obtain a match.

In the end, all three PDF passwords were recovered using the assigned methods and each password was verified by successfully opening its corresponding PDF. Overall, the exercise improved my understanding of hashes, wordlists, password-recovery tools and practical cybersecurity troubleshooting.
