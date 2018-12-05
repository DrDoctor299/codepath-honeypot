For this project, I deployed a honeypot through the penetration testing software "pentbox". 
I encountered issues with the "Modern Honey Network" installation on Google Cloud Platform VM, 
and elected instead to use a utility I found for Kali-Linux ("pentbox"). The pentbox utility is 
older, and as such, documentation surrounding its installation was frequently outdated. After
finding a download link, I was able to install the application onto Kali-linux with no trouble.

The honeypot detected 96 intrusions total, all of which originated from attacks I launched. 
As I was unable to get the honeypot working until recently, I was unable to leave it running for
a long period of time to attract roaming attackers. I simulated attacks from the outside by using
the nmap utility on kali-linux; having it attempt to map out the network of the honeypot, which 
was open on port 80. 

The messages sent to the honeypot by my commands were sometimes interesting to observe, oftentimes
containing characters not covered by the UTF-8 character set (and apparently not UNICODDE either) I'm
assuming that these requests to the "server" were intended to break things, but I'm not sure in what way.
I would be curious to find out how they function, and how the honeypot could be configured to be high interaction
so that more information could be caputured from the seemingly nonsense requests.
