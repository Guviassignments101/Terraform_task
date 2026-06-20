# Terraform_task
Task Description:  Launch Linux EC2 instances in two regions using a single Terraform file.  Techstacks needs to be used :   AWS EC2 Terraform AWS CLI
multi-ec2-multi-region
|
|-------- main.tf
|-------- providers.tf
|-------- variables.tf
|
|-------- modules/
 |------ ec2/
 |----- main.tf
 |------ variables.tf
 |---
<img width="412" height="567" alt="image" src="https://github.com/user-attachments/assets/7ac5bbbe-5765-434a-ad1a-b07d80055440" />


Step 1: Define Region Map
<img width="1217" height="732" alt="image" src="https://github.com/user-attachments/assets/a1efecb7-1533-4b4b-8f91-eb1e09365c7f" />
Step 2: Configure providers
<img width="1349" height="893" alt="image" src="https://github.com/user-attachments/assets/3d3a7d87-38d2-401a-8974-b9a35c251aa2" />
Step 3: Create Single reusable template
modules/ec2/variables.tf
<img width="1604" height="684" alt="image" src="https://github.com/user-attachments/assets/92f197e7-02be-471d-9f52-447a00ded9ab" />
modules/ec2/main.tf
<img width="1578" height="873" alt="image" src="https://github.com/user-attachments/assets/b7d99680-fe47-4386-902d-bcd3f1e6a9e6" />
modules/ec2/outputs.tf
<img width="1547" height="740" alt="image" src="https://github.com/user-attachments/assets/917726f5-f697-43e2-8afe-8adb3987e75b" />
Step 4: Use Single template multiple times main.tf
<img width="1568" height="854" alt="image" src="https://github.com/user-attachments/assets/49eb80cb-1f43-4228-a716-bede811509e5" />

Step 5 : Final results 2 EC2 instance created in two regions
<img width="1693" height="825" alt="image" src="https://github.com/user-attachments/assets/0bf04f24-98a8-44c3-90c1-1a1f793145c8" />
<img width="1412" height="474" alt="image" src="https://github.com/user-attachments/assets/b1f5349d-e1de-413c-b96d-615f98d9f9f8" />
<img width="1874" height="845" alt="image" src="https://github.com/user-attachments/assets/e8427ace-967a-4cde-accb-70d689e1a9ac" />
<img width="1897" height="827" alt="image" src="https://github.com/user-attachments/assets/378dc58c-94e4-402e-9fe8-71209bb722cf" />







