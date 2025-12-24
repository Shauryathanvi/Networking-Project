# Networking Project

This repository documents and stores the artefacts for a proposed multi-site network redesign for FinTec Inc. The materials include the written report, the original assignment brief, and the Cisco Packet Tracer topology used to validate the design.

## Repository contents
- `Networking.docx`: Detailed routing and switching report describing the proposed network, configuration steps, and validation outputs for each site.
- `Problem document.docx`: Assignment brief outlining FinTec Inc.'s networking needs and constraints.
- `Network.pkt`: Cisco Packet Tracer project file containing the configured topology, devices, and tests referenced in the report.

## Network design highlights
- Four sites (London, Liverpool, Leicester, and Leeds) interconnected with OSPF for dynamic routing, with static routes configured as a fallback in case OSPF fails.
- Per-site VLAN segmentation with three VLANs—Finance (30), Executive (40), and Employees (50)—to separate traffic and enforce least-privilege access.
- Router-on-a-stick on each site router to provide inter-VLAN routing, paired with DHCP services at every site so end devices receive addresses automatically.
- Access control lists limit internet access to the London site while blocking outbound traffic attempts from other sites.
- Security posture includes SSH-only device management, encrypted system passwords, and disabled unused switch ports to harden the infrastructure.

## Usage
1. Open `Network.pkt` in Cisco Packet Tracer to explore the topology, device configurations, and validation tests.
2. Review `Networking.docx` for the step-by-step configurations, IP addressing plan, and testing evidence aligned with the topology.
3. Consult `Problem document.docx` to understand the original requirements and how the design addresses them.
