
Why Ansible????
let me explain you the use of ansible with a small story.

I am the owner of the company called XYZ . I have hired some developers , testers ,Ops team , and 1 system administrator.
I have multiple computers installed in my office so they have to come to the office and work.
Now, let there is a Ram and Shyam . Ram is a system adminstrator and shyam is a developer.
Both are new joinee in my company. shyam work on day shift while Ram works on night shift .
BOth have same system assigned.
So, i as owner doesnt want my company whole access will be given to  employees . so i just created an acount for ram and shyam in same system .
as both have different shift so, same system can be assigned to both. now i give only some access to them depends on their job rols.
now , the Ram as a system administator his job is to install python in all the developers system of the comapny and selenium software in all testers of the company. 
One thing he can do is that he can manually access each one of system using ssh and install . but i have 1000k developer and 500 tester in my company.
he cant do that manually . as he will took a month to do that work.
And That comes the use of ansible . he just have to login as ram . write an inventory file where he mention all the ip address and divide into group for developer and tester . he also mention his own system ip becasuse his system is also assigned to 1 developer but the user name is shyam.
so he has to mention user name shyam and ip address of his system. because he want to install in that shyam account as shyam is also developer.
Now he can write one playbook where he mention for all developer install python module and for all tester install selenium module.
and just run that script using that single command . This will install software in all 1000k and 500k system parallely within few minutes.
Imagine how much time he saved just using ansible only.
Now the shyam login as shyam user in that system and he can find the software is installed in his system.
basically it was installed in his account.

in real life we dont give same system to developer and system administator. its just an expample that we can also mention our own ip in inventory file and user name can be different.

that's the use of ansible. Thanks for reading , hope now you have some idea about Ansible :) 




