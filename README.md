I will show you how to easily block the servers hosting Spotify ads on your Linux, Mac, or Windows machine. This will allow you to listen all day long on a free account without hearing a single ad or being tracked by third parties. This trick is very simple, legal, and works great.

To remove those pesky ads, all we need to do is set up our hosts file to override the DNS for Spotify's ad servers and redirect that traffic to our local machine.

When the traffic hits our local machine, the call will fail, and the third-party tracking and advertising will be skipped.

**Test Functionality:**
Open Spotify and ensure it functions as expected. Some ad and telemetry blocking might cause issues with specific features, so ensure essential functions are not disrupted.

**Regular Updates:**
Keep your hosts file updated with the latest entries from hosts file. Regular updates ensure ongoing privacy protection as new tracking domains emerge.

Download & open [**hosts**](https://github.com/x0uid/SpotifyAdBlock/blob/master/hosts) file using your favorite text editor. 

**For Windows 11, 10 & 8:**

*Press the Windows key.*
*Type Notepad in the search field.*
*In the search results, right-click Notepad and select Run as administrator.*
*From Notepad, open the following file: c:\Windows\System32\Drivers\etc\hosts*
*Make the necessary changes to the file. Click File > Save to save your changes.*

**For Linux:**

*Open a terminal window.*
*Open the hosts file in a text editor (you can use any text editor) by typing the following line:*

*sudo nano /etc/hosts*

**For Mac OS X 10.6 through 10.12:**

*Open Applications > Utilities > Terminal.*
*Open the hosts file by typing the following line in the terminal window:*

*sudo nano /private/etc/hosts*

*Type your domain user password when prompted.*
*Edit the hosts file.The file contains some comments (lines starting with the # symbol), and some default hostname mappings* (for example, 127.0.0.1 – local host). Add your new mappings after the default mappings.*
*Save the hosts file by pressing Control+x and answering y.*
*Make your changes take effect by flushing the DNS cache with the following command:*

*dscacheutil -flushcache*

*There you go, editing hosts file has taken effect.*

It is advisable to clear Spotify cache afterwards in order for the changes to take effect.


**Pi-hole compatible versions can be found here:**

Blocklist: https://github.com/x0uid/SpotifyAdBlock/blob/master/SpotifyBlocklist.txt  
Whitelist: https://gist.github.com/captainhook/9eb4132d6e58888e37c6bc6c73dd4e60  
Bash script to import whitelist: https://gist.github.com/captainhook/f4ccfc82dc6696270d62b54b13f871c4  
Credits to: [captainhook](https://github.com/captainhook)

## Buy me a coffee
I have maintained this ad-blocking list because I am passionate about this, and i think u have all the right to protect your privacy while enjoying music. 
Donations are one of the many ways to support what I do.

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://paypal.me/anis)
