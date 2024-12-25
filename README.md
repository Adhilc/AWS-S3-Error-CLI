# AWS-S3-Error-CLI
S3 Error: The difference between the request time and the current time is too large

problem statement:

--> aws s3 ls

Getting this error? here is the two steps that will help you...
________________________________________________________________


1.The time on your local box is out of sync with the current time. Sync up your system clock and the problem will go away.

2.Run these commands:
  sudo ntpdate ntp.ubuntu.com
  sudo apt-get install ntp

if at any time you get a message saying the NTP socket is still in use, stop it with 

"sudo /etc/init.d/ntp stop" and re-run your command.

