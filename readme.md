# Steps to creating a VPC

### Guide Reference

- This guide follows instructions from acloudguru.com **Solutions Architect Associate course**.
    - Chapter 9 => VPCs
        - Lab => Create a Basic VPC and Associated Components in AWS

![Diagram of VPC](assets/basic-vpc-img.png)

### Steps to Follow

#### Create VPC

- [ ] Login to AWS Account

- [ ] Head to VPC and select Your **VPCs** from the left menu bar.
    - [ ] Click on **Create VPC** button
    - [ ] Fill in Name tag (Optional)
    - [ ] Fill in IPv4 CIDR Block
        - [ ] Choose IPv6 CIDR Block (Optional)
    - [ ] Click create button

#### Create Internet Gateway

- [ ] Click **Create Internet Gateway** button.

- [ ] Fill in Name Tag => try to be **specific**
    - [ ] Add more tags if necessary (Optional)
    - [ ] Click **Create Internet Gateway** button

- [ ] Attach newly created Internet Gateway to VPC through the
      **Actions** button on the top right, click on **Attach to VPC**
      from the drop down menu
    - [ ] Select the VPC you want to attach to from the drop down menu
    - [ ] Click **Attach Internet Gateway** button

#### Create Subnets

- [ ] Click **Subnets** from the left side menu under Virtual Private Cloud

- [ ] Click on **Create subnet** button
    1) Create Public subnet first
    2) Select the vpc your creating the subnet in from the drop down menu
       under **VPC ID**
       - Associated VPC CIDRs will populate underneath

     3) Under Subnet subnet settings
        3.1) Select the **First** availability zone
        3.2) Fill in IPv4 CIDR block
             - e.g. => 172.16**.1.**0/24
             - e.g. => 10.0**.1.**0/24
        3.3) Fill in Name tag, be specific about what subnet you're creating
              e.g. => <IPv4 CIDR block> - <AZ name> => 172.16.1.0 - us-east-1**a**
        3.4) Click **Create subnet** button

- [ ] Repeat the steps above till you reach 3.1
    3.1) Select the **Second** availability zone
    3.2) Fill in IPv4 CIDR block
        e.g. => 172.16**.2.**0/24
        e.g. => 10.0**.2.**0/24
    3.3) Fill in Name tag, be specific about what subnet you're creating
        e.g. => <IPv4 CIDR block> - <AZ name> => 172.16.2.0 - us-east-1**b**
    3.4) Click **Create subnet** button



