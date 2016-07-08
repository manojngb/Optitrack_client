# Optitrack_client 

Simple python Optitrack client - NESL

Prints Frame number, position and rotation of rigid body

Assumption: 
1. Client/Server PC are different.
2. Rigid body is already defined in Motive PC.

No installation of any package required. 
Just change the following  in NatNetClient according to the LAN and motive configuration

        # Change this value to the IP address of the NatNet server.
        self.serverIPAddress = "172.17.5.14"

        # This should match the multicast address listed in Motive's streaming settings.
        self.multicastAddress = "224.0.0.0"

        # NatNet Command channel
        self.commandPort = 1510
        
        # NatNet Data channel     
        self.dataPort = 1511
        
Source: NatNet SDK (Optitrack)
