Guide to extract active git committers for the last 90 days
===========================================================

You may use this guide if you are in the process of estimating how many GHAS licenses you need for the active committers you have in your business critical git repos. Some information that you need to know.

1. Github assigns GHAS license on Users that have active commits on the private repo for the last 90 days. You may view this link for more information: 
 - https://docs.github.com/en/enterprise-cloud@latest/billing/managing-billing-for-github-advanced-security/about-billing-for-github-advanced-security#about-committer-numbers-for-github-advanced-security

2. To extract the active committers in the last 90 days, run the script as follows in your target private repo (clone it if you haven't yet). With the extracted information, you would know exactly how many users will need licenses before you enable GHAS feature. The script uses both native git and bash command.
 - https://github.com/pangoy2nd/git_license_report/blob/main/git-linux-cmd
 
3. To avoid incurring unnecessary licensing cost, you may setup an approval process before a User is added into the repo. You may use your favorite ticketing tool, but the idea is, all Users that need access to your sensitive git repos where GHAS is enabled will need User Manager and Infosec approval before they can be added to the git repo. With this, you have an audit and control of who is being added to the repo which is also a security best practice.
