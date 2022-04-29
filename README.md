# burpsuite
##################################** Prequisites **#############################################

	**Download .jar file for Burp Suite Pro from**
		--> https://portswigger.net/burp/releases/
	**Download Burp Loader files. Then Follow Below Steps for Activation**
		--> https://github.com/indiansharma/burpsuite
	**If using in Windows 10, Download and Install Java and JDK**
		**For Java** --> https://javadl.oracle.com/webapps/download/AutoDL?BundleId=244068_89d678f2be164786b292527658ca1605
		**For JDK**  --> https://www.oracle.com/in/java/technologies/javase-jdk15-downloads.html

################################** Execution and Activation **################################
	
	**1. Place all files in 1 folder**
		For Example lets take as --> C:\Users\IndianSharma\Desktop\burp\
	----------------------------------------------
	**2.1 Run This Command for Windows in CMD Prompt.**
		java --illegal-access=permit -Dfile.encoding=utf-8 -javaagent:"C:\Users\IndianSharma\Desktop\burp\loader.jar" -noverify -jar "C:\Users\IndianSharma\Desktop\burp\burpsuite_pro_v2022.1.jar"
	**2.2 Run this command for Linux in Terminal. Suppose Your files are in /home/kali/Desktop/burp/**
		java --illegal-access=permit -Dfile.encoding=utf-8 -javaagent:/home/IndianSharma/Desktop/burp/loader.jar -noverify -jar /home/IndianSharma/Desktop/burp/burpsuite_pro_v2022.3.5.jar &
	----------------------------------------------
	**3. Use keygen.jar to generate the License key**
		java -jar keygen.jar
	----------------------------------------------
	**4. Activate Burp Suite Pro**
		1. Modify License String like "license to IndianSharma"
		2. Copy License key from keygen.jar and paste in Burp Suite Pro and click Next.
		3. Select Manual Activation Option on your bottom Right in Burp Suite Pro.
		4. Copy License Request from BurpSuite_Pro and paste in keygen.jar
		5. Copy license response from keygen.jar and paste in BurpSuite_Pro, and next and Done
	----------------------------------------------
	**5.1 For Windows Follow These Steps**
		1. Open Notepad and Paste command at 2.1 and save the file with name burp.bat in C:\Users\IndianSharma\Desktop\burp\   Folder.
		2. Open another Notepad and Paste below command and save it with burp.VBS extension in Desktop.
			Set WshShell = CreateObject("WScript.Shell")
			WshShell.Run chr(34) & "C:\Users\IndianSharma/Desktop\burp\burp.bat" & Chr(34), 0
			Set WshShell = Nothing
	**5.2 For Linux Follow these Steps**
		1. With Sudo Permissions, Create a file with command "gedit /bin/burp"
		2. Open the folder where your Burpsuite is located or you downloaded using github
    3. Now open terminal from same window, by right click and open terminal in window
    4. Now run the command "chmod +x /home/kali/Desktop/burp/start.sh"
    5. Right click and then left click on Create Launcher
        a) Select below options in window:
        b) Type: Application in Terminal
        c) Name: Start Burpsuite
        d) Command: /home/nikhil/Desktop/burp/start.sh (Path to start.sh - Bash File)
        e) Comment: Start Burp or Start Burpsuite
    6. Now goto the folder of BurpSuite and double click the launcher, easily this will launch Burpsuite without doing copy-paste license or activation or        running command in terminal.
	----------------------------------------------
	**6.1 For Executing Burp in Windows, Double Click on burp.VBS file.**
	**6.2 For Executing Burp in Linux, Write burp in Terminal and press Enter.**
