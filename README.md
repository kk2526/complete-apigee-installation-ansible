# Project Name

Custom setup to install ApiGee All-in-One/Single-Region

## Installation

1. Setup the control-server and intall pre-requisites for the nodes 	
    a. cd environment-setup-playbooks/  
    b. Edit resources/credential.yml  
    c. Edit hosts file  
    d. Run setup.yml 
  
  * Copy your license file to ~/.apigee/license.txt  
2. Install Edge Components  
   a. cd apigee-edge-installation-playbooks/  
   b. ansible-galaxy -fr install requirements  
   c. ansible-plabook -i hosts installation.yml
   
   
3. Install Dev-Portal  
   a. cd apigee-devportal-installation-playbooks/  
   b. ansible-galaxy -fr install requirements  
   c. ansible-plabook -i hosts installation.yml

   

## Credits

* Carlos Frias ( https://github.com/carlosfrias  ) 
