#Road Map
---------
In priority order (feel free to reorder.)
###etherRe.al components
An **etherReal-KΞY** is the "smart contract" that a user must use to access the admin rights of their etherReal-IÐ.  The etherReal-KΞY is not uneque and if the user looses accss to, or control over, their etherReal-KΞY it can be revoked and a new etherReal-KΞY created. 

An **etherReal-AÐÐress** is a unique and imutable, publicly accessable address used to referance a persistant **etherReal-IÐ** no matter whether the user looses forgets or changes their **etherReal-KΞY** the **etherReal-AÐÐress** for a given **etherReal-IÐ** will remain the same.  

An **etherReal-IÐ** is the sum of a users credentials, digital relationships and other attested information, particulaly the interconnections with the **etherReal-IÐs** of others.   The **etherReal-IÐ** stores this information in a **VouchSafe**

The **VouchSafe** is an off chain data store that contains the kind of personal information that one would keep in a safe (or other secure place) at home.  IT may contain digital representations of Birth Certificates, Passports, driving licences etc.


-----------------

###etherre.al registration
- [ ] Pretorian ** etherReal- AÐÐress creation** Contract that lets any user register/generate a primary key they then ask the “Pretorian” to enter that etherReal-IÐ into the etherReal-AÐÐress registry, 
- [ ] **etherReal-AÐÐress  registry** -> users etherReal-KΞY maped to  **etherReal-IÐ**, Plus public information ? Like nick name, DOB ? <- this is the public record part of the system.  
  - [ ] ***etherReal-KΞYRING sub registry** -> user may have as many other keys as they wish to asociate with their etherReal-IÐ.  This sub regestry tracks these sock pupets as belonging to one uneque Real-ID <- this regestry is searchable but all the serch shoud reveal is a zero knowledge froof that the key is "owned" by a Real ID.

###proxy contract
- [ ] each user 
###sortition
- [ ] **Sortition** -> search through a regestry and return x random ID's based on peramiters <-- this should be useful for all sorts of other structurs and is better kept in a contract than any one (not just etherreal) can call.
 - [ ] **EtherReal Sortition** etherreal calls Sortition with a geographical permiter and a range peramiter.
 - [ ] **asigning roles** the keys returned by Sortition are matched to their roles:- Hoste - Witness - Watchman  <- [ ] IMPROVE perminlogy this sucks!

###etherre.al engine
I propose that the ID engine be run on a token system that creates an audit trail from ID to ID.  Tokens are transferable but non fungible, are minted within an EtherReal-ID at account creation and one is transfered to each etherreal-ID the account vouches for.
- [ ] **Reality Cheque** users Real-IDs have are ranked by checking their "ballance" or ID tokens.  <-  Max reality cheque balance should be 100.  Accounts are created with a minus balance to signify that they are "UnReal"
- [ ] **Bean Counter** (A type of block explorer)  when a user verifes another user they "swap" tokens.  If the tokens a user holds turn ‘bad’ that reflects bably on the them. 
  - [ ] **Witch Finder**  If a user flaggs an other ID as "UnReal" they stake their own ID on the clame. Equaly they stake their own ID on a clame that others are "EtherReal". 
  - [ ] **Ducking Stool** If a suspect ID turns out to be a REAL person then the "witch finder" gets punished (their ID is suspect.  do their tokens get tainted?)
  - [ ] **Poisening the Well** If the suspect ID turns out to be a FAKE then all the tokes that originated with that fake ID become bad and damage the IDs of their holders.

###VouchSafe					
- [?] Information is accessed by ring signature <--
- [ ] verification system key signing
- [ ] reporting, mechanism
- [ ] add transaction with evaluation - any TX on the blockchain can be referenced and evaluated as long as the user has taken part in it
- [ ] Multi-Sig-Wallet with daily limits

###Watchman 
- [ ]

####App / HTML / Wisper / Whatever stuf that can be kept off the block 
- [ ] **OpenID** allow users to register with an OAuth or OpenID account in order to save them the typing of the information
- [ ] **Leverage OpenPGP** If a user has an OpenPGP certificate, import it from https://sks-keyservers.net/i/ and if any signer of her certificate is a member already, then ask her to validate the signature
- [ ] **QR-code handeler** generate QR-Code to avoid typing when validating IDs

#House Keeping#
- [ ] Create the framework consultaiton process on http://dapp.etherre.al <<Does not exist yet 
- [ ] Populate Github issues

####Dont know where to put.
- [ ] sort users by gographical location (and distance they are prepaired to travel.)
- [ ] FoaF (Friend of a friend) network / WoT (Web of Trust) folowing the read write web moddel
        identi.fi ? may be a good FoaF system to use? have emailed, will see what becomes of it.
              (Not a core part of etherre.al but it will speed addoption)




