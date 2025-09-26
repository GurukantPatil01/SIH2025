# SIH2025
# Challenges and Enhancements

While your proposed solution is sound, there are a few challenges to consider for a more robust system, as highlighted in the problem statement's detailed description:

* **Accuracy**: GNSS data from mobile phones is inherently less accurate than high-cost systems like LIDAR. The accuracy can vary from a few meters to tens of meters depending on the environment (urban canyons, open sky, etc.). To improve this, you could implement a data-fusion algorithm that combines GNSS data with other on-board sensors like the accelerometer and gyroscope (from the mobile phone's Inertial Measurement Unit or IMU) to create a more stable and accurate position estimate.

* **Real-time Performance**: The latency introduced by the GET requests and the server processing needs to be minimal to ensure a timely collision warning. For a truly real-time system, you might consider using WebSockets instead of repeated GET requests, as they provide a persistent, two-way communication channel between the client and server.

* **Decentralized Communication**: The problem statement also suggests avoiding a centralized server. While a server simplifies the initial development, a more advanced solution would use peer-to-peer (P2P) communication protocols like Bluetooth Low Energy (BLE) or Wi-Fi Direct to share data directly between phones, which would reduce latency and make the system more resilient. This would require each phone to run a more complex, distributed algorithm to determine proximity and potential collisions.

* **Indoor Navigation**: For indoor or challenging environments, GNSS signals are often unavailable. As the problem statement suggests, you would need to augment your system with other technologies. This could involve using a few phones as static "base stations" that communicate with the moving phones. This would essentially create a local positioning system using signals like Wi-Fi or BLE for ranging and trilateration.
