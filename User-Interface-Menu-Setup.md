1.	Go to My WebMethods Applications and select "Fabric Tasks".
[[/Images/Picture12.png|ALT TEXT]]

2.	Click on the context menu and select New --> Page.
[[/Images/Picture13.png|ALT TEXT]]

3.	In the options for the page, enter "SmartEDI" as the folder name and save.

4.	Go to properties of the folder. Check the options "Is Task Folder" and "Is Openable" and add an alias "smartedifolder"  
[[/Images/Picture14.png|ALT TEXT]]

5. Click on Apply.

6.	Create a new folder "EDI Interfaces" underneath the previously created "SmartEDI" Folder.

7.	Go to properties of the "EDI Interfaces" folder and check the "Is Task Folder" and click Apply.

8.	Create another Page "Inbound EDI Setup" under "EDI Interfaces" and in the properties of the "Inbound EDI Setup" page check options "Is Task Folder" and "Is Openable" and click Apply.

9.	Edit the page "Inbound EDI Setup" by selecting edit page in the properties/context menu.

10. "Check View as an Expert", select Properties and go to layout option. Choose "one column" and "Click Ok".
[[/Images/Picture15.png|ALT TEXT]]

11.	On the left "Tools" navigation menu, drag the "Inbound EDI Step 1" Portlet under project "SmarEDIPrj" into to canvas on the right.

12.	Select the Properties of the "Inbound EDI Step" and uncheck "Title Bar" and "Border" and click Apply.
[[/Images/Picture16.png|ALT TEXT]]

13.	Save the changes now for the page "Inbound EDI Setup". The target page should look like shown below.
[[/Images/Picture17.png|ALT TEXT]]

14.	Add another page under "EDI Interfaces" called "Outbound EDI Setup". Repeat steps 9 through 11 but this time drag "Outbound EDI Step 1" Portlet from the SmartEDIPrj. Repeat steps 12 through 13. The target page should look like shown below.
[[/Images/Picture18.png|ALT TEXT]]

