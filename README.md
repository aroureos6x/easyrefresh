# easyrefresh

EasyRefresh:<br>
I created a rough version of this application when I wanted to create a site but was fed up with the constant need to refresh the page.<br>
This is what this application does:<br>
  -Creates a local http server at the specified file's directory<br>
  -Opens a window of your prefered browser with the specified file open<br>
  -Everytime you modify any HTML,Javascript,CSS file in the specified file's directory the browser page refershes.<br>
 This was so helpful to me and I believe it will to many HTML beginers as it allows 'real-time' modification. (Real-time because you can make very small<br> changes and immediatelly watch the page update)<br>
<br>
Requirements:<br>
Windows 8 or 10<br>
Any of the following browsers and the corresponding driver (links to the drivers are provided at the end of the file):<br>
-Microsoft Edge<br>
-Chrome<br>
-Firefox<br>
<br>
Parametres:<br>
'-fp' : the exact path to the html file<br>
'-f'  : the path to the directory where the html file is<br>
'-n'  : the name of the html file (default:index.html)<br>
'-p'  : the port number you want the localhost to be hosted at (default:8080)<br>
'-d'  : the coresponding numer to your prefered browser ( 1 - Microsoft Edge  (default:2)<br>
                                                          2 - Chrome<br>
                                                          3 - Firefox )<br>
'-fd' : the exact path to the directory where the driver .exe is (default: C:\bin)<br> 
<br>
How to use:<br>
Run the easyrefresh.exe from cmd and specify the parametres (parametre order does not matter)<br>
A window will the open and your html file will be there.<br>
All you need to do now is to modify any file in the same directory on your editor and save. The browser will then instantly refresh.<br>
The app will crash if you move,create,delete any files in the file's directory.<br>
<br>
i.e.:<br>
  The simplest one:<br>
  <path>\easyrefresh\easyrefresh.exe -fp C:\Users\User1\Desktop\demo\demo.html --- The demo.html file is opened in localhost:8080 using Chrome<br>
  <br>
  <path>\easyrefresh\easyrefresh.exe -f C:\Users\User1\Desktop\demo -n demo.html --- This will also work the same way as the previous one<br>
  if the file's name is index.html the following can also be done:<br>
  <path>\easyrefresh\easyrefresh.exe -f C:\Users\User1\Desktop\demo             --- This will also work like the two previous examples<br>
  <br>
  <path>\easyrefresh\easyrefresh.exe -fp C:\Users\User1\Desktop\demo\demo.html -p 10 -d 1 -fd C:\bin\msedgedriver --- The demo file is opened in localhost:80 using Microsoft Edge
