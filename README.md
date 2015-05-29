![a kraken](https://raw.githubusercontent.com/netkraken/minion/master/res/octopus.png)

# netkraken | the spider

spiders a whole bunch of hosts, fetching its network connection data

## TL;DR

* ```build-exe BUILDHOST``` bundles the minion and python libs to one archive (use the BUILDHOST with the oldest glibc to get a most-portable archive)

* ```jumpto JUMPHOST``` transfer everything you need to the privileged jump host

* on the jump host: ```spreadout LIST_OF_HOSTS``` spreads the minion to the listed hosts

* on the jump host: ```spider LIST_OF_HOSTS``` spiders the connection data on all listed hosts (Note1: minion must be present on all hosts. Note2: pdsh syntax possible, like ^FILE_WITH_HOSTNAMES)

* on the jump host: ```reap LIST_OF_HOSTS``` collects spidered data from listed hosts


