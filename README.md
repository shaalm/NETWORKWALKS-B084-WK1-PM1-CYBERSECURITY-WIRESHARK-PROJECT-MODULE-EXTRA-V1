Wireshark SOC Labs: Network Traffic Analysis
This repository contains my completed work for the Networkwalks Wireshark SOC Project Module. As part of this practical module, I investigated 6 different network capture (PCAP) scenarios using Wireshark. Each lab consisted of 10 tasks designed to simulate real-world Security Operations Center (SOC) analyst workflows.

🎯 Project Objectives
The goal of these labs was to build practical Wireshark skills by investigating real network traffic. Key areas of focus included:

Threat Hunting: Identifying malicious actors and targets within a network.

Traffic Analysis: Isolating specific protocols and examining packet-level details.

Stream Reassembly: Following TCP streams to reconstruct conversations and find hidden data.

Credential Harvesting: Locating plaintext passwords transmitted over unencrypted protocols (HTTP).

Incident Detection: Recognizing attack patterns like brute-force attempts.

VoIP Analysis: Extracting audio from VoIP calls to investigate social engineering scams.

📊 Lab Summary & Results
Below is a summary of the 6 completed labs and my scores. All 60 tasks were attempted, with a 90% overall average.

Lab	Topic	Key Skills Practiced	Score
Lab 3	Identify the Attacker's IP	Filtering SYN packets, identifying IP scanning/port probing, determining attack types.	100%
Lab 4	Follow TCP Stream	Rebuilding chat sessions, finding chat ports, extracting passwords/text from streams.	90%
Lab 5	Follow TCP Stream, Part 2	Analyzing HTTP streams, finding hidden data in downloads, determining file transfers.	80%
Lab 6	HTTP Plain Text Credentials	Filtering HTTP POST requests, extracting usernames/passwords, identifying login pages.	100%
Lab 7	Catch the Brute Force Attacker	Detecting repeated failed logins, isolating the attacker IP, identifying successful compromise.	80%
Lab 8	Catch the Call Scammer	Analyzing SIP/RTP traffic, replaying VoIP audio, extracting sensitive data from calls.	90%
🛠️ Tools Used
Wireshark: Primary tool for packet capture analysis, filtering, and stream following.

Networkwalks Labs Platform: Browser-based lab environment provided for the project.

📂 Repository Structure (Suggested)
/screenshots: Contains proof of completion for each lab (as seen in the provided images).

/notes: Brief text files or markdown notes detailing the exact filters used (e.g., ip.addr == 192.168.1.1, http.request.method == "POST") and the logic behind finding specific answers.

🔍 Key Takeaways
Wireshark Filtering: Mastered the use of display filters to cut through noise and focus on specific traffic (e.g., tcp.flags.syn == 1).

Protocol Analysis: Gained a deeper understanding of HTTP, TCP, and VoIP protocols and how they look at the packet level.

Security Implications: Reinforced the critical importance of encrypting traffic (HTTPS vs. HTTP) and the dangers of plaintext credential transmission.
