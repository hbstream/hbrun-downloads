# StreamCall 1.2.3 Authorization Correction

This correction applies to section 6 of the operations manual included in `StreamCall-Server-1.2.3-Linux-x86_64.tar.gz`. That section incorrectly states that Business Integration includes Endpoint SDK integration. Use the following entitlement scope for delivery and license issuance:

| Authorization | Included rights |
| --- | --- |
| Production Deployment | Private deployment of the official Server, Command Center, and endpoints |
| Business Integration | Production Deployment and the Business API |
| Dispatch Integration | Business Integration and the full Dispatch API |
| Endpoint SDK Integration | Separately agreed and explicitly enabled in the license; may be combined with the above |

Integrating the Endpoint SDK into a customer-owned Windows, Linux, Android, or Web application also requires registration of the customer application and endpoint installation. Downloading the SDK or obtaining Business or Dispatch API rights does not grant Endpoint SDK integration rights.

This correction does not change the 1.2.3 packages, license enforcement, or their existing SHA-256 hashes. Deliver this notice with the 1.2.3 Server package and confirm the actual issued rights during license application.
