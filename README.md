<B>Nagios</B>



<B>Why we need?</B>
1, failure of CI/CD Pipelines
2, We can't effort any downtime(when your application in the production stage)
3, Tackle the issue before the incident happen



<B>What's continuous monitoring</B>
1, tackle the issue before the failure happen
2, monitor the service on real time and continuously
Phases(standard by NIST):
Define -> Establish -> Implement -> Analysis -> Respond -> review and Update -> Defind
Patriot step:
1, Continuous Discovery(monitor all the service running)
2, Assessment the service (compare the information stage)
3, Continuous Audit (review all the configuration correct or not)
4, Continous Patching (review the patching update)
5, Continous Reporting (Report all the scanning result)

Continous Monitoring Tools:
there're a lot of things, but Nagios is much more better



<B>What's Nigous?</B>
Monitors the entire IT infrastructure to ensure systems, application and service running properly.
Nagios Server -> Hosts/Servers -> Web Interface/SMS/Email
Benefit:

- Easy Writing Plugins
- Monitors BP and IT infrastructure with a Single Pass
- Issues can be Fixed Automatically
- Support for implementing redundant monitoring hosts



<B>Nagios Architecture</B>
The Nagios Process will send the message to Nagios UI and the plugins will monitor all the service that we need

Mostly, the Nagios will monitor all the process, and send the data to the UI, it can monitor the localhost too
The Nagios will using the check_nrpe to the remote process(NRPE)
then, the NRPE will check everything on the target machine, and replace the information to the original tools