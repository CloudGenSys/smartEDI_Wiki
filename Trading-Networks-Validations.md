Trading Partner Agreements

1. Login to My webMethods Server as an "Administrator" user. In the left navigation, go to Trading Partner Agreement under B2B.

2. If Partner doesn't expect an FA(Functional Acknowledgement),turn Off "FA Auto Generation flag" in EDITPA. You may want to turn FA off during development.
[[/Images/Picture38.png|ALT TEXT]] 

3. Smart EDI Uses Custom TPA "ENTEDITPA" to hold interface specific information that is used for Alerts and Logging. Fill in the interface and alerts specific details.
[[/Images/Picture39.png|ALT TEXT]] 

[[/Images/Picture40.png|ALT TEXT]] 

4. When a new transaction is setup with SmartEDI, a main EDI handler stub service is generated. This service had pre-populated services with a save and restore pipeline to help with debug. Adjust the fileName variable in debug branch of the main EDI handler. Also, ensure to remove this before moving to non-Development environment.
[[/Images/Picture41.png|ALT TEXT]] 

5. When a new transaction is setup with SmartEDI, an ENTEDITPA is created one for each sender/receiver pair. Setup the EDI qualifiers, values and all the Outbound parms as required.
[[/Images/Picture42.png|ALT TEXT]] 