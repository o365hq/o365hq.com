+++
title = "Office 365 Encrypted Email - Initial Setup"
description = "Office 365 uses encryption in two ways: in the service, and as a customer control. In the service, encryption is used in Office 365 by default. If you want to increase the security level of messaging and protect extremly sensitive data, we will provide implementation service to email encryption and rights protection capabilities. "
date = 2019-02-22

[taxonomies]
products = ["Office 365"]
types = ["Security and Protection"]

[extra]
sku = "ITPWW280IMPOT"
price = "$450"
duration = "1 day"
manager = "Mike Mackey"
+++

Microsoft provides three email encryption options for your Office 365.
IT Partner will be able to implement any of them. You might compare the
options shown below. Also, please check out the [YouTube video
explanation](https://www.youtube.com/watch?v=KmfxCd5ublI).

  ------------------------------------------------------------------------------------------------------------------------------------------------------
                    Office 365        Information Rights Management in Exchange Online                                               S/MIME for message
                    Message                                                                                                          signing and
                    Encryption                                                                                                       encryption
  ----------------- ----------------- ---------------------------------------------------------------------------------------------- -------------------
  What is it?\      Office 365        IRM is an encryption solution that also applies usage restrictions to email messages. S/MIME is a
                    Message.          It helps prevent sensitive information from being printed, forwarded, or copied by             certificate-based
                    Encryption        unauthorized people.\                                                                          encryption solution
                    (OME) is IRM capabilities in Office 365 use Azure Rights Management (Azure RMS).\     that allows you to
                    a service built                                                                                                  both encrypt and
                    on Azure Rights                                                                                                  digitally sign a
                    Management (Azure                                                                                                message. The
                    RMS)                                                                                                    message encryption
                    that lets you                                                                                                    helps ensure that
                    send encrypted                                                                                                   only the intended
                    email to people                                                                                                  recipient can open
                    inside or outside                                                                                                and read the
                    your                                                                                                             message. A digital
                    organization,                                                                                                    signature helps the
                    regardless of the                                                                                                recipient validate
                    destination email                                                                                                the identity of the
                    address (Gmail,                                                                                                  sender.\
                    Yahoo! Mail,                                                                                                     Both digital
                    Outlook.com,                                                                                                     signatures and
                    etc.).\                                                                                                          message encryption
                    As an admin, you                                                                                                 are made possible
                    can set up                                                                                                       through the use of
                    transport rules                                                                                                  unique digital
                    that define the                                                                                                  certificates that
                    conditions for                                                                                                   contain the keys
                    encryption. When                                                                                                 for verifying
                    a user sends a                                                                                                   digital signatures
                    message that                                                                                                     and encrypting or
                    matches a rule,                                                                                                  decrypting
                    encryption is                                                                                                    messages.\
                    applied                                                                                                          To use S/MIME, you
                    automatically.\                                                                                                  must have public
                    To view encrypted                                                                                                keys on file for
                    messages,                                                                                                        each recipient.
                    recipients can                                                                                                   Recipients have to
                    either get a                                                                                                     maintain their own
                    one-time                                                                                                         private keys, which
                    passcode, sign in                                                                                                must remain secure.
                    with a Microsoft                                                                                                 If a recipient's
                    account, or sign                                                                                                 private keys are
                    in with a work or                                                                                                compromised, the
                    school account                                                                                                   recipient needs to
                    be associated with                                                                                                  get a new private
                    Office 365.                                                                                                      key and
                    Recipients can                                                                                                   redistribute public
                    also send                                                                                                        keys to all
                    encrypted                                                                                                        potential senders.\
                    replies. They                                                                                                    
                    don't need an                                                                                                    
                    Office 365                                                                                                       
                    subscription to                                                                                                  
                    view encrypted                                                                                                   
                    messages or send                                                                                                 
                    encrypted                                                                                                        
                    replies.\                                                                                                        

  What does it do?\ OME:\    IRM:\                                                                                 S/MIME addresses
                    Encrypts messages Uses encryption and usage restrictions to provide online and offline protection for email      sender
                    sent to internal  messages and attachments.\                                                                     authentication with
                    or external       Gives you, as an admin, the ability to set up transport rules or Outlook protection rules to   digital signatures,
                    recipients.\      automatically apply IRM to select messages.\                                          and message
                    Allows users to   Lets users manually apply templates in Outlook or Outlook Web App.\                            confidentiality
                    send encrypted                                                                                                   with encryption.\
                    messages to any                                                                                                  
                    email address,                                                                                                   
                    including                                                                                                        
                    Outlook.com,                                                                                                     
                    Yahoo! Mail, and                                                                                                 
                    Gmail.\                                                                                                          
                    Allows you, as an                                                                                                
                    admin, to                                                                                                        
                    customize the                                                                                                    
                    email viewing                                                                                                    
                    portal to reflect                                                                                                
                    your                                                                                                             
                    organization's                                                                                                   
                    brand.\                                                                                                          
                    Microsoft                                                                                                        
                    securely manages                                                                                                 
                    and stores the                                                                                                   
                    keys, so you                                                                                                     
                    don't have to.\                                                                                                  
                    No special client-                                                                                                
                    side software is                                                                                                 
                    needed as long as                                                                                                
                    the encrypted                                                                                                    
                    message (sent as                                                                                                 
                    an HTML                                                                                                 
                    attachment) can                                                                                                  
                    be opened in a                                                                                                   
                    browser.\                                                                                                        

  What does it not  OME      Some applications may not support IRM emails on all devices. For more information     S/MIME doesn't
  do?\              doesn't let you   about these and other products that support IRM email, see [Client device             allow encrypted
                    apply usage       capabilities](https://docs.microsoft.com/en-us/azure/information-protection/requirements#BKMK_ClientCapabilities).\   messages to be
                    restrictions to                                                                                                  scanned for
                    messages. For                                                                                                    malware, spam, or
                    example, you                                                                                                     policies.\
                    can't use it to                                                                                                  
                    stop a recipient                                                                                                 
                    from forwarding                                                                                                  
                    or printing an                                                                                                   
                    encrypted                                                                                                        
                    message.\                                                                                                        

  Recommendations   We recommend      We recommend using IRM when you want to apply usage restrictions as well as           We recommend using
  and example       using             encryption. For example:\                                                                      S/MIME when either
  scenarios\        OME when A manager sending confidential details to her team about a new product applies the "Do Not     your organization
                    you want to send  Forward" option.\                                                                              or the recipient's
                    sensitive         An executive needs to share a bid proposal with another company, which includes an attachment  organization
                    business          from a partner who is using Office 365, and require both the email and the attachment to be    requires true
                    information to    protected.\                                                                                    peer-to-peer
                    people outside                                                                                                   encryption.\
                    your                                                                                                             S/MIME is most
                    organization,                                                                                                    commonly used in
                    whether they're                                                                                                  the following
                    consumers or                                                                                                     scenarios:\
                    other businesses.                                                                                                Government agencies
                    For example:\                                                                                                    communicating with
                    A bank employee                                                                                                  other government
                    sending credit                                                                                                   agencies\
                    card statements                                                                                                  A business
                    to customers\                                                                                                    communicating with
                    A doctor's office                                                                                                a government
                    sending medical                                                                                                  agency\
                    records to a                                                                                                     
                    patient\                                                                                                         
                    An attorney                                                                                                      
                    sending                                                                                                          
                    confidential                                                                                                     
                    legal information                                                                                                
                    to another                                                                                                       
                    attorney\                                                                                                        
  ------------------------------------------------------------------------------------------------------------------------------------------------------

Our **objective** is to enable email encryption in your Office 365
tenant and provide instruments to control sensitive data with flexible
policies or ad hoc customer controls that are built into Office 365.

An implementation project will be considered **successful** when you:

1.  send encrypted emails from any device
2.  easily navigate through encrypted messages
3.  deliver encrypted email directly to recipients' inboxes
4.  decrypt and read encrypted email with confidence, without installing
    client software
5.  enjoy simplified user management that eliminates the need for
    certificate maintenance

### IT Partner responsibilities

-   Set up Email Encryption in Office 365
-   Create mail flow rules that define the conditions for encryption
-   Bring your own key (BYOK) settings if needed

### Client responsibilities

-   Provide a dedicated point of contact responsible for working with IT
    Partner and coordinate any outside vendor resources and schedules, if needed
-   Configure all networking equipment, such as load balancers, routers,
    firewalls, and switches
-   Set up and configure the email client(s) on end-user devices

### Outside  the scope of this project (additional cost items)

-   Mailbox migration to Office 365 (Exchange Online)
-   AD and group policy settings

Upon completion of the engagement, we will provide a project closeout
report. This document will indicate final project status, including
evidence of meeting acceptance criteria, outstanding issues, if any, and final
budget. If you want more extensive documentation, it can be provided
for an additional fee.

### Prerequisites

-   You must have global admin level access to the source Office 365
    tenant
-   You must have global admin level access to the destination Office
    365 tenant, with Exchange Online licenses available

To use the new OME capabilities, you need one of the following
plans:

-   Office 365 Message Encryption is offered as part of Office 365 E3
    and E5, Microsoft E3 and E5, Office 365 A1, A3, and A5, and Office
    365 G3 and G5. Customers do not need additional licenses to receive
    the new protection capabilities powered by Azure Information
    Protection
-   You can also add Azure Information Protection Plan 1 to the
    following plans to receive the new Office 365 Message Encryption
    capabilities: Exchange Online Plan 1, Exchange Online Plan 2, Office
    365 F1, Office 365 Business Essentials, Office 365 Business Premium,
    or Office 365 Enterprise E1
-   Each user benefiting from Office 365 Message Encryption needs to be
    licensed to be covered by the feature
-   For the full list, see the [Exchange Online service
    descriptions](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-service-description)
    for Office 365 Message Encryption.

### Plan

May vary depending on your needs.

1.  Kickoff meeting
2.  Pre-implementation system health check
3.  Сonfiguring OME and additional tools
4.  Setting up Exchange Online Transport Rules
5.  Verify email encryption
6.  Post-implementation tasks

### Results

You will be able to use Office 365 Message Encryption (OME)
capabilities that protect your emails, and mail flow rules that define the
conditions for encryption. Your email recipients should be able to
receive and reply to your secure emails using any device with any email
client.

### Relevant articles

1.  [Office 365 Message Encryption
    FAQ](https://support.office.com/en-us/article/office-365-message-encryption-faq-0432dce9-d9b6-4e73-8a13-4a932eb0081e)
2.  [Office 365 Message
    Encryption](https://products.office.com/en-us/exchange/office-365-message-encryption)
3.  [Email encryption in Office
    365](https://support.office.com/en-us/article/email-encryption-in-office-365-c0d87cbe-6d65-4c03-88ad-5216ea5564e8)
