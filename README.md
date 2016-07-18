# jboss-eap7-domains-labs
JBoss EAP 7 Domain deployments – Part 1: Setup a simple EAP Domain
This repository is used to track all the configuration changed in the JBoss EAP 7 Labs.

1 Domain Controller on a machine called host0
1 Host Controller on a machine host1 with two EAP instances Server11 and Server12
1 Host Controller on a machine host2 with Three EAP Instances Servers21, Server22 and  Server23
Host0 should be run as the master controller,
Host1 and Host2 are slaves connecting to Host0
  Server11 and Server21 are members of the primary server group ( name=primary-server-group)
  Server12 and Server22 belong  to the secondary server group (name=secondary-server-group)
  Server23 is the only member of the  singleton server group ( name= singleton-server-group)
In real life Machine Host1, Host2 are mostly  in different physical location but for the purpose of this tutorial we are going to simulate them  on the same localhost using a signed EAP 6.4 installation and different configuration folders for each Machine.
