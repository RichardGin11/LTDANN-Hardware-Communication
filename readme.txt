This code will utilize the meshtastic framework to send messages.
Core hardware components are a microprocessor and LoRaWAN antenna with reception and transmission capabilities.


// Pseudocode for the Receiver and Nodes.

Create Node Object Class
	Function for sending messages
	Function for receiving messages

void main() {
	// Create the 4 nodes with send and receive capability
	Create Node1 Object
	Create Node2 Object
	Create Node3 Object
	Create Node4 Object
	
	// Create 4 data files to store timestamp/distance information for each node
	Create distanceNode1
	Create distanceNode2
	Create distanceNode3
	Create distanceNode4
	
	while(true) {
		Node1.send(timestamp)
		Node2.send(timestamp)
		Node3.send(timestamp)
		Node4.send(timestamp)
		
		distanceNode1 = parse( Node1.receive() )
		distanceNode2 = parse( Node2.receive() )
		distanceNode3 = parse( Node3.receive() )
		distanceNode4 = parse( Node4.receive() )
		
		delay(Set amount of time before resending transmissions)
	}
}
