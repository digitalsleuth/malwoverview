# Malwoverview.py

[<img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/alexandreborges/malwoverview?color=Red&style=for-the-badge">](https://github.com/alexandreborges/malwoverview/releases/tag/3.1.2) [<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/alexandreborges/malwoverview?color=Yellow&style=for-the-badge">](https://github.com/alexandreborges/malwoverview/releases) [<img alt="GitHub Release Date" src="https://img.shields.io/github/release-date/alexandreborges/malwoverview?label=Release%20Date&style=for-the-badge">](https://github.com/alexandreborges/malwoverview/releases) [<img alt="GitHub" src="https://img.shields.io/github/license/alexandreborges/malwoverview?style=for-the-badge">](https://github.com/alexandreborges/malwoverview/blob/master/LICENSE) 
[<img alt="GitHub stars" src="https://img.shields.io/github/stars/alexandreborges/malwoverview?logoColor=Red&style=for-the-badge">](https://github.com/alexandreborges/malwoverview/stargazers) [<img alt="Twitter Follow" src="https://img.shields.io/twitter/follow/ale_sp_brazil?color=blueviolet&style=for-the-badge">](https://twitter.com/ale_sp_brazil)
[<img alt="PayPal" src="https://img.shields.io/badge/Donate-Paypal-brightgreen?style=for-the-badge&logo=appveyor">](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=M8F458EZH8UZE&source=url)


![Alt text](pictures/picture_1.jpg?raw=true "Title")
![Alt text](pictures/picture_2.jpg?raw=true "Title")
![Alt text](pictures/picture_3.jpg?raw=true "Title")
![Alt text](pictures/picture_4.jpg?raw=true "Title")
![Alt text](pictures/picture_5.jpg?raw=true "Title")
![Alt text](pictures/picture_6.jpg?raw=true "Title")
![Alt text](pictures/picture_7.jpg?raw=true "Title")
![Alt text](pictures/picture_8.jpg?raw=true "Title")
![Alt text](pictures/picture_9.jpg?raw=true "Title")
![Alt text](pictures/picture_10.jpg?raw=true "Title")
![Alt text](pictures/picture_11.jpg?raw=true "Title")
![Alt text](pictures/picture_12.jpg?raw=true "Title")
![Alt text](pictures/picture_13.jpg?raw=true "Title")
![Alt text](pictures/picture_14.jpg?raw=true "Title")
![Alt text](pictures/picture_15.jpg?raw=true "Title")
![Alt text](pictures/picture_16.jpg?raw=true "Title")
![Alt text](pictures/picture_17.jpg?raw=true "Title")
![Alt text](pictures/picture_18.jpg?raw=true "Title")
![Alt text](pictures/picture_19.jpg?raw=true "Title")
![Alt text](pictures/picture_20.jpg?raw=true "Title")
![Alt text](pictures/picture_21.jpg?raw=true "Title")
![Alt text](pictures/picture_22.jpg?raw=true "Title")
![Alt text](pictures/picture_23.jpg?raw=true "Title")
![Alt text](pictures/picture_24.jpg?raw=true "Title")
![Alt text](pictures/picture_25.jpg?raw=true "Title")
![Alt text](pictures/picture_26.jpg?raw=true "Title")
![Alt text](pictures/picture_27.jpg?raw=true "Title")
![Alt text](pictures/picture_28.jpg?raw=true "Title")
![Alt text](pictures/picture_29.jpg?raw=true "Title")
![Alt text](pictures/picture_30.jpg?raw=true "Title")
![Alt text](pictures/picture_31.jpg?raw=true "Title")
![Alt text](pictures/picture_32.jpg?raw=true "Title")
![Alt text](pictures/picture_33.jpg?raw=true "Title")
![Alt text](pictures/picture_34.jpg?raw=true "Title")
![Alt text](pictures/picture_35.jpg?raw=true "Title")
![Alt text](pictures/picture_36.jpg?raw=true "Title")
![Alt text](pictures/picture_37.jpg?raw=true "Title")
![Alt text](pictures/picture_38.jpg?raw=true "Title")
![Alt text](pictures/picture_39.jpg?raw=true "Title")
![Alt text](pictures/picture_40.jpg?raw=true "Title")
![Alt text](pictures/picture_41.jpg?raw=true "Title")
![Alt text](pictures/picture_42.jpg?raw=true "Title")
![Alt text](pictures/picture_43.jpg?raw=true "Title")
![Alt text](pictures/picture_44.jpg?raw=true "Title")
![Alt text](pictures/picture_45.jpg?raw=true "Title")
![Alt text](pictures/picture_46.jpg?raw=true "Title")
![Alt text](pictures/picture_47.jpg?raw=true "Title")
![Alt text](pictures/picture_48.jpg?raw=true "Title")
![Alt text](pictures/picture_49.jpg?raw=true "Title")
![Alt text](pictures/picture_50.jpg?raw=true "Title")
![Alt text](pictures/picture_51.jpg?raw=true "Title")

      Copyright (C)  2018-2020 Alexandre Borges <alexandreborges at blackstormsecurity dot com>

      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      (at your option) any later version.

      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.

      See GNU Public License on <http://www.gnu.org/licenses/>.


# Current Version: 3.1.2

## Important note:  Malwoverview does NOT submit samples to Virus Total or Hybrid Analysis by default. It submits only hashes, so respecting Non-Disclosure Agreements (NDAs). Nonetheless, if you use the "-V" (uppercase), "-A" (uppercase) or "-P" (uppercase), so Malwoverview SUBMITS your malware sample to Virus Total, Hybrid Analysis and Polyswarm, respectively. 


# ABOUT

Malwoverview.py is a simple tool to perform an initial and quick triage of malware samples, URLs and hashes. 
Additionally, Malwoverview is able to show some threat intelligence information.   

This tool aims to : 

1. Determine similar executable malware samples (PE/PE+) according to the import table (imphash) and group 
   them by different colors (pay attention to the second column from output). Thus, colors matter!
2. Show hash information on Virus Total, Hybrid Analysis, Malshare, Polyswarm and URLhaus engines. 
3. Determining whether the malware samples contain overlay and, if you want, extract it. 
4. Check suspect files on Virus Total, Hybrid Analysis and Polyswarm.
5. Check URLs on Virus Total, Malshare, Polyswarm and URLhaus engines. 
6. Download malware samples from Hybrid Analysis, Malshare and HausURL engines.
7. Submit malware samples to VirusTotal, Hybrid Analysis and Polyswarm.
8. List last suspected URLs from URLHaus.
9. List last payloads from URLHaus. 
10. Search for specific payloads on the Malshare.
11. Search for similar payloads (PE32/PE32+) on Polyswarm engine.
12. Classify all files in a directory searching information on Virus Total and Hybrid Analysis. 
13. Make reports about a suspect domain. 
14. Check APK packages directly from Android devices against Hybrid Analysis and Virus Total. 
15. Submit APK packages directly from Android devices to Hybrid Analysis and Virus Total. 
16. Show URLs related to an user provided tag from URLHaus.
17. Show payloads related to a tag (signature) from URLHaus.
18. Show information about an IP address from Virus Total.
19. Show IP address, domain and URL information from Polyswarm. 
20. List different types of payloads from Malshare along their Yara hits. 

# CONTRIBUTORS:

      Alexandre Borges (project owner)
      Corey Forman (https://github.com/digitalsleuth)

# REQUERIMENTS

This tool has been tested on Ubuntu, Kali Linux 2020, REMnux, Windows 8.1 and 10. Malwoverview can be installed by executing the following command:

      pip3.8 install git+https://github.com/alexandreborges/malwoverview (preferred method) 
      or...
      python -m pip install malwoverview
      or...
      git clone https://github.com/alexandreborges/malwoverview


To use Malwoverview you should insert VirusTotal, Hybrid Analysis, URLHaus, Malshare and Polyswarm APIs into the .malwapi.conf configuration 
file (the default one at the home directory -- if the file doesn't exist, so you should create it) or you could create a custom configuration file
and indicate it by using the -c option. 

The .malwapi.conf configuration file (from the the home directory) has the following format: 

      [VIRUSTOTAL]
      VTAPI = 

      [HYBRID-ANALYSIS]
      HAAPI = 

      [MALSHARE]
      MALSHAREAPI = 

      [HAUSSUBMIT]
      HAUSSUBMITAPI = 

      [POLYSWARM]
      POLYAPI = 

In Windows systems, when the package is installed using pip, the suggestion is to create the .malwapi.conf in either C:\Users\<username> directory. 
Additionally, you don't need to specify "-w 1" option while using malwoverview.py on Windows anymore. 

To check the installation, execute:

       malwoverview.py --help
       
Further information is available on: 

       (PYPI.org repository) https://pypi.org/project/malwoverview/
       (Github) https://github.com/alexandreborges/malwoverview

If you want to perform the manual steps, so few steps will be necessary:

## Kali Linux

1. Python version 3.8 or later (Only Python 3.x !!! It does NOT work using Python 2.7) 

       $ apt-get install python3.8  (for example)
            
2. Python-magic.  

      To install python-magic package you can execute the following command:
      
       $ pip3.8 install python-magic
      
      Or compiling it from the github repository:
      
       $ git clone https://github.com/ahupp/python-magic
       $ cd python-magic/
       $ python3.8 setup.py build
       $ python3.8 setup.py install
      
      As there are serious problems about existing two versions of python-magic package, my recommendation is to install it
      from github (second procedure above) and copy the magic.py file to the SAME directory of malwoverview tool. 
      
3. Install several Python packages: 

       $ pip3.8 install -r requirements.txt
       
       OR
       
       $ pip3.8 install -U pefile
       $ pip3.8 install -U colorama
       $ pip3.8 install -U simplejson
       $ pip3.8 install -U python-magic
       $ pip3.8 install requests==2.2.22
       $ pip3.8 install -U validators
       $ pip3.8 install -U geocoder
       $ pip3.8 install polyswarm-api==1.1.1
       $ pip3.8 install -U pathlib
       $ pip3.8 install -U configparser
       
4. To check an Android mobile you need to install the "adb" program by executing the following command:

       # apt get install adb

   PS: before trying Android's options, check:
       
       * If the adb program is listed in the PATH environment variable.
       * If the system has authorized access to the device by using "adb devices -l"

## Windows

1. Install the Python version 3.8.x or later from https://www.python.org/downloads/windows/ 

2. Python-magic.  

      To install python-magic package you can execute the following command:
      
       C:\> python.exe -m pip install python-magic
      
      Or compiling it from the github repository:
      
       C:\> git clone https://github.com/ahupp/python-magic
       C:\> cd python-magic/
       C:\> python.exe setup.py build
       C:\> python.exe setup.py install
      
3. Install several Python packages: 
      
       C:\> python.exe -m pip install -r requirements.txt
       
       OR: 
       
       C:\> python.exe -m pip install pefile
       C:\> python.exe -m pip install colorama
       C:\> python.exe -m pip install simplejson
       C:\> python.exe -m pip install python-magic
       C:\> python.exe -m pip install requests
       C:\> python.exe -m pip install validators
       C:\> python.exe -m pip install geocoder
       C:\> python.exe -m pip install polyswarm-api
       C:\> python.exe -m pip install pathlib
       C:\> python.exe -m pip install configparser
       C:\> python.exe -m pip install python-magic-bin

4. To check an Android mobile you need to install the "adb" program by:

       * Downloading and installing the Android Studio from: https://developer.android.com/studio#downloads (Recommended)
       * Downloading it from https://dl.google.com/android/repository/platform-tools-latest-windows.zip
   
   PS: before trying Android's options, check:
       
       * If the adb program is listed in the PATH environment variable.
       * If the system has authorized access to the device by using "adb devices -l"

       
# USAGE

To use the malwoverview, execute the command as shown below:

      root@ubuntu19:~/malwoverview# python3.8 malwoverview.py  | more

      usage: python malwoverview.py -c <config file> -d <directory> -f <fullpath> -i <0|1> -b <0|1> -v <0|1>
      -a <0|1> -p <0|1> -s <0|1> -x <0|1> -w <|1> -u <url> -H <hash file> -V <filename> -D <0|1> -e<0|1|2|3|4>
      -A <filename> -g <job_id> -r <domain> -t <0|1> -Q <0|1> -l <0|1> -n <1-12> -m <hash> -M <0|1> 
      -U <url> -S <url> -z <tags> -B <0|1> -K <0|1> -j <hash> -J <hash> -P <filename> -N <url> 
      -R <PE file, IP address, domain or URL> -G <0|1|2|3|4> -y <0|1> -Y <file name> -Z <0|1> 
      -X <0|1> -Y <file name> -T <file name> -W <tag> -k <signature> -I <ip address>


Malwoverview is a malware triage tool written by Alexandre Borges.

      optional arguments:

      -h, --help        show this help message and exit
      -c CONFIG FILE, --config CONFIG FILE
                        Use a custom config file to specify API's
      -d DIRECTORY, --directory DIRECTORY
                        specify directory containing malware samples.
      -f FILENAME, --filename FILENAME
                        Specifies a full path to a file. Shows general information about the file (any filetype)
      -b BACKGROUND, --background BACKGROUND
                        (optional) Adapts the output colors to a white terminal. The default is black terminal
      -i IAT_EAT, --iat_eat IAT_EAT
                        (optional) Shows imports and exports (it is used with -f option).
      -x OVERLAY, --overlay OVERLAY
                        (optional) Extracts overlay (it is used with -f option).
      -s SHOW_VT_REPORT, --vtreport SHOW_VT_REPORT
                        Shows antivirus reports from the main players. This option is used with the -f option (any filetype).
      -v VIRUSTOTAL, --virustotal VIRUSTOTAL
                        Queries the Virus Total database for positives and totals.Thus, you need to edit the configmalw.py 
                        and insert your VT API.
      -a HYBRID_ANALYSIS, --hybrid HYBRID_ANALYSIS
                        Queries the Hybrid Analysis database for general report. Use the -e option to specify which 
                        environment are looking for the associate report because the sample can have been submitted to a 
                        different environment that you are looking for. Thus, you need to edit the configmalw.py i
                        and insert your HA API and secret.
      -p USE_VT_PUB_KEY, --vtpub USE_VT_PUB_KEY
                        (optional) You should use this option if you have a public Virus Total API. It forces a one 
                        minute wait every 4 malware samples, but allows obtaining a complete evaluation of the 
                        malware repository.
      -w RUN_ON_WINDOWS, --windows RUN_ON_WINDOWS
                        This option is used when the OS is Microsoft Windows.
      -u URL_VT, --vturl URL_VT
                        SUBMITS a URL for the Virus Total scanning.
      -I IP_VT, --ipaddrvt IP_VT
                        This options checks an IP address on Virus Total.
      -r URL_DOMAIN, --urldomain URL_DOMAIN
                        GETS a domain's report from Virus Total.
      -H FILE_HASH, --hash FILE_HASH
                        Specifies the hash to be checked on Virus Total and Hybrid Analysis. For the Hybrid Analysis
                        report you must use it together -e option.
      -V FILENAME_VT, --vtsubmit FILENAME_VT
                        SUBMITS a FILE(up to 32MB) to Virus Total scanning and read the report. Attention: use forward 
                        slash to specify the target file even on Windows systems. Furthermore, the minimum waiting time
                        is set up in 90 seconds because the Virus Total queue. If an error occurs, so wait few minutes 
                        and try to access the report by using -f option.
      -A SUBMIT_HA, --submitha SUBMIT_HA
                        SUBMITS a FILE(up to 32MB) to be scanned by Hybrid Analysis engine. Use the -e option to specify
                        the best environment to run the suspicious file.
      -g HA_STATUS, --hastatus HA_STATUS
                        Checks the report's status of submitted samples to Hybrid Analysis engine by providing the 
                        job ID. Possible returned status values are: IN_QUEUE, SUCCESS, ERROR, IN_PROGRESS and 
                        PARTIAL_SUCCESS.
      -D DOWNLOAD, --download DOWNLOAD
                        Downloads the sample from Hybrid Analysis. Option -H must be specified.
      -e HA_ENVIRONMENT, --haenv HA_ENVIRONMENT
                        This option specifies the used environment to be used to test the samlple on Hybrid Analysis:
                        <0> Windows 7 32-bits; <1> Windows 7 32-bits (with HWP Support); <2> Windows 7 64-bits; 
                        <3> Android; <4> Linux 64-bits environment. This option is used together either -H option 
                        or the -A option or -a option.
      -t MULTITHREAD, --thread MULTITHREAD
                        (optional) This option is used to force multithreads on Linux whether: the -d option is specifed
                        AND you have a PAID Virus Total API or you are NOT checking the VT while using the -d option.
                        PS1: using this option causes the Imphashes not to be grouped anymore; PS2: it also works on 
                        Windows, but there is not gain in performance.
      -Q QUICK_CHECK, --quick QUICK_CHECK
                        This option should be used with -d option in two scenarios: 1) either including the -v option
                        (Virus Total -- you'll see a complete VT response whether you have the private API) for a 
                        multithread search and reduced output; 2) or including the -a option (Hybrid Analysis) for a
                        multithread search and complete and amazing output. If you are using the -a option, so -e option
                        can also be used to adjust the output to your sample types. PS1: certainly, if you have a
                        directory holding many malware samples, so you will want to test this option with -a option; i
                        PS2: it also works on Windows, but there is not gain in performance.
      -l MALSHARE_HASHES, --malsharelist MALSHARE_HASHES
                        Show hashes from last 24 hours from Malshare. You need to insert your Malshare API into the
                        configmalw.py file.
      -m MALSHARE_HASH_SEARCH, --malsharehash MALSHARE_HASH_SEARCH
                        Searches for the provided hash on the Malshare repository. You need to insert your Malshare API
                        into the configmalw.py file. PS: sometimes the Malshare website is unavailable, so should check
                        the website availability if you get some error message.
      -n FILE_TYPE, --filetype FILE_TYPE
                        Specifies the file type to be listed by -l option. Therefore, it must be used together i
                        -l option. Possible values: 1: PE32 (default) ; 2: Dalvik ; 3: ELF ; 4: HTML ; 5: ASCII ; 
                        6: PHP ; 7: Java ; 8: RAR ; 9: Zip ; 10: UTF-8 ; 11: MS-DOS ; 12: data ; 13: PDF ; i
                        14: Composite(OLE).
      -M MALSHARE_DOWNLOAD, --malsharedownload MALSHARE_DOWNLOAD
                        Downloads the sample from Malshare. This option must be specified with -m option.
      -B URL_HAUS_BATCH, --haus_batch URL_HAUS_BATCH
                        Retrieves a list of recent URLs (last 3 days, limited to 1000 entries) from URLHaus website.
      -K HAUS_PAYLOADS, --haus_payloadbatch HAUS_PAYLOADS
                        Retrieves a list of downloadable links to recent PAYLOADS (last 3 days, limited to 1000 
                        entries) from URLHaus website. Take care: each link take you to download a passworless zip file
                        containing a malware, so your AV can generate alerts!
      -U URL_HAUS_QUERY, --haus_query URL_HAUS_QUERY
                        Queries a URL on the URLHaus website.
      -j HAUS_HASH, --haus_hash HAUS_HASH
                        Queries a payload's hash (md5 or sha256) on the URLHaus website.
      -S URL_HAUS_SUB, --haus_submission URL_HAUS_SUB
                        Submits a URL used to distribute malware (executable, script, document) to the URLHaus website.
                        Pay attention: Any other submission will be ignored/deleted from URLhaus. You have to register
                        your URLHaus API into the configmalw.py file.
      -z [HAUSTAG [HAUSTAG ...]], --haustag [HAUSTAG [HAUSTAG ...]]
                        Associates tags (separated by spaces) to the specified URL. Please, only upper case, lower 
                        case, '-' and '.' are allowed. This parameter is optional, which could be used with the 
                        -S option.
      -W [HAUSTAGSEARCH [HAUSTAGSEARCH ...]], --haustagsearch [HAUSTAGSEARCH [HAUSTAGSEARCH ...]]
                        This option is for searching malicious URLs by tag on URLhaus. Tags are case-senstive and only
                        upper case, lower case, '-' and '.' are allowed.
      -k [HAUSSIGSEARCH [HAUSSIGSEARCH ...]], --haussigsearch [HAUSSIGSEARCH [HAUSSIGSEARCH ...]]
                        This option is for searching malicious payload by tag on URLhaus. Tags are case-sensitive and
                        only upper case, lower case, '-' and '.' are allowed.
      -J HAUS_DOWNLOAD, --haus_download HAUS_DOWNLOAD
                        Downloads a sample (if it is available) from the URLHaus repository. It is necessary to provide
                        the SHA256 hash.
      -P POLYSWARMFILE, --polyswarm_scan POLYSWARMFILE
                        (Only for Linux) Performs a file scan using the Polyswarm engine.
      -N POLYSWARMURL, --polyswarm_url POLYSWARMURL
                        (Only for Linux) Performs a URL scan using the Polyswarm engine.
      -O POLYSWARMHASH, --polyswarm_hash POLYSWARMHASH
                        (Only for Linux) Performs a hash scan using the Polyswarm engine.
      -R POLYSWARMMETA, --polyswarm_meta POLYSWARMMETA
                        (Only for Linux) Performs a complementary search for similar PE executables through 
                        meta-information or IP addresses using the Polyswarm engine. This parameters depends on
                        -G parameters, so check it, please.
      -G METATYPE, --metatype METATYPE
                        (Only for Linux) This parameter specifies whether the -R option will gather information about
                        the PE executable or IP address using the Polyswarm engine. Thus, 0: PE Executable ;
                        1: IP Address ; 2: Domains ; 3. URL.
      -y ANDROID_HA, --androidha ANDROID_HA
                        Check all third-party APK packages from the USB-connected Android device against Hybrid Analysis
                        using multithreads. The Android device does not need be rooted and you need have adb in your 
                        PATH environment variable.
      -Y ANDROID_SEND_HA, --androidsendha ANDROID_SEND_HA
                        Send an third-party APK packages from your USB-connected Android device to Hybrid Analysis. The
                        Android device does not need be rooted and you need have adb in your PATH environment variable.
      -T ANDROID_SEND_VT, --androidsendvt ANDROID_SEND_VT
                        Send an third-party APK packages from your USB-connected Android device to Virus Total. The 
                        Android device does not need be rooted and you need have adb in your PATH environment variable.
      -Z ANDROID_VT, --androidvt ANDROID_VT
                        Check all third-party APK packages from the USB-connected Android device against VirusTotal 
                        using Public API (slower because of 60 seconds delay for each 4 hashes). The Android device 
                        does not need be rooted and you need have adb in your PATH environment variable.
      -X ANDROID_VT, --androidvtt ANDROID_VT
                        Check all third-party APK packages from the USB-connected Android device against VirusTotal 
                        using multithreads (only for Private Virus API). The Android device does not need be rooted and
                        you need have adb in your PATH environment variable.
                        

        Remember that public VT API only allows 4 searches per second (as shown at the image above). Therefore,
        if you are willing to wait some minutes, so you can use the -p option, which forces a one minute wait 
        every 4 malware samples, but allows obtaining a complete evaluation of the repository.


        * ATTENTION 1: if the directory contains many malware samples while using -d option, so malwoverview.py
                       could take some time. Nonetheless, you can use the new -t option (multithreading) to
                       speed-up things. :)
         
        ** ATTENTION 2: All engines enforces quota of submission and/or verification per day and/or month. 
                        Take care!
        
        *** ATTENTION 3: Some options searching on Hybrid Analysis strongly depend of the "-e" option, which 
                         specifies the environment. Therefore, to check an Android sample (for example) it is 
                         necessary to use the right environment (-e 3 for Android).
        
        **** ATTENTION 4: When you execute Malwoverview on Windows systems, you MUST to specify the "-w 1" option
                          if you've clone using git tool. 


## Examples:

      python3.8 malwoverview.py -d /root/malware/misc/
      python3.8 malwoverview.py -d /root/malware/misc/ -t 1
      python3.8 malwoverview.py -d /root/malware/misc/ -t 1 -v 1
      python3.8 malwoverview.py -d /root/malware/misc/ -v 1 -p 1
      python3.8 malwoverview.py -d /root/malware/misc/ -Q 1 -v 1
      python3.8 malwoverview.py -d /root/malware/misc/ -Q 1 -a 1
      python3.8 malwoverview.py -d /root/malware/android/ -Q 1 -a 1 -e 3
      python3.8 malwoverview.py -d /root/malware/linux/ -Q 1 -a 1 -e 4
      python3.8 malwoverview.py -f /root/malware/misc/sample1 -v 1 -s 1
      python3.8 malwoverview.py -f /root/malware/misc/sample1 -i 1
      python3.8 malwoverview.py -f /root/malware/misc/sample1 -v 1 -s 1 -x 1
      python3.8 malwoverview.py -u <url>
      python3.8 malwoverview.py -r <domain>
      python3.8 malwoverview.py -H <hash> -e 2
      python3.8 malwoverview.py -H <hash> -e 1
      python3.8 malwoverview.py -V /root/malware/android/sample.apk
      python3.8 malwoverview.py -A /root/malware/windows/sample1
      python3.8 malwoverview.py -A /root/malware/android/sample.apk -e 3
      python3.8 malwoverview.py -g <job_id>
      python3.8 malwoverview.py -l 1
      python3.8 malwoverview.py -l 1 -n 2
      python3.8 malwoverview.py -l 1 -n 3
      python3.8 malwoverview.py -m <hash>
      python3.8 malwoverview.py -m <hash> -M 1
      python3.8 malwoverview.py -B 1
      python3.8 malwoverview.py -U <URL>
      python3.8 malwoverview.py -K 1
      python3.8 malwoverview.py -j <hash>
      python3.8 malwoverview.py -J <hash>
      python3.8 malwoverview.py -S <URL> -z SpelevoEK exe psixbot
      python3.8 malwoverview.py -O <hash>
      python3.8 malwoverview.py -N <URL>
      python3.8 malwoverview.py -P sample1
      python3.8 malwoverview.py -R /root/malware/windows/sample1
      python3.8 malwoverview.py -y 1
      python3.8 malwoverview.py -Y skype
      python3.8 malwoverview.py -Z 1
      python3.8 malwoverview.py -X 1
      python3.8 malwoverview.py -T twitter 
      python3.8 malwoverview.py -u https://toulousa.com/omg/159EYJSFYHMS.exe
      python3.8 malwoverview.py -k Trickbot
      python3.8 malwoverview.py -m e47a415662b5fad1f3049764456ba2ac33a1bde6fd3181ec2b658d382ad17d41
      python3.8 malwoverview.py -W mirai
      python3.8 malwoverview.py -I 149.56.79.215
      python3.8 malwoverview.py -R 164.132.92.180 -G 1
      python3.8 malwoverview.py -R sndoffo79.ddns.net -G 2
      python3.8 malwoverview.py -R http://t.turconfiok.pro -G 3


# HISTORY

Version 3.1.2:

      This version:
      
            * Introduces the -c option that allows the user to specify a custom API configuration file. 
            * The API configuration file has been changed to .malwapi.conf file.
            * The project structure has been changed to make easier to install it in different operating 
              systems.
            * Updates for this version are a contribution from Corey Forman (https://github.com/digitalsleuth).
            
Version 3.0.0:

      This version:
      
            * Includes fixes in the URL reporting (-u option) from Virus Total.  
            * New players have have been included in the URL reporting (-u option) from Virus Total.
            * Fixes have been included in payload listing (-K option) from URLhaus.
            * Yara information has been include in the hash report (-m option) from Malshare.
            * Fixes have been included in the -l option. 
            * New file types have been included in the -n option: Java, Zip, data, RAR, PDF, Composite (OLE),
              MS_DOS and UTF-8.
            * New -W option, which is used to show URLs related to an user provided tags from URLHaus.
            * New -k option, which is used to show payloads related to a tag from URLHaus
            * New -I option, which is used to show information related to an IP address from Virus Total.
            * The -R option was refactored and now it supports searching for file, IPv4, domain or URL on 
              Polyswarm. 

Version 2.5.0:

      This version:
      
            * Introduces the following options:
                  * -y to check all third-party APKs from an Android device against 
                       the Hybrid Analysis. 
                  * -Y to send a third-party APKs from an Android device to the Hybrid
                       Analysis. 
                  * -Z to check all third-party APKs from an Android device against 
                       the Virus Total. 
                  * -X to check all third-party APKs from an Android device against the
                       Virus Total (it is necessary private API). 
                  * -T to send a third-party APK from an Android device to Virus Total. 
            * Fixes several issues related to color in command outputs.  
            * Adds the filename identification in the report while sending a sample to Virus Total.

Version 2.1.9.1:

      This version:
      
            * Fixes several issues about colors in outputs. 
            * Removes the -L option from Malshare (unfortunately, Malshare doesn't provide an 
              URL list anymore). 
            * Removes the -c option.
            * Introduces some verification lines in the URLHaus command. 

Version 2.1:

      This version:
      
            * Fixes formatting issues related to Hybrid Analysis output (-Q 1 -a 1). 
            * Fixes color issues. 
            * Fixes small issues related to Polyswarm. 

Version 2.0.8.1:

      This version:
      
            * Introduces installation using: pip3.8 install malwoverview (Linux) or 
              python -m pip install malwoverviewwin (Windows). 
            * Fixes small problems related to Polyswarm usage. 
            * Changes the help to verify whether the APIs were inserted into configmalw.py file. 

Version 2.0.1:

      This version:
      
            * Fixes a problem related to searching by hash on Malshare (-m option). 
            * Fixes a problem related to searching by hash on Polyswarm (-O option). 

Version 2.0.0:

      This version:
      
            * Introduces a completely ported version of Malwoverview to Python 3.x (it does not work in 
              Python 2.7.x anymore!)
            * Fixes several bugs related to IAT/EAT listing. 
            * Fixes several bugs related to colors. 
            * Introduces multi-threading to some options. 
            * Introduces several options related to Malshare. 
            * Introduces several options related to URLHaus.
            * Introduces several options related to Polyswarm engine. 
            * Changes the place of the API key configuration. Now you should edit the configmalw.py file. 
            * Changes the help libraries and functions, so making the Malwoverview's help more complete. 
            * Introduces geolocation feature by using the package named Geocoder written by Dennis Carrierre.
            * Fixes problems related to Hybrid Analysis engine. 
            * Fixes several mistaked related to a mix between spaces and Tab.
            * Extends the -d option to include Hybrid Analysis. 
            
Version 1.7.5:

      This version: 
      
            * It has been fixed a problem related to sample submission to Hybrid Analysis on Windows operating 
              system. Additionally, file name handling has been also fixed. 
            
Version 1.7.3:

      This version: 
      
            * Malwoverview has been adapted to API version 2.6.0 of Hybrid Analysis.
            * -A option has been fixed according to new version (2.6.0) of Hybrid Analysis.
            * -a option has been modified to work together with  -e option.
            * help information has been modified. 
            
Version 1.7.2:

      This version: 
      
            * A small fix related to -g option has been included. 
            
Version 1.7.1:

      This version: 
      
            * Relevant fix of a problem related to options -A and -H options.
            * Includes a new Hybrid Analysis environment to the -e option (Windows 7 32-bits with HWP support).
            * Updates the Malwoverview to support Hybrid Analysis API version 2.5.0.
            
Version 1.7.0:

      This version: 
      
            * Includes -A option for submitting a sample to Hybrid Analysis.
            * Includes -g option for checking the status a submission of a sample to Hybrid Analysis.
            * Includes -e option for specifying the testing environment on the Hybrid Analysis.
            * Includes -r option for getting a complete domain report from Virus Total.
            * Modifies the -H options for working together the -e option.
            * Modifies several functions of the tool to prepare it for version 1.8.0
            
Version 1.6.3:

      This version: 
      
            * Includes creation of new functions aiming 1.7.0 version.
            * Includes new exception handling blocks.
            
Version 1.6.2:

      This version: 
      
            * Includes small fixes.
            * For the Hybrid Analysis API version 2.40 is not longer necessary to include the API Secret.  
            
Version 1.6.1:

      This version: 
      
            * Includes small format fixes.
            
Version 1.6.0:

      This version: 
      
            * It is using the Hybrid Analysis API version 2.4.0.
            * Includes certificate information in the Hybrid Analysis report. 
            * Includes MITRE information in the Hybrid Analysis report. 
            * Includes an option to download samples from Hybrid Analysis. 
            
Version 1.5.1:

      This version: 
      
            * Small change to fix format issue in -d option. 
      
Version 1.5.0:

      This version: 
      
            * Includes the -u option to check URLs against Virus Total and associated engines. 
            * Includes the -H option to find existing reports on Virus Total and Hybrid Analysis through the 
              hash.
            * Includes the -V option to submit a file to Virus Total. Additionally, the report is shown afer 
              few minutes.
            * Includes two small fixes. 

Version 1.4.5.2:

      This version:

            * Includes two small fixes.

Version 1.4.5.1:

      This version:

            * Includes one small fix. 
            
Version 1.4.5:

      This version:
      
            * Adds the -w option to use malwoverview in Windows systems.
            * Improves and fixes colors when using -b option with black window.  

Version 1.4: 

      This version:

            * Adds the -a option for getting the Hybrid Analysis summary report.
            * Adds the -i option for listing imported and exported functions. Therefore, imported/exported
              function report was decoupled for a separated option.  
                  
Version 1.3: 

      This version:

            * Adds the -p option for public Virus Total API.
            
Version 1.2: 

      This version includes:

            * evaluates a single file (any filetype)
            * shows PE sessions.
            * shows imported functions.
            * shows exported function.
            * extracts overlay.
            * shows AV report from the main players. (any filetype)

Version 1.1: 

      This version:

            * Adds the VT checking feature.


Version 1.0:

      Malwoverview is a tool to perform a first triage of malware samples in a directory and group them 
      according to their import functions (imphash) using colors. This version:

            * Shows the imphash information classified by color. 
            * Checks whether malware samples are packed.  
            * Checks whether malware samples have overlay. 
            * Shows the entropy of the malware samples. 


