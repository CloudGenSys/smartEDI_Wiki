1.	Download and copy the SmartEDIIntegrationServer.zip and SmartEDIMWS.zip files to 
~SAGHome\IntegrationServer\instances\default\packages\WmDeployer\replicate\inbound
2.	Select the Deployer on the Integration Server Administration menu and the Deployer opens up in a new tab.
3.	Select "Import Build" from the Deployer menu and select SmartEDIIntegrationServer.zip.
[[/Images/Picture1.png|ALT TEXT]]
[[/Images/Picture2.png|ALT TEXT]]
4.	After the build import, a project is created by Deployer underneath the list of deployer projects.
[[/Images/Picture3.png|ALT TEXT]]
5.	Click on the Define for the SmartEDI_01252018 project and the deployment set should have all Integration Server packages.
[[/Images/Picture4.png|ALT TEXT]] 
6.	Click on the Map tab and create a new Deployment Map.
[[/Images/Picture5.png|ALT TEXT]] 
7.	Add the target Integration server this build should be deployed to.
[[/Images/Picture6.png|ALT TEXT]] 
8.	Click on the Deploy tab and create a deployment candidate.
[[/Images/Picture7.png|ALT TEXT]]
9.	Simulate the build by clicking on Simulate and Deploy the build after Simulation report looks good.
10.	Repeat steps 1-10 for the SmartEDIMWS.zip build. Ensure to select an MWS as the target server for the Deployer project created by SmartEDIMWS.zip.