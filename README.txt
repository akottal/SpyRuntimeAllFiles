This is a Virtual machine for the tool Spy@Runtime. To learn about the working and functionality of the tool, refer to the paper(link is provided)

Instructions to Run in the terminal- 

--Use cd Desktop/spy-monitoring

--To run the server, run-
./run-server.sh

-- In a different terminal, enter into Desktop/spy-monitoring and run- 
./run-ipcollection-junit.sh config/parameters-test-storageservice.xml storageServer.StorageServerClientViewTest

-- For Model generation, run-
./run-spy-quick.sh -w it.polimi.dei.spy.wrappers.StorageServiceClientViewWrapper storageServerClient.StorageServiceClientView

-- To enable Monitoring facility, run-
./run-monitoring.sh config/monitoring-storageservice.xml storageServerClient.StorageServiceClientGUIToMonitor

--Give inputs as shown in the video, to check for its functionality

--In the server terminal, terminate the previous run using Cntrl-C and run-
./run-server.sh

--To inject fault,
Press 1 and enter

--In a new terminal, enter into Desktop/spy-monitoring and run- 
./run-monitoring.sh config/monitoring-storageservice.xml storageServerClient.StorageServiceClientGUIToMonitor

--Check for functionality after injecting fault, by given inputs as shown in the video






Reference Links - 
--The paper on Spy@Runtime - http://dl.acm.org/citation.cfm?id=2337430 
--Official tool website - http://www.inf.usi.ch/postdoc/mocci/spy-testing/index.xhtml
--Video of the tool (presented by the authors of the paper)- https://www.youtube.com/watch?v=EqQ7k_UG448&feature=youtu.be 
