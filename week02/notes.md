/Users/kanishka
The command ls -a prints hidden files and directories along with three dots .  .. which ls doesn't show.
drwx------@   4 kanishka  staff   128 12 Jul 21:47 Applications. the first column represents the file type and access permissions.
It works because the path starts from my current directory, so I don't need to use cd first. coding-cafe/week02 is a relative path because it is based on my current location.
mv was used to move the file from one folder to another and then to rename the file.
There are 12 folders in my PATH. They are separated by :
My python3 is located at /Library/Frameworks/Python.framework/Versions/3.14/bin/python3.
No, our paths are different because Python is installed in different locations on our computers.
The shell said zsh: command not found: pyton3. This means the shell could not find pyton3 in the folders listed in my PATH because the command was typed incorrectly.
.venv did not show up with ls because it is a hidden folder. Files and folders starting with . are hidden, but ls -a shows them.
(.venv) appeared at the beginning of my prompt. This shows that the virtual environment is activated.
No, the paths are different. Activating .venv changed my PATH to use the Python inside the virtual environment.
The second list has requests and some other packages that were not in the first list. They were added when I installed requests.
python3 points back to /Library/Frameworks/Python.framework/Versions/3.14/bin/python3.
ls -h shows file sizes in a human-readable format, making them easier to understand.
Ctrl + C stopped the current process, Ctrl + D tells the terminal that there is no more input and exits the Python prompt.
