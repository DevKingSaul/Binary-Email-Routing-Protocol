# Main Concept
#### BERP (Binary Email Routing Protocol) is a replacment for the old SMTP. SMTP is a text protocol but BERP will be a binary protocol.

# Upgrade Process
#### A BERP server will add the response `250-SMTP_BERP` to EHLO/HELO command.
#### A BERP client will send the command `UPGRADEBERP` if it sees `250-SMTP_BERP`
#### BERP Server will send `220 Upgrade to BERP` if it gets command `UPGRADEBERP` and sets streaming mode to Binary Email Routing Protocol. From here on the TCP packets will be sent in the format of BERP
