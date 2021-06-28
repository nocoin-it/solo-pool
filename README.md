# Nocoin
## Goal
The followed procedure describe how to setup remove harvest using solo plots,
it's completely based on the official procedure described on [Farming-on-many-machines](https://github.com/Chia-Network/chia-blockchain/wiki/Farming-on-many-machines)
How to setup remote harvest


## What you need to setup your harvest


- follow the official doc to import CA [Farming-on-many-machines](https://github.com/Chia-Network/chia-blockchain/wiki/Farming-on-many-machines)
- be sure your host it's reachable on 8560 
- stop all service 
  - chia stop all
- On config.yml setup update the followed parameters
  - <b>Setup farmer_peer</b>
    - farmer_peer:
      - host: afdc.nocoin.it
      - port: 8447
  - <b>Update change self_hostname value</b>
    -  default value is  localhost need to be updated to 0.0.0.0 
 - Start only harvest service
   - chia start harvest

# What you need to give to us
To finalize the join please send us (info@nocoin.it) your farmer and pool key (no mnemonic)

# Warning
<b>Avoid to run farming  when you run remote harvest to avoid dual farming
and incurring in ban</b>
