# whitelist-generator

Simple script to create white list of the mail servers of big
companies who won't comply with the RFCs — for obvious reasons.

# Grey listing against spam
Grey listing is a very effective anti spam mechanism. The RFC states
that any message that is not accepted should be tried again in a few
minutes. Usually after a second attempt a grey filtering host accepts
the message. Spam bots don't have time to go through those procedures
and will not retry.

# Big Companies
On the other hand, big companies like gmail and hotmail have to deal
with massive volumes of mail and also don't retry sending emails.

# How this script works.
To create a whitelist for those hosts this script checks their usually
well maintained spf record. An spf record is stored in the txt record for dns.

# Reference for SPF records.
Here is a complete syntax description for spf records:
  http://www.openspf.org/SPF_Record_Syntax

