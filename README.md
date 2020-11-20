# easyrefresh

EasyRefresh:
I created a rough version of this application when I wanted to create a site but was fed up with the constant need to refresh the page.
This is what this application does:
  -Creates a local http server at the specified file's directory
  -Opens a window of your prefered browser with the specified file open
  -Everytime you modify any HTML,Javascript,CSS file in the specified file's directory the browser page refershes.
 This was so helpful to me and I believe it will to many HTML beginers as it allows 'real-time' modification. (Real-time because you can make very small changes and immediatelly watch the page update)

Requirements:
Windows 8 or 10
Any of the following browsers and the corresponding driver (links to the drivers are provided at the end of the file):
-Microsoft Edge
-Chrome
-Firefox

Parametres:
'-fp' : the exact path to the html file
'-f'  : the path to the directory where the html file is
'-n'  : the name of the html file (default:index.html)
'-p'  : the port number you want the localhost to be hosted at (default:8080)
'-d'  : the coresponding numer to your prefered browser ( 1 - Microsoft Edge  (default:2)
                                                          2 - Chrome
                                                          3 - Firefox )
'-fd' : the exact path to the directory where the driver .exe is (default: C:\bin) 

How to use:
Run the easyrefresh.exe from cmd and specify the parametres (parametre order does not matter)
A window will the open and your html file will be there.
All you need to do now is to modify any file in the same directory on your editor and save. The browser will then instantly refresh.
The app will crash if you move,create,delete any files in the file's directory.

i.e.:
  The simplest one:
  <path>\easyrefresh\easyrefresh.exe -fp C:\Users\User1\Desktop\demo\demo.html --- The demo.html file is opened in localhost:8080 using Chrome
  
  <path>\easyrefresh\easyrefresh.exe -f C:\Users\User1\Desktop\demo -n demo.html --- This will also work the same way as the previous one
  if the file's name is index.html the following can also be done:
  <path>\easyrefresh\easyrefresh.exe -f C:\Users\User1\Desktop\demo             --- This will also work like the two previous examples
  
  <path>\easyrefresh\easyrefresh.exe -fp C:\Users\User1\Desktop\demo\demo.html -p 10 -d 1 -fd C:\bin\msedgedriver --- The demo file is opened in localhost:80 using Microsoft Edge
