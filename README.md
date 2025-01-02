# Ransomware Attack

![Screenshot 2023-12-24 at 5 46 59 PM](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/e22ff71d-fc02-4128-bb18-857c302d138c)

## Summary

In this project I built a fake environment for a student, using Oracle VirtualBox and then attacking the system using a ransomware attack, utilizing visual studio for the creation of the virus code.  

I learned how ransomware works on the coding side of things, as well as how quick a system can get encrypted if you do get hacked.


## Technologies & Components Used

- Windows Server 2019
- Oracle VirtualBox
- Visual Studio Community 2019 
	-.NET desktop Development
- File and Storage Services
- VirusTotal
- C#
- Windows Security
- Firewall


<details> 
  <summary><h2>Set-Up</h2></summary>
	
I worked with virtualBox to create the fake student environment, (making sure to not use my personal pc/mac since we are dealing with viruses) using a windows 2019 ISO.

![1 student account](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/5cd5ad1b-7970-43aa-b241-834098a8b755)

From here, I downloaded Visual Studio Community 2019 for our coding part, as well as being sure to download the ‘.NET desktop development’ workload as well before completion.

![2 download](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/5a8587a4-5a23-4d15-97f3-7657e2e6776f)

![3 visual 2019](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/c716c6ac-18fc-47d7-bb9d-add03f6f0bff)

After getting this, the last set-up step was getting the ransomware project files from online. From there, I created a folder named “Safe_Folder” and placed it in our C: Drive so that it wouldn’t be affected by our ransomware attack (that will attack other on the machine as well as being able to be manipulated/decrypted later without any issue.

![4 folder 1](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/4609427e-30f2-40a8-956c-5ed4343a7caf)

![4 folder 2](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/726e3bcd-1565-4d1e-a6d2-bf6bf980d009)

</details>



<details> 
  <summary><h2>Creating Fake Desktop Environment</h2></summary>


Now to the fun stuff! To make the environment feel more authentic I created fake files, created folders and saved images throughout the machine which covered Desktop, Documents and Picture directories.

![5 before pic](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/a6a79981-de1f-49f5-82bf-c79f9d533d25)

</details>

<details> 
  <summary><h2>Encryption</h2></summary>

After disabling our Windows Security (to protect our virus from possibly getting detected) in the VM, I then opened up our ransomware project that I downloaded and placed in our “Safe_Folder” previously through VisualStudio to see the current code, it’s GUI and make any customizations that I see fit.

![6 gui 1](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/bfbf236e-0705-47bd-8919-6518ff654255)

![7 code](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/9ab39285-a7b9-4c20-ae7c-1e6a70357a75)

Afterwards, I ran the ransomware .exe file and watched live as the files across the 3 directories became infected. You can recognize the infected files by the image becoming blank beside the file name as well as “.jcrypt” being added to the end of each file.

![8 being encrypted](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/af747943-aa3a-4298-bca9-0027b61e35eb)

![9 finished files 2](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/bc4d435b-fc59-412e-b328-58d1349734d0)

After all of the files were finished being encrypted, our pop-up showed up on the screen, notifying the “victim” that their files have been encrypted, and to send us 5 bitcoins to an address and email for transaction confirmation.

![10 encrypted](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/a337ba16-aa5c-48d1-8c62-456f21675ad1)

In addition to this, a new file is created on the desktop notifying the user that the files are encrypted with the log of each of the file and what directories they were in, with the previous info from the GUI present as well.

![11 recovery file left for victimes](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/50e38dd5-39d1-4a09-b317-d942f51e739c)

</details>


<details> 
  <summary><h2>Analysis Of Ransomware</h2></summary>

Lastly, I used VirustTotal to analyze our ransomware that we just used.

![12 VIRUST TOTAL Home](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/697f177d-ad82-4a6b-be16-0cdaf2520331)

From here, we’re able to see that our malware was detected by 46 out of 72 machines.

![13 virus being flagged](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/291fae8b-cc2a-446d-a452-283637e057aa)

In the details section, we can also find more info regarding the malware including the MD5 & Sha256 hashing.

![14 details virus](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/d5b722a3-dd3a-4470-8a67-e1d26c4db1c3)

The ones that weren’t able to detect our malware were probably because their anti-virus engine used signature-based detection whereas are code was customized.


![15 DIDN'T CATCH IT! (WRITE NOTES ON WHY FROM VIDEO)](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/931d2491-751c-4df2-bdf0-57abc29c20d6)

</details>

<details> 
  <summary><h2>Conclusion</h2></summary>


In closing, this project gave me the ability to learn more about malware from an attackers prospective as well as a user. In addition to using new services like visual studio, and manipulating C# code I was to get more hands-on experience as an attacker and how to find and use malware to put myself in the shoes of a Red Teamer.

</details>

<details> 
  <summary><h2>P.S Decrypting The Attacked Computer</h2></summary>

I was also able to get the decryption files for this malware as well, so if you were following along you can gift yourself 5 bitcoins lol and then send yourself the decryption .exe and run that to decrypt your environment to get that perspective as well.


![16 decryp](https://github.com/EricMcclellan1/ransomware-attack/assets/147299619/e7c69d27-24a4-4b2c-893a-182d264e3c37)

</details>








