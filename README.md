# Nocoin solo pool
## Description
With the coming out of chia un-official pools, anyone who wants to join a pool need replotting his plots or trash previous ones made with personal farmer and pool keys and (in some cases) execute custom binary untrusted code!!

We have found a way to make a pool with all people that now are solo farming without exchange private keys nor run custom chia patched versions. 

## Remote harvesting
The following procedure describes how to setup a remote harvest completely based on the official chia procedure at [Farming-on-many-machines](https://github.com/Chia-Network/chia-blockchain/wiki/Farming-on-many-machines.

You will harvest your own plots thowards our farmer server without any patch needed on your behalf!

## What you need to setup your harvest
- Follow the official doc to import from this repository our CA [Farming-on-many-machines](https://github.com/Chia-Network/chia-blockchain/wiki/Farming-on-many-machines)
- Be sure to open port 8560 on your host (it's used to count correctly your plots in our space)
- Stop all services
  - chia stop all
- Update in your config.yml the following parameters
  - <b>farmer_peer</b> to point to our farmer peer instead of localhost
    - farmer_peer:
      - host: afdc.nocoin.it
      - port: 8447
  - <b>self_hostname</b> from localhost to 0.0.0.0 in order to be reachable from outside when you open the port 8560 in previous step
    -  self_hostname: 0.0.0.0 
 - Start the harvest service (if you need in addiction you can start your wallet-only service too)
   - chia start harvest

# How to get your plots counted correctly
Once you have completed all steps in previous point please apply using the form on this page:
https://forms.gle/hc3BmnReFaJSdufn9
We need ONLY public keys (no mnemonic) in order to associate your harvest correctly... diffidate from every one asking your private keys!

# Warning
<b>Avoid in any way to solo farming when you are harvesting on our pool or you will incurr in BAN for dual farming without getting any rewards and loosing the possibility to get accepted in future in our pool!</b>

# Need info?
Feel free to join our telegram channel at [@nocoin_it](https://t.me/nocoin_it) or mail us at info@nocoin.it
