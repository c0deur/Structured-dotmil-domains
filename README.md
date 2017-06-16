# Purpose
This repository was built only for research purposes in accordance with https://hackerone.com/deptofdefense?view_policy=true.
If you interested in contributing or research - make sure you read it.

# Relevance
All listed dotmil domains was alive at the moment of publication (bad records was filtered - domains with DNS errors, ConnectFailure, etc. - but sure, we could miss something). We will check and update the lists in the future.
The domains with 403, 404, 401, 500 codes, TrustFailure or other SSL problems was listed too. In general, this repository contains around 2000 valid domain records.

# Testing
Some subdomains are not accessible on port 80, so `https://` prefix is required upon testing. Also some domains requires `www.` prefix. Avoid the using of automated tools - DoD firewalls can block your IP address and even IP pool, and you will loose access to the some part of domains. If you still want to use it - make sure that you set the delay between requests (2-3 sec. minimum).

# Methodology used for collecting
1) Enumerating all possible subdomains through various tools (DNScan, SubBrute, Sublist3r, passive collection from search engines, etc)
2) Merging them to one big list.
3) Deleting duplicate records.
4) Checking common ports (80, 443, 8000, 8080, 8888), generating new list of valid subdomains
5) Committing to the repository.
As you see, we still can miss some domains, which have some services running on non-standart ports. In the future, we will recheck the original lists again with Masscan tool, and update the lists.


# Credits
https://twitter.com/h1_sp1d3r (Evgeniy Yakovchuk)

https://twitter.com/_Psycho_Mantis (Alyssa Herrera) - this repository was previously based on the fork of the researcher's project - https://github.com/Alyssa-o-Herrera/Mil-Domains, but now contain much more records, and structurized for easier targeting and scope testing.

#### Make The DoD Security Great Again!
