# Site-to-Site VPN Lab — Project Tracker

## Phase 0 — Planning & GitHub Setup
- [x] Create GitHub repository
- [x] Create initial README
- [ ] Finalize network architecture and addressing
- [ ] Prepare Hyper-V environment

## Phase 1 — Hyper-V Networking
- [ ] Review existing Hyper-V virtual switches
- [ ] Create Site A LAN virtual switch
- [ ] Create Site B LAN virtual switch
- [ ] Create WAN/transit virtual switch
- [ ] Verify virtual network configuration

## Phase 2 — VPN Endpoints
- [ ] Obtain pfSense installation media
- [ ] Create pfSense-A VM
- [ ] Configure Site A WAN and LAN interfaces
- [ ] Create pfSense-B VM
- [ ] Configure Site B WAN and LAN interfaces
- [ ] Verify connectivity between VPN endpoints

## Phase 3 — IPsec Site-to-Site VPN
- [ ] Configure Site A IPsec settings
- [ ] Configure Site B IPsec settings
- [ ] Configure Phase 1 parameters
- [ ] Configure Phase 2 parameters
- [ ] Configure required firewall rules
- [ ] Establish IPsec tunnel

## Phase 4 — Validation & Troubleshooting
- [ ] Verify IPsec tunnel status
- [ ] Verify security associations
- [ ] Test traffic across the VPN
- [ ] Capture validation evidence
- [ ] Introduce one intentional configuration failure
- [ ] Diagnose and resolve the failure
- [ ] Document troubleshooting results

## Phase 5 — Portfolio Documentation
- [ ] Create final network architecture diagram
- [ ] Add relevant screenshots
- [ ] Document configuration and validation
- [ ] Document troubleshooting scenario
- [ ] Add lessons learned
- [ ] Review README for accuracy
- [ ] Mark project complete

---

## Completion Criteria

The project is complete when two isolated private networks are connected through a functioning IPsec site-to-site VPN, connectivity has been validated, one troubleshooting scenario has been documented, and the final architecture and results have been published in this repository.
