# Introduction to the skills of pentesting

## Create a TryHackMe account!
After account registration, the sidebar is where I should start. "Learning Paths" makes the most sense in this case. Even doing anything in life, we need to have specific goals to reach. When things get tough, there is still something to follow. 

### Basic things to do
To hack machines in TryHackMe, there are 2 ways
- Connect using OpenVPN (free)
  - Download OpenVPN
  - Install configuration file
  - Run OpenVPN
  - Check status
- Connect using Browser Kali Machine (premium feature)

## Researching 
When encountering problems that cannot be solved, how to keep going?
It is normal not to know everything, therefore one should have a reliable source of reference for knowledge base.
Google is a very useful search engine in information security.

### Vulnerability searching
Content Management Systems (CMS) like Wordpress, FuelCMS, Ghost are among the popular target. CMSs are meant to ease the process of setting up websites and hackers take the advantage of this convenience to their benefit.

#### Out of the box exploits
There are also ready-to-use exploits that can be downloaded. Figuring out the version of the target CMS is an important step in reconnaissance.
These 3 websites are useful if we want to search for the exploits related to a specific software.
- [ExploitDB](https://www.exploit-db.com/)
- [National Vulnerability Database (NVD)](https://nvd.nist.gov/vuln/search)
- [Common Vulnerabilities and Exposures (CVE) Mitre](https://cve.mitre.org/)

NVD keeps track of exploits in the following form:
CVE-YEAR-IDNUMBER

#### Exploit searching 
Search for exploits on [ExploitDB](https://www.exploit-db.com/). Say that I am looking for exploits on a FuelCMS:
- Personal Kali machine
  - Use the command `searchsploit fuelcms`
- The website
  - Type "fuelcms" in the search bar and hit enter
  - The only FuelCMS exploit with CVE number is 1.4.1
  - Learn more about the exploit by clicking on the exploit

### Utilizing manual pages on the console
We can use the manual page when interacting with the tools inside the terminal.
- For example: How to use the `ssh` command?
  - Invoke `man ssh` to get the manual page for SSH
  - Referring "DESCRIPTION", invoke `ssh user@hostname` to use SSH
- Switches
  - Include switches to make the command execute the other tasks
    - How can we see the version of our SSH?
    - The switch `-V` will do the job
    - The full command: `ssh -V`
- Search with the `grep` command
  - Filter out everything else and search specifically for what we require
    - Invoke `man ssh | grep -e "version number"`
