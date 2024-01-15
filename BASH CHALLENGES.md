
`					`**BASH CHALLENGES**

1\.       a.) Display the path of your current directory

pwd

` 		`command is used to display the path of current directory

( b.) List out the contents of your current directory

` `ls

command is used to list out contents of current directory

`	`( c.) List out the contents of your current directory including hidden files

` `ls –a

` 		`command is used to list out contents of current directory including hidden files


2\.

( a.) Create a new directory named a

`	`mkdir a

(make directory) command is used to make  create a new directory .mkdir a creates new directory with name a

( b.) Move to the newly created directory a

`	`cd a

(change directory) command is  used to change the current working directory . cd a traverses to directory a.

( c.) Create a blank file named “file1”

` 	 `touch file1

touch command is used to create a file without any content .



`	`( d.) Display the file type of “file1”

`	`file file1

file command is used to determine the type of a file and its data

( e.) Add the line “Hello World” to “file1” using the command echo

`	`echo “Hello World” >>file1

echo command can be used to add new text file to a file or overwrite the previous texts in a file.

( f.) Display the contents of “file1”

`	`cat file1

cat command is used to display the content of a file. It can also be used to add content to an existing file.

`	`( g.) Display the file type of “file1” again

` 	`file file1


3\.   ( a.) Stay in directory a. Create a file “file2” and add the contents below using the  command cat

`	`touch file2

cat  <<EOF > file2

First Line Second Line Third Line

EOF

` `Touch command is used to create file 2 and cat command was used to add content to file 2.EOF stands for End Of a File. Contents can be added in the space between <<EOF and EOF.

` 	`( b.) Display the contents of “file2”

`	`cat file2

`	`( c.) Display the contents of “file2” with the lines reversed

`	`tac file 2

can be used to reverse the lines

**rev file 2**

can be used to reverse the characteristics within a single line.



4\.

`	`a.) Stay in directory a. Concatenate the contents of “file1” and “file2” and save them into a new file “file3”

` `cat file1 file 2 > file3

contents of two files can be concatenate the contents into file3.if file 3 doesn’t exist it will be created or if already contents are there, it will be overwritten.



`	`( b.) Display the contents of “file3”

`	`file file3



b. 	cat file3




**5.**( a.) Stay in directory a. Create 2 directories b/c with a single command

**( b.) Create a new directory d**

**( c.) Copy the directory d to directory c using a single command**

**( d.) Delete the directory d in the current directory a**

**( e.) Copy “file3” to the directory d with a single command**









**6.**

**a.) Go to directory d and rename “file3” to “file0”**

**( b.) Stay in the same directory and move “file0” to directory a**






**7.**

**a.) Go to your home directory**

**b.) Create a file named “test” in the directory a/b/c/d**

**c.) Stay in the home directory. Find and display the path of “test”**







**8.)**( a.) Go to directory a. Get the man page of grep and save its contents to a file named “grepman.txt”

**( b.) Print the lines containing the word “FILE” (Case sensitive) in the file “grepman.txt”**










**9.( a.)** Go to directory a and remove the directory b with a single command

**( b.)** R**emove the files starting with the word “file” with a single command.**








**10.)**

a.) Go to <https://blog.bi0s.in/>  and download the logo.png image using wget

**b.) Do the same with python script (Hint : request library)**

**(c.) Also, display the metadata of the png.**






import requests

from PIL import Image

url = 'https://blog.bi0s.in/assets/logo.png'


response = requests.get(url)

if response.status\_code == 200:



`    `with open('img.png', 'wb') as file:

`        `file.write(response.content)





`    `img = Image.open('img.png')

`    `img.show()

`    `print("Image downloaded and displayed successfully.")

else:

`    `**print(f"Failed to download image. Status code: {response.status\_code}")**






**11. a.)** Use **traceroute** on google.com and find list of the IP addresses and hostnames between you and  google.com

`     `**( b.)** Find  Subdomains,ip addresses of google.com using nslookup command

**12.**

**Start a web server on port 8080 with python command**

**(In any directory and access the files in web browser )**






**13.**

**( a.) Learn about nmap and use that scanner to scan your own machine**


**(b.)**

**Go to <https://tryhackme.com/room/furthernmap> and get ip address and** Scan the ip address with (-sS,-sV,-A) in your terminal include all ports






**14.**

**( a.) Create a chat application using nc on your local machine with one terminal as server and other as the client**


**															

**( b.) Transfer a file from server to client (save that file with another name) and display the file.**
