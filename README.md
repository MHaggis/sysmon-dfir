# Sysmon DFIR
Sources, configuration and how to detect evil things utilizing Microsoft Sysmon.

# Install Sysmon

To install Sysmon, use the following command:

    Sysmon.exe -i -h MD5,IMPHASH -n

After installation, load the custom configuration file with the following command:

    Sysmon.exe -c sysmon.cfg

Upon installation, Sysmon will begin logging events to the operational event log “C:\Windows\System32\ winevt\Logs\Microsoft-Windows-Sysmon%4Operational.evtx”.

### Install ###
Run with administrator rights
~~~~
sysmon.exe -accepteula -i sysmonconfig-export.xml
~~~~

### Update existing configuration ###
Run with administrator rights

sysmon.exe -c sysmonconfig-export.xml

### Configs ###

**Sysmon-a.cfg**

http://www.blacklanternsecurity.com/blog/2016/12/11/sysmon-woes-elasticsearch-and-mitres-attack-matrix/

**Sysmon-b.cfg**

https://github.com/crypsisgroup/Splunkmon/edit/master/sysmon.cfg

http://www.crypsisgroup.com/images/site/CG_WhitePaper_Splunkmon_1216.pdf

**Sysmon-c.cfg**

https://decentsecurity.com/enterprise/#/sysmon-enterprise-configuration/

**@SwiftOnSecurity Updated config**

https://github.com/SwiftOnSecurity/sysmon-config


**Sysmon-d.cfg**

http://909research.com/sysmon-the-best-free-windows-monitoring-tool-you-arent-using/

**Sysmon-e.cfg**

https://github.com/Prevenity/sysmon

(Translated comments to english)

**Sysmon_config.xml**

https://www.malwarearchaeology.com/logging/

**Additional configs**

Configs are updated frequently

Server Config: https://gist.github.com/Neo23x0/a4b4af9481e01e749409

Client config: https://gist.github.com/Neo23x0/f56bea38d95040b70cf5


# Resources

http://security-research.dyndns.org/pub/slides/BotConf/2016/Botconf-2016_Tom-Ueltschi_Sysmon.pdf

[Advanced Incident Detection and Threat Hunting using Sysmon and Splunk - Tom Ueltschi](https://youtu.be/vv_VXntQTpE)

https://securitylogsdotorg.files.wordpress.com/2017/01/sysmon-2017-16-1.pdf

http://www.paul-sec.com/client-monitoring.html

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
