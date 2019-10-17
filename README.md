Laptop
=======

Laptop is a script to setup a MacOS computer for teams and to keep it updated.


It can be run multiple times on the same machine safely.
It installs, upgrades or skips packages based on what is already installed.


Requirements
------------


This has been tested on

* OS X Mojave (10.14) 
* OS X El Capitan (10.11)
* OS X Yosemite (10.10)




Install
-------


Open the Terminal application on your Mac. 

In your Terminal window, copy and paste the command below, then press `return`


```sh
bash <(curl -s https://raw.githubusercontent.com/ddl-retornam/laptop/master/laptop)
```


The [script](https://github.com/ddl-retornam/laptop/blob/master/mac) itself is available
in this repo for you to review.

The script will ask you to enter your laptop's password at various points in the install
process. 


It is highly recommended to run the script regularly to keep your computer up to date.
Once installed you'll be able to run it at your convenience by typing `laptop` and hitting
`return` in your Terminal.




Customize in `~/.ddllaptop/.laptop.local` and `~/Brewfile.local`
----------------------------------------------------------------

Your `~/.laptop.local` is run at the end of the `mac` script.
Put your customizations there. If you want to install additional tools or Mac apps
with Homebrew, add them to your `~/.ddllaptop/Brewfile.local`.

```sh
# Go go your user's $HOME directory
cd ~/.ddllaptop/
```

We currently install the following tools and apps:

* [Docker]          - Docker for Mac
* [Keybase]         - Keybase client for Mac
* [Minikube]        - Minikube
* [Slack]           - Slack
* [Harvest]         - Harvest time tracking for Mac
* [Ack]             - Better grep tool for programmers
* [k9s]             - Kubernetes CLI to manage your cluster in style
* [kubectx]         - Kubernetes context tool
* [jq]              - commandline JSON tool
* [tfenv]           - Terraform environment management tool
