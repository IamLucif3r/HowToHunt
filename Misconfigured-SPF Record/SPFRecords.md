## Misconfigured SPF Records

### What is an SPF Record ?
An SPF record is a Sender Policy Framework record. It’s used to indicate to mail exchanges which hosts are authorized to send mail for a domain. It’s defined in RFC 4408, and clarified by RFC 7208.

### What is the Impact of No-SPF Records ?
SPF can help protect email senders and recipients from spam, spoofing, and phishing. In addition to safeguarding against email risks, properly configuring your email authentication can positively impact your deliverability. When there is no SPF record, the 

---

### How to check SPF Record for a domain ?

1.You can use several online tools to check the SPF record for a domain. Some of these are : <br>
   -[Kitterman](https://www.kitterman.com/spf/validate.html)<br>
   -[MXToolBox](https://mxtoolbox.com/)<br>
2. Browse to any one of the above tools and enter the domain name.
3. If you find any existing SPF record, this means the domain is not vulnerable.
4. Else if there is no SPF record, means you can report the issue.


### Exploiting 

1. Go to a Fake Mail sending Service.
 - [Emkei](https://emkei.cz/) : You can use this service
2. In the Sender's email, write Email from an authority of company (For ex. admin@company.com)
3. Send the mail to yourself.
4. You'll receive an email that would look like a genuine email from compant.

<b>You Can report this vulnerability</b>
