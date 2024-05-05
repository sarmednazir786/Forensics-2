## Title: Man in the Middle
## Details:
* difficulty: Medium
* category: Forensics
* author: Sarmed
* flags: flag{solved}

## Description:
This is a medium difficulty lab where a traffic capture file has been provided and analysis is required to capture the flag.

## Hint:
Keep it simple.

## Intended Learning and outcome:
With the given challenge, I was able to learn the importance of encrypted traffic and how to analyze captured traffic. 

## Solution: 
The provided traffic file can be analyzed with many different tools, I'll be using wireshark. When we open the file in wireshark, we see 2 packets. We the proceed to right click on the first and click **Follow -> TCP Stream**. A page opens that shows a message which contains a link as well as a password stating that the link to the image has an embedded file. We then download the image from that link and use steghide to extract the embedded file that contains the flag.

........
