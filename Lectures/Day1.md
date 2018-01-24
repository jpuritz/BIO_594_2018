# Day 1- Getting Setup

## Goals
* Go over the syllabus
* Setup an RSA key for sshing into the class server
* Clone the class git repository to both your server account and your laptop
* Test out terminal functionality in RStudio



### Logging into the class server

Due to security reasons this will be a live demo in class.

### Setting up an RSA key

#### OS X
First, check to make sure you don't already have one
`ls -a ~/.ssh`

Make sure that there is nothing that looks like: `id_rsa` or `id_rsa.pub`

If there is not, then generate a new key:

`ssh-keygen -t rsa`

Just hit enter when it asks for a passphrase:

`Enter passphrase (empty for no passphrase):`

Hit enter again to confirm.

Now, you can copy your key to the server.  Let's pretend the user name on the server is ged.

`ssh-copy-id ged@kitt.uri.edu -p 22`

You should see somthing like this:
```
The authenticity of host '131.XXX.XXX.X' can't be established.
RSA key fingerprint is XXXXXXXXXX.
Are you sure you want to continue connecting (yes/no)?
```
Enter yes, and you should see the following:


```
/usr/bin/ssh-copy-id: INFO: attempting to log in with the new key(s), to filter out any that are already installed
/usr/bin/ssh-copy-id: INFO: 1 key(s) remain to be installed -- if you are prompted now it is to install the new keys
*******************************************
      ______ _______________________      *
      ___  //_/___  _/__  __/__  __/      *
      __  ,<   __  / __  /  __  /         *
      _  /| | __/ /  _  /   _  /          *
      /_/ |_| /___/  /_/    /_/           *
                                          *
The population genomics workstation of the* 
Puritz Lab of Marine Evolutionary Ecology *
*******************************************

You're entering a shadowy flight into the dangerous 
world of loci that might not exist.  

You're a young loner on a crusade to champion the 
cause of the innocent, the helpless, the powerless 
in a world of bioinformatics that operates above the law.

Please be responisble using this shared resource and 
contact Jon Puritz (jpuritz@uri.edu) with any issues.


ged@kitt.uri.edu's password: 
```
Enter the password that's on the board and you should be set.

### Windows 

I reccomend following the steps in this [LINK](https://docs.joyent.com/public-cloud/getting-started/ssh-keys/generating-an-ssh-key-manually/manually-generating-your-ssh-key-in-windows) through step 8.

>To generate an SSH key with PuTTYgen, follow these steps:

> 1. Open the PuTTYgen program.
> 2. For Type of key to generate, select SSH-2 RSA.
> 3. Click the Generate button.
> 4. Move your mouse in the area below the progress bar. When the progress bar is full, PuTTYgen generates your key pair.
> 5. Type a passphrase in the Key passphrase field. Type the same passphrase in the Confirm passphrase field. You can use a key >without a passphrase, but this is not recommended.
> 6. Click the Save private key button to save the private key. Warning! You must save the private key. You will need it to connect to your machine.
> 7. Right-click in the text field labeled Public key for pasting into OpenSSH authorized_keys file and choose Select All.
> 8. Right-click again in the same text field and choose Copy.

* Once the key is copied, log into the server using your password and navigate to: `~/.ssh`
* Then, enter `nano authorized_keys`
* Copy the contents into the window
* Hit CTL+X to exit and save.  Press Y to confirm. Then hit enter.


