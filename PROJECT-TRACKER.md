# Site-to-Site VPN Lab — Project Tracker

## Phase 0 — Planning & GitHub Setup
- [x] Create GitHub repository
- [x] Create initial README
- [x] Finalize network architecture and addressing
- [x] Prepare Hyper-V environment
- [x] Create initial network architecture diagram
      
## Phase 1 — Hyper-V Networking
- [x] Review existing Hyper-V virtual switches
- [x] Create Site A LAN virtual switch
- [x] Create Site B LAN virtual switch
- [x] Create WAN/transit virtual switch
- [x] Verify virtual network configuration

## Phase 2 — VPN Endpoints
- [x] Obtain pfSense installation media
- [x] Create pfSense-A VM
- [x] Configure Site A WAN and LAN interfaces
- [x] Create pfSense-B VM
- [x] Configure Site B WAN and LAN interfaces
- [x] Verify pfSense endpoint configuration

## Phase 3 — IPsec Site-to-Site VPN
- [x] Configure Site A IPsec settings
- [x] Configure Site B IPsec settings
- [x] Configure Phase 1 parameters
- [x] Configure Phase 2 parameters
- [x] Configure required firewall rules
- [x] Establish IPsec tunnel

## Phase 4 — Validation & Troubleshooting
- [x] Verify IPsec tunnel status
- [x] Verify security associations
- [x] Test traffic across the VPN
- [x] Capture validation evidence
- [x] Introduce one intentional configuration failure
- [x] Diagnose and resolve the failure
- [x] Document troubleshooting results

### Troubleshooting Exercise

**Intentional failure:**  
Changed the Site B Phase 2 encryption proposal from AES-256 to AES-GCM-128 while leaving Site A configured for AES-256 only.

**Observed behavior:**  
Phase 1 (IKE_SA) established successfully, but Phase 2 (CHILD_SA) failed to establish.

**Diagnostic evidence:**  
The pfSense IPsec log reported:
`failed to establish CHILD_SA, keeping IKE_SA`

**Root cause:**  
The Phase 2 encryption proposals on the two VPN endpoints did not match.

**Corrective action:**  
Restored AES-256 as the Phase 2 encryption algorithm on Site B, applied the configuration, and re-established the IPsec tunnel.

**Final validation:**  
Phase 1 and Phase 2 successfully re-established, and a Site B → Site A ping completed with 0% packet loss.

## Phase 5 — Portfolio Documentation
- [x] Create final network architecture diagram
- [x] Add relevant screenshots
- [x] Document configuration and validation
- [x] Document troubleshooting scenario
- [x] Add lessons learned
- [x] Review README for accuracy
- [x] Mark project complete

---

## Completion Criteria

The project is complete when two isolated private networks are connected through a functioning IPsec site-to-site VPN, connectivity has been validated, one troubleshooting scenario has been documented, and the final architecture and results have been published in this repository.
