A simulation-based project that demonstrates how UPI payments can work without active internet connectivity using a mesh networking approach. Transactions are propagated across nearby devices and completed once a node regains internet access.
Features.
Offline Payment Creation
Users can initiate UPI transactions even without internet.
Mesh Gossip Protocol
Transactions are passed device-to-device using a simulated peer network.
 Bridge Node Sync
When any node gets internet, it syncs the transaction with the backend.
 Distributed System Simulation
Demonstrates real-world concepts like fault tolerance and delayed consistency.
 Interactive Dashboard UI
Simple interface to simulate and visualize the flow of transactions.
Tech Stack
Backend: Java, Spring Boot
Frontend: HTML, CSS, JavaScript (Thymeleaf)
Build Tool: Maven
Architecture: REST APIs + Mesh Simulation Logic
How It Works
Create Payment (Offline)
User enters sender, receiver, amount, and PIN.
Inject into Mesh
Transaction is stored as a packet in a simulated mesh network.
Gossip Rounds
Packets are shared between nodes (devices), mimicking offline transfer (like Bluetooth).
Bridge Node Activation
When a node gains internet access, it forwards the transaction to the backend.
Transaction Completion
Payment is processed and marked successful.
Future Improvements
 Mobile-based peer-to-peer communication (Bluetooth/WiFi Direct)
 End-to-end encryption
 Real-time visualization of node communication
 Deployment with live demo
