(reference-terms-ssl-certificates)=
# SSL certificates

**Secure Sockets Layer (SSL) certificates** are part of creating secure communication over the internet. They provide a process for encrypting and authenticating data sent between a client and a server. In the context of Landscape, being a systems management tool, it uses SSL certificates to communicate securely with its servers, reducing the chance of unauthorized access and data breaches.

If you install Landscape with a public IP, the {ref}`how-to-quickstart-installation` guide recommends you install an SSL certificate from a certificate authority, such as LetsEncrypt. The SSL certificate is used to secure the communication between the Landscape server and the clients as the data travels over public networks. This ensures that only the intended recipient can decrypt and access it. In other words, if someone were able to intercept the communication, they wouldn't be able to understand the data being sent because it's encrypted.

You can think of Landscape as a post office system and SSL certificates as special keys to specific mailboxes. The mailboxes represent the network connections between Landscape servers and clients. The Landscape server is like a mail carrier, and the Landscape clients are the recipients. To send a secure message, the mail carrier (the Landscape server) locks the message (data) with a special key (SSL certificate). Only the recipient (the Landscape client) with the matching key can open it. This is how Landscape communicates securely with servers using an SSL certificate.
<br>
<br>
<br>

> *Thanks to the following contributor(s): [@Owsalla](https://github.com/Owslla)*

