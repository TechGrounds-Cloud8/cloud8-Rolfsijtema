Elastic Cloud Compute

WHAT IS EC2

- [ ] Virtual Computing Environment. More than 500 instances
- [ ] Flexibel compute capacity 
- [ ] Launch instances with many different operational systems 
- [ ] Run as many instances as you need
- [ ] Build with: AMI’s : Amazon Machine Images  

PRICING: 
- [ ] On demand instances are the most expensive option, no long therm commitments,  but they’re also the most flexible. Used by: Netflix, Spotify, Prime.
- [ ] 
- [ ] Reserved instances are mostly very cheap,
- [ ] You pay upfront, cheaper than Demand, You can only reserve instances only for 1 or 3 years, they are reliable. . 
- [ ] 
- [ ] Spot instanced 
- [ ] Are the cheapest, you save money,-  but there not always reliable. When others take ur ‘cheaper space in Region: Oregen” you might go to a more expensive region like Frankfurt. 

SECURITY: 

Security Groups.  (Network level)
- [ ] Allow to add rules
- [ ] Anything that is not allowed, is always denied 
- [ ] 1 default rule allows all Outbound traffic. 

NACL: NETWORK ACCES CONTROL LIST 
- [ ] Extra layer of security
- [ ] A NACL has both explicit allow and deny rules, stateless firewalls.
- [ ] You allow rules manually
- [ ] You denied rules manually 

The Assignment
Build wi
1. Choose name for instance
2. Choose AMI (Amazon Machine Image, Information list zodat je instance gebouwd kan worden)
3. Chose type instance. T2  free tiers
4. Choose key pair
5. Choose network and and a securitygroup.  HTTP HTTP
6. Configure Volume 1gb
7. advanced details, termination protection enable. 
8. helemaal onderaan kun je een bash scripts toevoegen aan de user data. Dit zal ge-rund worden bij het starten van de instance
9. click create instance and show status check
10: Click instance open: status check. 


Stateful firewalls are capable of monitoring and detecting states.

Stateless firewalls: only focus on individual packets, using preset rules to filter traffic.


￼


￼
