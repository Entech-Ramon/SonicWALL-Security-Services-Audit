# SonicWALL Firewall Security Services Auditing

This project involved making Security Services Flexible Assets in ITGlue to allow easy auditing and ticketing of security services being disabled for our clients, without the use of SonicWALLs GMS.

### Prerequisites

Hardware:
    Next Gen SonicWALLs that support the SonicOS 6.5.3 firmware. (Required for SonicOS API introduced in version 6.5.1, we are NOT using SSH)

Software/Services:

Azure Automation Account or Server to Run Scripts with Powershell version 3 or above.
Database (Can be SQL, Power Apps Common Data Service, Excel SpreedSheet/CSV or even ITGlue) of client external IPs, and a way to Link to their ITGlue ID.

Azure KeyVault (Used to store ITGlue and Ticketing Software API keys)

Enable the SonicOS API for each SonicWALL using Basic Auth

ITGlue:
    SonicWALL Admin Passwords Documented and Specific Password Category set for them. (Example, We used the Password Category "SonicWALL Admin")


### Details


### Security Considerations

In an effort to ensure Security is kept for our company and clients, I've choosen to use Auzre for handling the Powershell Scripts.
Using an Azure Automation account and Azure Key Vault, we are able to pull API Keys and Sonicwall Passwords without the fear of this sensitive info being passed or stored insecurely.

## Authors

Ramon Ayala - Entech
https://EntechUS.com
