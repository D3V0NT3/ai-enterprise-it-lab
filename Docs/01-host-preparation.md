# 01 — Host Preparation

## Objective

Check that the host can support the initial virtual lab and choose
a suitable location for virtual machines and installation media.

## Readiness Checks

| Item | Observed result |
| --- | --- |
| CPU cores | 6 |
| Logical processors | 12 |
| Hardware virtualisation | Enabled |
| C: available storage | 7.16 GB |
| E: available storage | 412 GB |

Storage figures were recorded at the time of the checks.

## Storage Decision

I selected E: for the lab because it had sufficient available capacity.
The system drive had limited free space.

Planned locations:

- Virtual machines: E:\Labs\Northstar-v2\VMs
- Installation media: E:\Labs\Northstar-v2\ISOs
- Local evidence: E:\Labs\Northstar-v2\Evidence

## Preparation Checklist

- [x] Verify hardware virtualisation is enabled.
- [x] Check available storage.
- [x] Select the lab storage drive.
- [x] Create the lab folders.
- [x] Set the VirtualBox default machine folder.
- [ ] Confirm installation media is available.

## Skills Practised

Host readiness checks, capacity planning and technical documentation.

## Next Step

Configure the virtual lab network and create the Windows Server VM.