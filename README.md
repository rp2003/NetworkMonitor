# NetworkMonitor
Developed a Linux-based Network Monitoring System that tracks real-time metrics for multiple interfaces, including status, data throughput, and error rates. Implemented socket programming for synchronized communication and signal handling for controlled shutdowns.It ensures high resilience and reliability by incorporating signal handling for controlled shutdown via SIGINT, facilitating a smooth termination process and freeing up resources effectively.

Designed to withstand real-world use, the system can automatically reset interfaces that experience downtime, reducing manual intervention and enhancing uptime. During testing, the Network Monitoring System demonstrated its capability for continuous data polling and accurate, real-time metric reporting, making it a reliable tool for network performance analysis.

# Features:

**Multi-interface Monitoring:** Tracks multiple network interfaces simultaneously, capturing essential metrics such as operational status, up/down counts, bytes transmitted/received, and error rates.

**Socket Programming:** Implements synchronous communication between the main network monitor and individual interface monitors, ensuring accurate data exchange and coordination.

**Controlled Shutdown with Signal Handling:** Supports graceful termination using SIGINT handling, ensuring smooth shutdown, resource cleanup, and prevention of data corruption.

**Resilience and Self-healing:** Includes automatic reset functionality for interfaces that go down, enhancing system robustness and uptime.

**Results:** Tested for continuous data polling and real-time statistical reporting, proving its reliability in monitoring network performance with accurate and timely metrics.

**Makefile Automation**
To streamline development, I designed a Makefile that automates the compilation and build processes. Highlights include:

**Selective Debugging:** make debug builds the project with debug flags, allowing me to trace execution effectively.
**Run Automation:** make run launches the network monitor with sudo to access interfaces, saving time during testing.
**Clean-Up Command:** make clean removes compiled objects and executables in seconds, keeping the workspace organized.
