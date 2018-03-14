1. Login to My webMethods Server as an "Administrator" user.

2. Navigate to Administration --> Integration --> B2B --> Processing Rules.

3. Add 5 processing rules above the "Default Rule" in the below Order.

	Rule Name (No .1): ProcessInboundEDIEnvelop
	"	Choose the Sender Partner Group as "EDIHUBPARTNERS"
	"	Receiver Partner Group as "EDIHUBDIVISION" and Select "X12 Envelope" in the DocumentType
	"	Go To "Action" Tab and Add "Change UserS tatus" to "DONE"
	"	Click "Save"
   [[/Images/Picture33.png|ALT TEXT]] 

	Rule Name (No .2): ProcessInboundEDIGroup
	"	Choose the Sender Partner Group as "EDIHUBPARTNERS"
	"	Receiver Partner Group as "EDIHUBDIVISION" and Select "X12 Envelope"  in the DocumentType
	"	Go To "Action" Tab and Add "Change UserS tatus" to "DONE"
	"	Click "Save"
	[[/Images/Picture34.png|ALT TEXT]]

	Rule Name (No .3): ProcessInboundEDIDocuments
	"	Choose the Sender Partner Group as "EDIHUBPARTNERS"
	"	Receiver Partner Group as "EDIHUBDIVISION" and Select "X12 Envelope"  in the DocumentType
	"	Go To "Action" Tab and Add "Execute Service" and Select the service "SmartEDI.EDI.EDIRecogn:EnterpriseEDIRecogn" 
	"	Also "Change User Status" to DONE
	"	Click "Save"
	[[/Images/Picture35.png|ALT TEXT]]
 
Note: For InboundEDIDocuments, add all the appropriate EDI Documents in the Document Type Section

	Rule Name (No .4): ProcessOutboundEDIEnvelp
	"	Choose the Sender Partner Group as "EDIHUBDIVISION"
	"	Receiver Partner Group as "EDIHUBPARTNERS" and Select "X12 Envelope" in the DocumentType
	"	Go To "Action" Tab and Add "Execute Service" and Select the service "SmartEDI.EDI.EDIEnvelp:EnterpriseEDIEnvelp" 
	"	Also "Change User Status" to DONE.
	"	Click "Save"
	[/Images/Picture36.png|ALT TEXT]]

	Rule Name (No .5): ProcessOutboundEDIGroup
	3.	Choose the Sender Partner Group as "EDIHUBDIVISION"
	4.	Receiver Partner Group as "EDIHUBPARTNERS" and Select "X12 Envelope" in the DocumentType
	5.	Go To "Action" Tab and Add "Change Users status" to "DONE"
	6.	Click "Save"
	[/Images/Picture37.png|ALT TEXT]]
 

