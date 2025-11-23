# configuration file

## noun

A file that contains Splunk Enterprise and Splunk Cloud Platform settings and configuration information. Also referred to as a .conf file, configuration files are stored in the following locations:

Default files: $SPLUNK_HOME/etc/system/default
Local files: $SPLUNK_HOME/etc/system/local
App files: $SPLUNK_HOME/etc/apps/

To configure Splunk Enterprise, you can modify configuration settings by editing stanzas within copies of the default configuration files in a local directory. To configure Splunk Cloud Platform, you must use Splunk Web since Splunk Cloud Platform users do not have access to the file system of the Splunk Cloud Platform deployment and cannot manually edit .conf files.
