# Cloud-Security-Topology
This was an assignment where I was instructed to use Azure Cloud to create a highly available web server for Red Team testing and training. 

<h3><b>Objective:</b></h3> <br>
&#x2022; Set up a resource group and a cloud network using the Azure Portal. <br>
&#x2022; Create a network security group to control access to any resources in your subnet. <br>
&#x2022; Set up four virtual machines inside your cloud network, protect them with your network security group.  <br>
&#x2022; Use one of these machines as a jump box to access your cloud network, and the other machines will be web servers. <br>

<h3><b> Containerization and Configuration </b> </h3> <br>
&#x2022; Jumpbox VM runs Ansible Docker Container. <br>
&#x2022; Ansible playbook is configured to expedite coniguration of the 3 web servers. <br>
&#x2022; Each Web Server VM runs DVWA Docker Container. <br>
&#x2022; A Load balacer is installed in front of the web server VMs. <br>

<h3><b>Network Security Rules </b> </h3> <br>
&#x2022; SSH connection only from my current IP address to the Jump Box. <br>
&#x2022; SSH connection allowed from Ansible to all three web server VMs. <br>
&#x2022; HTTP connection allowed from  current IP address to the load balancer. <br>

<h3><b> Cloud Topology Map </b> </h3> <br>

   ![Kylan Aburto-Pratt Cloud Security](https://user-images.githubusercontent.com/110432400/213011628-e2847d8d-4f1a-4419-9856-5068faf6074f.jpg)
