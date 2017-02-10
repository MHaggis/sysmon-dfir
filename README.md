# Sysmon DFIR
Sources, configuration and how to detect evil things utilizing Microsoft Sysmon.

# Install Sysmon

To install Sysmon, use the following command:

    Sysmon.exe -i -h MD5,IMPHASH -n -l

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

**@SwiftOnSecurity config**

Recommended.

Config will assist with bringing you up to speed in relation to critical process monitoring, network utilization, and so on. Note that the concept is to not log everything, but the most important items.

https://github.com/SwiftOnSecurity/sysmon-config

**Sysmon_config.xml**

Solid, detailed config. Probably one of the best ones out there in relation to completeness.

[MalwareArchaeology](https://www.malwarearchaeology.com/logging/)

**Sysmon-a.cfg**

Basic config that will monitor critical Windows process execution. Very basic, but a good config to get used to sysmon and how things operate.

[Blog post by blacklanternsecurity](http://www.blacklanternsecurity.com/blog/2016/12/11/sysmon-woes-elasticsearch-and-mitres-attack-matrix/)

**Sysmon-b.cfg**

Crypsis Group published config and PDF. Fairly detailed list of excludes that should assist with understanding how they work and get a configuration started.

[Crypsis Group Config](https://github.com/crypsisgroup/Splunkmon/edit/master/sysmon.cfg)

[Crypsis Group PDF](http://www.crypsisgroup.com/images/site/CG_WhitePaper_Splunkmon_1216.pdf)

**Sysmon-c.cfg**

Great configuration to understand excludes and contains.

[Decent Security Config](https://decentsecurity.com/enterprise/#/sysmon-enterprise-configuration/)

**Sysmon-d.cfg**

Solid blog post related to getting started with Sysmon. Config is nicely laid out and easy to understand.

[909Research Blog](http://909research.com/sysmon-the-best-free-windows-monitoring-tool-you-arent-using/)

**Sysmon-e.cfg**

Config is specific but it provides a good foundation for capturing a lot of specific data.

https://github.com/Prevenity/sysmon

(Translated comments to english)


**Additional configs**

Configs are updated frequently

Server Config: https://gist.github.com/Neo23x0/a4b4af9481e01e749409

Client config: https://gist.github.com/Neo23x0/f56bea38d95040b70cf5


# Resources

[Advanced Incident Detection and Threat Hunting using Sysmon and Splunk Video - Tom Ueltschi](https://youtu.be/vv_VXntQTpE)

[Advanced Incident Detection and Threat Hunting using Sysmon and Splunk Slides - Tom Ueltschi](http://security-research.dyndns.org/pub/slides/BotConf/2016/Botconf-2016_Tom-Ueltschi_Sysmon.pdf)

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
