# Architectural Decision Record
## Date
9/13/23 

## Title
Persistent Storage

## Status
Accepted

## Context 


## Decision Drivers
- Need to for systems to scale: The Road Warrior has big user base. That will require infrastructure that can scale quickly and easily.
- Solution Architecture: The solution design has many features that can benefit greatly from managed services that cloud providers offer.

## Decision
Approve the use of Cloud based storage

## Trade-Offs/Mitigations
- Cloud storage can grow quickly. Care will need to be taken to ensure that costs do not outpace funding for the project.

## Consequences
- Reduced level of management and maintenance
- Reduced initial cost for hardware and software
- Increased ability to elastically match workload
