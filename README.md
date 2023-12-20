# ipinfo-automated-lookup
A Python 3 script that automates IP address lookup on IPInfo and displays the output in IPADDRESS[COUNTRY:ORGANIZATION] format. The script accepts IP address organization keyword/s and outputs the addresses matching the keyword/s (it is also capable of negating your searches). 

**NOTE:** It will require your IPInfo Access Token. 

The script/tool was made to address the need to lookup hundreds of IP addresses during analysis or investigation.

**How to Use**

Run the "iplooker.py" Python3 script on your machine; use the "-i" or "--ipList" option and specify the file location of the text file containing the list of IP addresses you want to lookup. Please note that the text file must be in a format that each IP address takes up one line, and no non-IP address content must be present. A samplelist.txt is available in the repository for your reference.

**Example:** iplooker.py -i C:\Users\$Username\Documents\List_of_IP_Addresses.txt

![image](https://github.com/UncleSocks/ipinfo-automated-lookup/assets/79778613/ff56eb5c-4da2-4b26-a869-ce46395aec3f)

When running the command, the script will ask for your IPInfo access token and your desired IP address organization keyword/s for searching. 

**NOTE:** When pasting the IPInfo token, use the right-click button of your mouse.

Use a space to separate multiple keywords (e.g., AMAZON MICROSOFT GOOGLE). The script will lookup each IP address in your text file list using the IPInfo API and will only output the addresses that matched ANY of the provided organization keywords. In short, the script will show you the list of addresses belonging to the organization/s in your search.

![image](https://github.com/UncleSocks/ipinfo-automated-lookup/assets/79778613/e68508ad-f521-4a7d-ba3c-f8a5fb8a52f9)

If you want to negate your search, prepend a "NOT" keyword on your search (e.g., NOT AMAZON MICROSOFT GOOGLE). Similarly, the script will still lookup each IP address inside the list using the IPInfo API but will only output the IP address that does not belong to the organization/s in your search.

![image](https://github.com/UncleSocks/ipinfo-automated-lookup/assets/79778613/25890c0b-0bc7-43e4-a0fd-9e0b29f9251c)

If you want to simply lookup all IP addresses in your list, use the "-" keyword.

![image](https://github.com/UncleSocks/ipinfo-automated-lookup/assets/79778613/9278f3eb-c5c7-4ea4-b84e-8830a72286e5)

**Output**

The script will display the result in IPADDRESS[COUNTRY:ORGANIZAITON] format. 




