Roles

1.	Login to My webMethods Server as "sysadmin".	

2.  Navigate to Folder --> Administrative Folders --> Directory --> Roles and Add a new Role "SmartEDIRole.
[[/Images/Picture19.png|ALT TEXT]]

3.  Go back to Folder --> Administrative Folders --> Directory --> Roles and edit the Members. Add "SmartEDIRole" to it.

4.	Click "Save" to apply changes.


Permissions Management

1. Login to My webMethods Server as "sysadmin".	

2. Navigate to Home --> Permissions Management.

3. Select My WebMethods Applications and Click "Next".
[[/Images/Picture20.png|ALT TEXT]]

4. Search and add the role "SmartEDIRole".
[[/Images/Picture21.png|ALT TEXT]]

5. Edit the Permissions and grant Permissions for all available options in "SmartEDI" Module.
[[/Images/Picture22.png|ALT TEXT]]

6. Click "OK" to save changes.

Menu Permissions

1. Login to My webMethods Server as "sysadmin".

2. Navigate to Folders --> My webMethods Applications --> Fabric Tasks -->SmartEDI -->EDI Interfaces > Inbound EDI Setup  

3. On the context menu/ properties, click on "Permissions" and Remove the Security Realm if any.

4. Go to permissions and search for "SmartEDIRole" in Roles and click "Add".
 
5. Grant All and click "OK".
[[/Images/Picture23.png|ALT TEXT]]
 
6. Make sure you apply the changes to the Children by selecting "Apply to Children".
[[/Images/Picture24.png|ALT TEXT]] 

7.	Repeat the above steps for the page "Outbound EDI Setup".

