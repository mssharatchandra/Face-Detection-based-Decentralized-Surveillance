## Face-Detection-based-Decentralized-Surveillance![1](https://user-images.githubusercontent.com/63927839/178406067-92e37c87-9d0c-4cc4-b297-67625af04beb.png)

#The system was designed to support a dual backend, one of the Ethereum 
Blockchain and the other of Cloud Database in an attempt of being failure-proof. 
Initially, the person's face is captured and the face recognition model recognizes the 
person if he is already a member of the community as shown in steps 1 and 2 in 
Figure 3.1. The image is uploaded to the IPFS and then the hash is received as shown 
in steps 3 and 4. The recognized details of the person, the timestamp, and the IPFS 
hash are put on the blockchain by running the Smart Contract, indicated by steps 5 
and 6. The ledger is visible to the community members from the front-end application 
powered by React JS as seen in step 12.
#
Simultaneously, the cloud backend also utilizes the hash returned by step 4 to 
trigger the AWS Lambda Function of writing the details and timestamp in the AWS 
Relational Database(MySQL) as shown in steps 9 and step 10. This RDS is designed 
to be highly redundant and protects all the information securely and reliably. The 
following information is then viewable by the community as shown in steps 11 and 
step 12.
#
In case of attempted intrusion, the Raspberry Pi will ring the buzzer connected to it 
to alert the community, send a notification to all the stakeholders, and securely 
appends the intruder details on both Blockchain and Cloud Backends. Hence, this 
architecture is entirely automated and immutable, boosting the trust and transparency 
associated with the proposed solution.
