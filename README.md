# aws_identity
# i understood about aws identity and access management(IAM) principle and components 
In AWS, IAM stands for Identity and Access Management.
It’s the service that helps you securely control access to your AWS resources. Think of it as the gatekeeper of AWS: it decides who (users, applications, services) can access what (resources like S3 buckets, EC2 instances, RDS databases) and how they can access them.
Key Concepts in IAM:
Users – Individual accounts for people or applications.
Groups – Collections of users that share permissions (e.g., "Developers" or "Admins").
Roles – Identities with a set of permissions that can be assumed by trusted entities (like EC2 instances or Lambda functions).
Policies – JSON documents that define permissions (what actions are allowed or denied on which resources).

# login to my root user aws-console
# search for IAM
# search for ec2 inside the IAM and click on allowfullaccess
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 15 30 AM" src="https://github.com/user-attachments/assets/487570c2-f865-4d81-a3f7-97ff916b5dfa" />
# Set permission
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 18 25 AM" src="https://github.com/user-attachments/assets/98b71476-ae5c-4620-92dd-a9f9ad9ac190" />
# created policy_for_eric
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 29 13 AM" src="https://github.com/user-attachments/assets/0065a6c0-8c8c-4c9b-bcf9-f2e050f9f4f3" />
# creating user named eric 
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 34 10 AM" src="https://github.com/user-attachments/assets/dc4f571f-9938-4e0c-8003-4b8a8e054e4e" />
# then set permission policies to custom and select the policy_for_eric created earlier
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 35 59 AM" src="https://github.com/user-attachments/assets/94234654-ed6c-4572-8bee-c891314d544d" />
# after reviwing the policy created
# my user Eric was created successfully
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 38 43 AM" src="https://github.com/user-attachments/assets/b3398607-3de9-48c0-9de3-6ed698d363f0" />
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 40 27 AM" src="https://github.com/user-attachments/assets/2a83c836-4ddd-4c5e-9ccf-eb3b0058130c" />
# go user group to create a group called development-team
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 41 49 AM" src="https://github.com/user-attachments/assets/6cefd51b-fc6b-410f-a828-8a9dd1ff79f1" />
# was successfull created
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 42 31 AM" src="https://github.com/user-attachments/assets/1639a78e-7537-4d9c-8250-913a2739becb" />
# went back to user to create another user called Jack
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 45 30 AM" src="https://github.com/user-attachments/assets/177452d7-ae8a-491a-8b9d-9e7111a84e6c" />
# set permission policy to add user to group just created
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 46 15 AM" src="https://github.com/user-attachments/assets/726524ec-8b87-4cc0-8cb5-86302f80fb36" />
# then review and create user
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 47 16 AM" src="https://github.com/user-attachments/assets/faf272c4-9ae2-4b5b-a6ce-d82175a0e68c" />
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 48 16 AM" src="https://github.com/user-attachments/assets/e1b8a679-85ec-4a5c-871e-7852024abf29" />
# created another user called Ade
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 49 02 AM" src="https://github.com/user-attachments/assets/6ea99751-114a-45b8-89ad-ce25fb6c8556" />
# set permission policy and add to group called development-team
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 50 03 AM" src="https://github.com/user-attachments/assets/ad2fa7de-8b1e-4393-857d-47acc7d70487" />
# this are users created
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 51 21 AM" src="https://github.com/user-attachments/assets/196df88b-fe0c-4b66-b624-2dd56c8a5932" />
# i navigate to policies section to craft new policy 
# select EC2 AND S3 
# name the policy development-team-policy
# rewiew the policy created 
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 12 58 56 AM" src="https://github.com/user-attachments/assets/91bafb19-beca-4e67-b3c1-74c1beda9260" />
# the new policy created 
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 1 00 52 AM" src="https://github.com/user-attachments/assets/5f2cb905-6ab3-476b-a16d-0a8f5840e930" />
# development-team-policy created
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 1 01 55 AM" src="https://github.com/user-attachments/assets/863a3ca8-fe4e-48e5-92aa-aa45f0b2f010" />
# navigate to user group and select development-team and click on permission to attach policy
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 1 03 20 AM" src="https://github.com/user-attachments/assets/d50dd3df-1f85-4f59-9d59-14e6305e57df" />
# select custom manage and select the developmet-team-policy created and attach
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 1 04 44 AM" src="https://github.com/user-attachments/assets/6a4122b7-4ae6-4ed1-b073-7dd46db8fcf1" />
<img width="1280" height="800" alt="Screen Shot 2025-09-05 at 1 06 37 AM" src="https://github.com/user-attachments/assets/509d9d69-5e03-4be9-af5b-e18d31112355" />

