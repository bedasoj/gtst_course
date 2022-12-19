# *Linux For User*
## *Overview of kali linux*
>**Kali Linux** is an open-source, Debian-based Linux distribution geared towards various information security tasks, such as Penetration Testing, Security Research, Computer Forensics and Reverse Engineering.
### *Linux Menu Tools*
>**1. Information Gathering**
Tools for gathering,in system, network, host.

>**2. Vulnerability Analysis**
Tools for finding vurnerbilities.

>**3. web Application Analysis**
Tools for finding Vulnerabilities and exploits on websites.

>**4.Database Assessment**
Tools for finding Vulnerabilities and exploits on Databases.

>**5. Password Attacks**
Tools for exploiting passwords for login, websites, application, windows.

>**6. Wireless Attacks**
Tools for exploiting Wireless Systems like WiFi, Bluetooth.

>**7. Reverse Engineering**
Tools for exploiting Sofwares, Mobile applicationns and any binary files.

>**8. Exploitation Tools**
Tools for exploiting Softwares, Mobile, Computers, Websites and Any thhings.

>**9. Sniffing & Spoofing**
Tools for Listeninig or hijacking networks.

>**10. POST Exploitation**
Tools for Maintaining our access. Used after exploiting a system.

>**1. Forensics**
Tools for  doing researches and innvestigate a Cyber Attacks.

>**12. Reporting Tools**
Tools for Report preparation. After some forensic you will get dataa and you will write report and these tools will help you.

>**13. Social Engineering tools**
Tools used for social engineering attacks.

>**14. System Services**
Buttons used to start some services.

>**15. Usually used applications**
Softwares for some basic purposes.

### Folder Manager


### Linux Commands
**What Is a Linux Command?**
>A  ***Linux command*** is a program or utility that runs on the CLI – a console that interacts with the system via texts and processes. It’s similar to the Command Prompt application in Windows.

>**Linux commands** are executed on Terminal by pressing Enter at the end of the line. You can run commands to perform various tasks, from package installation to user management and file manipulation.

Here is the list of basic Linux commands👍:

**1️⃣sudo command**
>Short for superuser do, sudo is one of the most popular basic Linux commands that lets you perform tasks that require administrative or root permissions.

>When using sudo, the system will prompt users to authenticate themselves with a password. Then, the Linux system will log a timestamp as a tracker. By default, every root user can run sudo commands for 15 minutes/session.

If you try to run **sudo** in the **command line** without authenticating yourself, the system will log the activity as a **security event.**

Here’s the general syntax:
*sudo (command)*
You can also add an option, such as:

**-k** or **–reset-timestamp** invalidates the timestamp file.
**-g** or **–group=group** runs commands as a specified group name or ID.
**-h** or **–host=host** runs commands on the host


**:two: pwd command**
Use the **pwd command** to find the path of your current working directory. Simply entering pwd will return the full current path – a path of all the directories that starts with a forward slash (/). For example, /home/username.

The **pwd command** uses the following syntax:
**pwd [option]**
>It has two acceptable options:
**-L or –logical** prints environment variable content, including symbolic links.
**-P or –physical** prints the actual path of the current directory.

**:three:cd command**
To navigate through the Linux files and directories, use the cd command. Depending on your current working directory, it requires either the full path or the directory name.

Running this command without an option will take you to the home folder. Keep in mind that only users with **sudo** privileges can execute it.

Let’s say you’re in **/home/username/Documents** and want to go to **Photos**, a subdirectory of **Documents**. To do so, enter the following command:
**cd Photos**

If you want to switch to a completely new directory, for example, **/home/username/Movies**, you have to enter cd followed by the directory’s absolute path:

**cd /home/username/Movies**

>Here are some shortcuts to help you navigate:
    **cd ~[username]** goes to another user’s home directory.
    **cd ..** moves one directory up.
    **cd-** moves to your previous directory.

**:four:ls command** ⏬
>The **ls** command lists files and directories within a system. Running it without a flag or parameter will show the current working directory’s content.

To see other directories’ content, type **ls** followed by the desired path. For example, to view files in the Documents folder, enter:
**ls /home/username/Documents**
>Here are some options you can use with the ls command:
**ls -R** lists all the files in the subdirectories.
**ls -a** shows hidden files in addition to the visible ones.
**ls -lh** shows the file sizes in easily readable formats, such as MB, GB, and TB.

**:five: cat command**
**Concatenate, or cat**, lists, combines, and writes file content to the standard output. To run the cat command, type cat followed by the file name and its extension. For instance:
**cat filename.txt.**
>Here are other ways to use the cat command:
**cat > filename.txt** creates a new file.
**cat filename1.txt filename2.txt > filename3.txt** merges **filename1.txt and filename2.txt** and stores the output in **filename3.txt.**
tac filename.txt displays content in reverse order.

**:six:cp command** 
Use the**cp command** to **copy** files or directories and their content. Take a look at the following use cases.

To copy one file from the current directory to another, enter **cp** followed by the file name and the destination directory. For example:

**cp filename.txt /home/username/Documents**

To copy files to a directory, enter the file names followed by the destination directory:

**cp filename1.txt filename2.txt filename3.txt /home/username/Documents**

To copy the content of a file to a new file in the same directory, enter **cp** followed by the source file and the destination file:

**cp filename1.txt filename2.txt**

To copy an entire directory, pass the **-R** flag before typing the source directory, followed by the destination directory:

**cp -R /home/username/Documents /home/username/Documents_backup**


**:seven: mv command** ✂️
The primary use of the** mv command** is to move and rename files and directories. Additionally, it doesn’t produce an output upon execution.

Simply type** mv** followed by the filename and the destination directory. For example, you want to move **filename.txt** to the **/home/username/Documents **directory:

**mv filename.txt /home/username/Documents.**

You can also use the mv command to rename a file:

**mv old_filename.txt new_filename.txt**


**:eight:mkdir command**
Use the **mkdir command** to create one or multiple directories at once and set permissions for each of them. The user executing this command must have the privilege to make a new folder in the parent directory, or they may receive a permission denied error.

Here’s the basic syntax:

🌟**mkdir [option] directory_name**

For example, you want to create a directory called Music:

🌟**mkdir Music**

To make a new directory called Songs inside Music, use this command:

🌟**mkdir Music/Songs**

>:star: The mkdir command accepts many options, such as:
    **-p or –parents** create a directory between two existing folders. For example, mkdir -p Music/2020/Songs will make the new “2020” directory.
    **-m** sets the file permissions. For instance, to create a directory with full read, write, and execute permissions for all users, enter mkdir -m777 directory_name.
    **-v** prints a message for each created directory.
