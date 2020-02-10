<B>Nagios</B>



<B>Why we need?</B>

1, failure of CI/CD Pipelines<BR>
2, We can't effort any downtime(when your application in the production stage)<BR>
3, Tackle the issue before the incident happen<BR>



<B>What's continuous monitoring</B>

1, tackle the issue before the failure happen<BR>
2, monitor the service on real time and continuously<BR>
Phases(standard by NIST):<BR>
Define -> Establish -> Implement -> Analysis -> Respond -> review and Update -> Defend<BR>
Patriot step:<BR>
1, Continuous Discovery(monitor all the service running)<BR>
2, Assessment the service (compare the information stage)<BR>
3, Continuous Audit (review all the configuration correct or not)<BR>
4, Continuous Patching (review the patching update)<BR>
5, Continuous Reporting (Report all the scanning result)<BR>

Continuous Monitoring Tools:<BR>
there're a lot of things, but Nagios is much more better<BR>



<B>What's Nigous?</B>

Monitors the entire IT infrastructure to ensure systems, application and service running properly.<BR>
Nagios Server -> Hosts/Servers -> Web Interface/SMS/Email<BR>
Benefit:<BR>

- Easy Writing Plugins
- Monitors BP and IT infrastructure with a Single Pass
- Issues can be Fixed Automatically
- Support for implementing redundant monitoring hosts



<B>Nagios Architecture</B>

The Nagios Process will send the message to Nagios UI and the plugins will monitor all the service that we need<BR>

Mostly, the Nagios will monitor all the process, and send the data to the UI, it can monitor the localhost too
The Nagios will using the check_nrpe to the remote process(NRPE)<BR>
then, the NRPE will check everything on the target machine, and replace the information to the original tools<BR>