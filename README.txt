This is a Virtual machine for the tool Spy@Runtime.
The example software used for Demo are - Storage service server software & RabbitMQ software.  
As this tool helps the user to Spy the software application they want, during run time, the user should replace the above two software files with the software application they want to test.  


Instructions to Run the example software, use the terminal- 

1.Use cd Desktop/spy-monitoring

2.To run the server, run-
./run-server.sh

3. In a different terminal, enter into Desktop/spy-monitoring and run- 
sudo ./run-ipcollection-junit.sh config/parameters-test-storageservice.xml storageServer.StorageServerClientViewTest

4. For Model generation, run-
./run-spy-quick.sh -w it.polimi.dei.spy.wrappers.StorageServiceClientViewWrapper storageServerClient.StorageServiceClientView

5. To enable Monitoring facility, run-
./run-monitoring.sh config/monitoring-storageservice.xml storageServerClient.StorageServiceClientGUIToMonitor

--Give inputs as shown in the video, to check for its functionality

6.In the server terminal, terminate the previous run using Cntrl-C and run-
./run-server.sh

7.To inject fault,
Press 1 and enter

8.In a new terminal, enter into Desktop/spy-monitoring and run- 
./run-monitoring.sh config/monitoring-storageservice.xml storageServerClient.StorageServiceClientGUIToMonitor

9.Check for functionality after injecting fault, by given inputs as shown in the video






Reference Links - 
--The paper on Spy@Runtime - http://dl.acm.org/citation.cfm?id=2337430 
--Official tool website - http://www.inf.usi.ch/postdoc/mocci/spy-testing/index.xhtml
--Video of the tool (presented by the authors of the paper)- https://www.youtube.com/watch?v=EqQ7k_UG448&feature=youtu.be 
