# Splunk Enterprise Deployment Project

## Overview
This project involves deploying and configuring Splunk Enterprise across multiple VMs, set up as follows:
- **Controller (Indexer):** Centralized data receiver and indexer.
- **Agents (Agent1, Agent2, Agent3):** Splunk Universal Forwarder instances for data collection.

## Architecture
Three universal forwarders send data to a single indexer. The setup aims for efficient search, analysis, and visualization of IT infrastructure data.

## Setup Process
### Controller
1. Installed and configured Splunk Enterprise.
2. Extracted additional Splunk add-ons for Linux.
3. Configured `inputs.conf` and started local Splunk web server.
4. Set receiving port to 9997 for data ingestion.

### Agents
1. Installed Splunk Universal Forwarder on each VM.
2. Configured each forwarder to send data to the controller.
3. Set the deploy poll and monitored directories for data transfer.
4. Ensured proper restart and operation of Splunk services.

## Results
- All components effectively log and visualize data in Splunk web interface.
- Real-time data from VMs confirmed functional communication.

## Challenges and Solutions
1. **Controller Not Visible:** Resolved by configuring `splunk-add-on-for-linux`.
2. **Agent Log Transmission Errors:** Reinstalled correct Splunk forwarder versions.

## Skills and Experience Gained
- VM management and Splunk-specific configurations.
- Problem-solving for network and software integration.
- Mastery in Splunk data indexing and visualization.

## Attachments
Include screenshots and PDFs documenting the setup and outcomes.
