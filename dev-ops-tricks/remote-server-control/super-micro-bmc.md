# SuperMicro BMC

There are 3 ways to use the BMC on a SuperMicro motherboard: through vanilla SSH, through a CLI provided by SuperMicro, and through web browser.

## Server Can Be Remotely Controlled with Vanilla SSH

This is most likely what you are going to use. It sound primitive at first, but that's the beauty of it.

## How to Power Cycle
```bash
ssh ADMIN@10.23.53.114                 # The default username and password for SuperMicro are ADMIN

cd system1                             # These two names are common for SuperMicro, but if unsure,
cd pwrmgtsvc1                          # use ls to query what are the entry names.

stop                                   # power down the machine

start                                  # power on the machine
```