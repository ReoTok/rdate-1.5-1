# rdate-1.5-1
rdate-1.5-1-omv4090.x86_64.rpm backup , who could sync standard time in Centos OS.

# how to install
rpm -ivh https://github.com/ReoTok/rdate-1.5-1/blob/main/rdate-1.5-1-omv4090.x86_64.rpm

# How to sync the time.
/usr/bin/rdate -s time.nist.gov

# Set a Crontab to sync automaticly maybe..
crontab -e
*/10 * * * * /usr/bin/rdate -s time.nist.gov
crontab -l

# Good , well done !
