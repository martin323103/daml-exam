# 🛠️ DamlLeaseAgreement 🛠️ 
DamlLeaseAgreement is a lease agreement management application built in Daml.

### I. Overview 
This project was created by using the `skeleton` template. The project adopts and exemplifies the `proposal-accept` design pattern. 

Tenant can create a LeaseAgreementProposal contract. Owner of the property can either Reject or Approve the proposal. Upon getting rejected, tenant can exercise Revise to re-propose the lease agreement with updated details. Upon getting accpeted, a LeaseAgreement contract is created, which then tenant and owner can renew or cancel the LeaseAgreement or do some checking on the LeaseAgreement.


### II. Workflow
1. tenant creates a LeaseAgreement contract     
2. owner exercises Reject with reason: "Want a higher rent, 22,000 maybe"
3. tenant exercises Revise with an updated rent
4. owner exercises Accept - Lease Agreement contract is created  


### III. Compiling & Testing
To compile and test, run the pre-written script in the `Test.daml` under /daml OR run:
```
$ daml start
```
