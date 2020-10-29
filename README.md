

Create stack:
```
./create.sh demo-network-stack network.yml network-parameters.json
./create.sh demo-server-stack servers.yml server-parameters.json
```

Update stack:
```
./update.sh demo-network-stack network.yml network-parameters.json
./update.sh demo-server-stack servers.yml server-parameters.json
```

Delete stack:
```
aws cloudformation delete-stack --stack-name demo-network-stack
aws cloudformation delete-stack --stack-name demo-server-stack
```

Note:
first create network, then servers
first delete servers, then network


# Sources:

#### Used code from the course example repo:
https://github.com/udacity/nd9991-c2-Infrastructure-as-Code-v1-Exercises_Solution
https://github.com/udacity/nd9991-c2-Infrastructure-as-Code-v1

#### Roles and Policies
https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-iam-role.html
https://knowledge.udacity.com/questions/292492
https://www.bogotobogo.com/DevOps/AWS/aws-creating-IAM-Roles-and-associating-them-with-EC2-Instances-in-CloudFormation.php
https://knowledge.udacity.com/questions/309582

#### used these to add instance profile to my EC2 server 
https://knowledge.udacity.com/questions/299818
https://knowledge.udacity.com/questions/311694
https://www.bogotobogo.com/DevOps/AWS/aws-creating-IAM-Roles-and-associating-them-with-EC2-Instances-in-CloudFormation.php
https://docs.amazonaws.cn/en_us/AWSCloudFormation/latest/UserGuide/aws-properties-ec2-instance.html
https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/iam-roles-for-amazon-ec2.html
https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/intrinsic-function-reference-ref.html

#### additional sources:
https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-cli-deleting-stack.html
https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/outputs-section-structure.html
https://classroom.udacity.com/nanodegrees/nd9991/parts/78ebd463-628c-4f6e-8802-f7a344f9cf55/modules/1fd045ed-5a01-42e9-9469-3695e2ac95db/lessons/9e4b346b-a0ce-4bfd-92e9-4f7412682240/concepts/ae4490fe-9cba-4bc7-b682-313dd2322f0e
plus git commands generated during github repo creation



Notes about pushing changes into repo:
```
echo "# AWS_CloudFormation_IaaS_demo_project" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/tristcoil/AWS_CloudFormation_IaaS_demo_project.git
git push -u origin main
```





