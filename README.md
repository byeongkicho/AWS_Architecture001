# AWS_Architecture001
AWS Architecture001 Design

<Overall>
  1.Multi-AZ, Multi-region for High Availability<br />
  2.Dedicated VPC for Production Environment.<br />
  3.Set AutoScaling to Multi-AZ so able to dynamic scaleout.<br />
  4.Linux 2 Ami userdata to Launch Configuration so install Apache automatically.<br />
  5.ALB is configured to distribute inbound traffic to Web servers set to multi-az.<br />
  6.The web server EC2 sends traffic to the WAS terminal via NLB to communicate with the WAS.<br />
  7.WAS cannot communicate with the outside world because it is on PrivateSubnet, and Tomcat of WAS has set       up NAT to enable access to the external Internet because it needs periodic updates.<br />
  8.All traffic in the VPC can go to the Internet via Internet Gateway.<br />
  9.the ACM-issued public certificate to the https listener of the web server load balancer to provide             security access through SSL (Secure Sockets Layer).<br />
 10.configured VPC and Subnet for Bastionhost separately for secure access, and then Peering is set up to         connect with Production VPC.<br />
 11.Client VPN Endpoint was set to promote secure access when external clients access resources within AWS.<br />
 12.CloudWatch and CloudTrail analyzed the logs so we could receive notifications of the resource's events through SNS.<br />
 13.set the automate the release process using Code Pipeline, CodeCommit, CodeDeploy.<br />

![alt text](https://github.com/taboo32/AWS_Architecture001/blob/main/AWS_Architecture001.png?raw=true)
