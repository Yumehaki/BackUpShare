BUS (BackUpShare) is a system that can perform backup in a safe state where P2P, encryption and high compression protect the privacy of people and people all over the world.
~Advantages and disadvantages~
+1: If the user loses the data on the PC, he / she can search for backup files on the PC from all over the world.
+2: BUS considers privacy. It uses a variety of encryption and is stored robustly.
+3: Even if you use BUS, big companies never see your data in peep. Unless you reveal your password, you are the only one to see the data.
+4: Data is compressed. So, the data of other people who do not use it anyway will not get in the way much.
+5: With BUS you can also store it on your own disc. However, it is not always an effective means when a disaster occurs.

-1: Not all data will be returned even if data is lost. This is because updating data is not always possible.
-2: Your disk will be compressed to some extent by the data of others.
-3: If the password is leaked, users and non-users all over the world can access your data.
-4: If you lose the path file (described below), your data will not be returned. We will deal with this later.

 0: This software has no warranty.

~ Technical structure of BUS ~
First you specify the files to back up.
The specified file is first wrapped in a number of ZIP files.
Encrypt this ZIP file. RSA → AES → (ZIP) → AES → RSA. The password in this case is defined by the path file.
In addition, it will multiply ZIP the encrypted files.
Finally, use "7z", which has a high compression rate. The file is now sent to n people.

In addition, the path file has a '2nd password' applied and is lightweight. For this reason, it can be operated without problems even on cloud servers of large companies.
It is recommended to use non-ASCII characters of 16bit or more for the 2nd password. It is also 2FACTA certified (mandatory).
However, when files are sent, you are obliged to receive backups of the same capacity for n people. If you do so, your backup will also be deleted.
The value of n can be changed freely with 2 or more. However, the change is applied only to the backup file created after the change.

~ Various Buses ~
First of all, it's a mistake to share top-secret files on BUS. If the password is leaked, it will be the second disaster. let's stop.
It is also effective for users who are not interested in privacy issues. Because large enterprise servers are usually located in one or several locations. Let's assume that one or more of these servers were destroyed in a disaster or conflict. Your data will not come back anymore. Even important memory data. That's why it's BUS. Also, if you put the path file introduced earlier on the server of a large company, it is better to divide it into multiple data servers. People who don't care about privacy will back up the path file on BUS. But it's pointless and dangerous. Because you need it when you retrieve the backup.
Uploading the pass file to SNS is one way. But it's a good idea to put some kind of sturdy code on your own.

BUS is open source. The usage fee is a small amount of your disc.
(Translate by Google Translation)
