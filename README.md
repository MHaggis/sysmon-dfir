# Sysmon DFIR
Sources, configuration and how to detect evil things utilizing Microsoft Sysmon.

# Install Sysmon

To install Sysmon, use the following command:
    Sysmon.exe -i -h MD5,IMPHASH -n
After installation, load the custom configuration file with the following command:
    Sysmon.exe -c sysmon.cfg
Upon installation, Sysmon will begin logging events to the operational event log “C:\Windows\System32\
winevt\Logs\Microsoft-Windows-Sysmon%4Operational.evtx”.

**Sysmon-a.cfg**
http://www.blacklanternsecurity.com/blog/2016/12/11/sysmon-woes-elasticsearch-and-mitres-attack-matrix/

**Sysmon-b.cfg**

https://github.com/crypsisgroup/Splunkmon/edit/master/sysmon.cfg
http://www.crypsisgroup.com/images/site/CG_WhitePaper_Splunkmon_1216.pdf


# Resources
https://www.rsaconference.com/writable/presentations/file_upload/hta-w05-tracking_hackers_on_your_network_with_sysinternals_sysmon.pdf
http://www.incidentresponderblog.com/2016/09/detecting-lateral-movement-using-sysmon.html
http://www.blacklanternsecurity.com/blog/2016/12/11/sysmon-woes-elasticsearch-and-mitres-attack-matrix/
http://www.darkoperator.com/blog/2014/8/8/sysinternals-sysmon
https://github.com/darkoperator/Posh-Sysmon
https://github.com/JamesHabben/sysmon-queries
https://www.crowdstrike.com/blog/sysmon-2/
https://joshuadlewis.blogspot.com/2014/10/advanced-threat-detection-with-sysmon_74.html
https://dfir-blog.com/2015/10/11/protecting-windows-networks-essential-logging/
http://www.crypsisgroup.com/images/site/CG_WhitePaper_Splunkmon_1216.pdf
https://github.com/splunk/TA-microsoft-sysmon
https://github.com/crypsisgroup/Splunkmon
