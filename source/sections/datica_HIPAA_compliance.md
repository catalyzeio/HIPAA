# Datica HIPAA Compliance

Learn how Datica not only complies with HIPAA, but builds a better, more secure environment to mitigate your risk and help you prove compliance with HIPAA. We did the hard work so you don't have to. And you can inherit a lot of the work that we've done in terms of audits. Our HIPAA compliant API, platform, and data integration service simplify compliance for you. To learn more about our products or to get setup with an account today, check out our [Compliant Cloud](https://datica.com/compliant-cloud) and [Managed Integration](https://datica.com/managed-integration).

In an effort to be transparent, we go into a good amount detail on this page. As a lead in, below is a high level summary our major architecture, our guiding principles, and how it maximizes our security posture.

Need | Datica Approach
--------- | -----------
Encryption  | All data is encrypted in transit, end to end, and at rest. Log data is also encrypted to mitigate risk of ePHI stored in log files.
Minimum Necessary Access | Access controls are always defaulted to no access unless overrided manually.
System Access Tracking | All access requests and changes of access, as well as approvals, are tracked and retained.
PHI Segmentation | All customer data is segmented. Additionally, all platform customers have a dedicated overlay network (subnet) for additional network segmentation.
Monitoring | All network requests, successful and unsuccessful, are logged, along with all system logs. API PHI requests (GET, POST, PUT, DELETE) log the requestor, location, and data changed/viewed. Additionally, alerts are proactively sent based on suspicious activity. OSSEC is used for IDS and file integrity monitoring.
Auditing | All log data is encrypted and unified, enabling secure access to full historical network activity records.
Minimum Risk to Architecture | Secure, encrypted access is the only form of public access enabled to servers. All API access must first pass through Datica firewalls. To gain full access to Datica systems, users must login via 2 factor authentication through VPN, authenticate to the specific system as a regular user, and upgrade privileges on the systems temporarily as needed.
Vulnerability Scanning | All customer and internal networks are scanned regularly for vulnerabilities.
Intrusion Detection | All production systems have intrusion detection software running to proactively detect anomalies.
Backup | All customer data is backed up every 24 hours. Seven (7) days of rolling backups are retained.
Disaster Recovery | Datica has an audited and regularly tested disaster recovery plan. This plan also applies to customers, and they inherit this from us.
Documentation | All documentation (policies and procedures that make up our security and compliance program) is stored and versioned using GitHub, and published [here](https://policy.datica.com).
Risk Management | We proactively perform risk assessments to assure changes to our infrastructure do not expose new risks to ePHI. Risks mitigation is done before changes are pushed to production.
Workforce Training | Despite not having access to the ePHI of our customers, all Datica workforce members undergo HIPAA and security training regularly. Current training is hosted [here](https://training.datica.com/).

See the finer grain details of how we comply with HIPAA below. These are mapped to specific HIPAA rules. There's a lot here but again, we are taking this responsibility on so that our customers don't have to. Controls marked with an (Req) are *Required*. Controls marked with an (A) are *Addressable*. In our environment, controls outlined below are implemented on all infrastructure that processes, stores, transmits or can otherwise gain access to ePHI (electronic protected health information). If have questions, please [email us](mailto:hello@datica.com).
