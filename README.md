system-log-analyzer
===================

This sample explains how you can do the LogEvent analytics real time as well as batch processing using WSO2 BAM+CEP

=========================Configure BAM CEP ============================
Download WSO2 BAM 2.4.0
Add mysql connector jar to BAM_HOME/repository/component/libs
Enable email transport in axis2_client.xml (according to your configs)
Download and extract CEP artifacts and add them to WSO2_BAM_2.4.0/repository/component/deployment folder
Start BAM

======================Configure AS => To send Logs to BAM/CEP=========================
Download WSO2 AS
Add LogEvent appender to root logger (see log4j.properties)
Start AS

**Observations

LogEvents will be published to BAM
Trigger a mail if an ERROR occurs
Will be able to see gadgets in gadget dashboard
