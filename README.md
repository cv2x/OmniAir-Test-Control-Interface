Work in progress under the OmniAir Application sub working-group of the Technical Working Group
These extensions add a simulation framework, that allows universal injection/simulation of all drives for all regions (China, ETSI-ITS, SAE) 
providing all possible vehicle data, events, lights, motions, accelerations, and any data found in a ETSI CAM, SAE BSM, etc.

Also included in this extension to TCI is the "Use Case Announcement Message" (UCAM) control, and the ASN for the UCAM itself.
UCAM's are not part of OATCI, but can be configured, enabled, disabled, and delivered  over TCI to by the test equipment.   
The UCAM’s themselves are JSON JER encoding of the ASN.1, and sent as UDP, TCP, WSMP, DSMP, ETSI-ITS BTP, or TCI to the recipients.  Over Radio broadcast, they are sent as UDP, WSMP, DSMP for sniffer/loggers, test equipment or RSU’s to capture in test environments.
UCAM’s record when any given “alert” use-case, was triggered, cleared, or preempted by higher priority alert . these alerts are geo-tagged, and named for test equipment or nearby radios to log and note to determine if the vehicle under test performs adequately. 
