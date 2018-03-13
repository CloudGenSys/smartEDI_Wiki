Shell Creation

1.	Login to My webMethods Server as "sysadmin".	

2.  Navigate to "Home".

3.	Go to "Shell Adminstration".

4.	Create a "New Shell".

5.	Name the new shell as "SmartEDI Shell".

6.	Do not modify the Shell section directly, always clone from the parent 'Noodle Shell' as shown below. Use the "Clone from Parent" option to Clone Header, Footer, Left Nav and Right Nav. 
[[/Images/Picture25.png|ALT TEXT]]

7.	Edit SmartEDI Shell Leftnav which will take you to the Properties.

8.	Enter the Application Root as the alias that we created for the parent folder as shown below and check "Show Applications", "Show Navigate" and "Show LHS", click Apply and then Save.
[[/Images/Picture26.png|ALT TEXT]]

9. Navigate to Folders --> System --> Shell Sections and search for "SmartEDI Shell Leftnav". In the properties for the LeftNav, set the permissions to "Everyone view only" and remove the Security Realm.

Shell Rules

1.	Login to My webMethods Server as "sysadmin".

2. Navigate to Folders --> Administrative Folders --> Administration Dashboard --> User Interface --> Manage Shell Rules. 

3. Create Shell Rule "SmartEDI Shell Rule" and paste the condition as

(("SmartEDIRole" matches user.groupMembershipDNs) or ("SmartEDIRole" matches user.roleMembershipDNs)) &&
 ( #{request.requestURI} startsWith "/smartedi" || portalResource isDescendant ("smartedifolder") ||
portalResource isDescendant ("/portlet/smartediprj___ ")) &&
!(user.name matches "sysadmin")

4. Verify that the Rule Evaluation Order shows "SmartEDI Shell Rule" above "My webMethods".
[[/Images/Picture27.png|ALT TEXT]]