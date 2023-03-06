nslookup (stands for “Name Server Lookup”) is a useful command for getting information from the DNS server. It is a network administration tool for querying the Domain Name System (DNS) to obtain domain name or IP address mapping or any other specific DNS record. It is also used to troubleshoot DNS-related problems.

`nslookup google.com`

![[Pasted image 20221130172629.png]]


`nslookup 142.250.77.174`
For the  reverse DNS look-up by providing the IP Address as an argument to nslookup.
![[Pasted image 20221130173007.png]]

`nslookup google.com -type=soa google.com`
Lookup for an soa record   
SOA record (start of authority), provides the authoritative information about the domain, the e-mail address of the domain admin, the domain serial number, etc

![[Pasted image 20221130173828.png]]

`nslookup google.com -type=any google.com`
nslookup followed by the domain name will display the “A Record” (IP Address) of the domain. Use this command to find the address record for a domain. It queries to domain name servers and gets the details.
![[Pasted image 20221130171828.png]]

`nslookup -type=ns google.com` 
Lookup for an ns record  NS (Name Server) record maps a domain name to a list of DNS servers authoritative for that domain. It will output the name serves which are associated with the given domain.

![[Pasted image 20221130173749.png]]

`nslookup -type=a google.com`
 We can also view all the available DNS records for a particular record using the _-type=a_ option.

![[Pasted image 20221130174201.png]]

`nslookup -type=mx google.com`
Lookup for an mx record MX (Mail Exchange) record maps a domain name to a list of mail exchange servers for that domain. The MX record tells that all the mails sent to “google.com” should be routed to the Mail server in that domain.

![[Pasted image 20221130174823.png]]

`nslookup -type=txt google.com`
Lookup for an txt record TXT records are useful for multiple types of records like DKIM, SPF, etc. You can find all TXT records configured for any domain using the below command.

![[Pasted image 20221130174932.png]]
