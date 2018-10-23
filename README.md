# AWS_VPC_BASTION_GUIDE_HW

**By : Erica P da Silva Correia**

#### Description :

Write a Readme file with instructions as to how to create and run a machine on AWS.

-----

#### Tech Used :
**AWS**

-----
##### how to download :


1. go to the github page [**https://github.com/EricaDaSilvaCorreia**](https://github.com/EricaDaSilvaCorreia)
2. Click repositories and select the repository [**Sparta_AWS_Instructions**](https://github.com/EricaDaSilvaCorreia/Sparta_AWS_Instructions)
3. Click 'Clone or Download'
4. Choose between **Open in Desktop**, **Download ZIP**, **Clone with SSH**, **Clone with HTTPs**

-----
##### how to make and run an AMI :

1. Log into your AWS account 
2. Once on the Dashboard page, go to your navbar and click on services
3. In the services section select EC2 (under Compute on the to left-hand-side).
4. Once in EC2, click on **Launch Instance** 
5. **Step 1:** Select your desired AMI (Amazon Machine Image) ensuring you choose the free tiers.
6. **Step 2:** Select your desired Instance Type.
7. **Step 3:** Configure Insance Details as Required.
8. **Step 4:** Add Storage and adujst storage specifications as required.
9. **Step 5:** Add tags to your machine (for example Name)
10.  **Step 6:** Configure Security Specifications (ssh)
11. Select under type select SSH and under source in the dropdown menu and select My IP.
12. Select exiting group (Wizard 1)
13. Once you're done with these steps click **Review and Launch**
14.  Review all your details and make sure everything is correct.
15. Once Reviewed click **Launch** at the bottom right and this will show you a pop-up to select a ssh key.
16. Select the relevant key.
17. Once this is done, your machine will Launch on AWS.
18. Ask your supervisor for the private key.
19. Open a Terminal on your computer.
20. **Your key must not be publicly viewable for SSH to work.** 
21.  If Necessary use the following command : chmod 400 PrivateKeyName.pem
22. Connect to your instance using its Public DNS: ssh -i "PrivateKeyName.pem" machine@DNS

-----
##### how to make a VPC and launch instance in that VPC:

1. Log into your AWS account.
2. Once on the Dashboard page, go to your navbar and click on Services.
3. In the services section select VPC (under Network & Content Delivery on the bottom left-hand-side of the menu that appears).
4. Once on the VPC Dashboard click on **Launch Wizard**
5. Click on **VPC with Public and Private Subnets** and then choose Select. **Note : this allows you to have both a private and a public subnet inside your VPC**
6. Name your VPC and Subnets to make them easier to recognise later on.
7. In **Specify the details of your NAT gateway**, enter the allocation ID for an Elastic IP address in your account.
8. Check the rest of the default values to see if there is anything else you need to customise. For the purpose of this Readme we will keep the other defaults as they are.
9. Once you've triple checked your details, click on create VPC
10. To launch an instance into your VPC Create an AMI with the following steps :
	1. Once on the Dashboard page, go to your navbar and click on services
	2. In the services section select EC2 (under Compute on the to left-hand-side).
	3. Once in EC2, click on **Launch Instance** 
	4. **Step 1:** Select your desired AMI (Amazon Machine Image) ensuring you choose the free tiers.
	5. **Step 2:** Select your desired Instance Type.
11. **Step 3:** Configure Insance Details : under Network, select the VPC that you just created and then select a subnet. **Note : depending on the function of your AMI, choose to put it in a private or public server.**
12. Assign a public IPv4 address and ensure that you choose Enable from the Auto-assign Public IP list.
13. **Step 4:** Add Storage and adujst storage specifications as required.
14. **Step 5:** Add tags to your machine (for example Name)
15.  **Step 6:** Configure Security Specifications (ssh)
16. Select under type select SSH and under source in the dropdown menu and select My IP.
17. Select exiting group (Wizard 1)
18. Once you're done with these steps click **Review and Launch**
19.  Review all your details and make sure everything is correct.
20. Once Reviewed click **Launch** at the bottom right and this will show you a pop-up to select a ssh key.
21. Select the relevant key.
22. Once this is done, your machine will Launch on AWS.
23. You have now created and implemented your AMI into your VPC with their respective subnet. 


-----


##### Challenges :

Overall, there weren't any challenges with this homework. 

-----

##### Take-Aways :

All in all I think today was very interesting. I enjoyed learning about Jenkins and AWS and I'm looking forward to tomorrow!

I give it a 8/10.

-----
