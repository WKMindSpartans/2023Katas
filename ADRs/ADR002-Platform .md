# Architectural Decision Record
## Date
9/13/23 

## Title
Platform (Infrastructure)

## Status
Accepted

## Context 
The Road Warrior will be designed with cloud services and infrastructure in mind.

## Decision Drivers
- Need to for systems to scale: The Road Warrior has big user base. That will require infrastructure that can scale quickly and easily.
- Solution Architecture: The solution design has many features that can benefit greatly from managed services that cloud providers offers.

## Decision
Approve the use of Cloud based infrastructure

## Trade-Offs/Mitigations
- Cloud implementations can grow quickly. Care will need to be taken to ensure that costs do not outpace funding for the project.

## Consequences
- Reduced level of management and maintenance
- Reduced initial cost for hardware and software
- Increased ability to elastically match workload
