# Welcome to Ronin Dojo
Ronin Dojo is the RPi4 and Odroid N2 installation variant of Samourai Wallet's Dojo. This is not a change to their code or application, rather the installation process modified specifically for RPi4/Odroid. 

Our Mission is to bring full on-chain self-sovereignity at an afforable price!

“I dreamt of worldly success once.”

> Miyamoto Musashi, also known as Shinmen Takezō, Miyamoto Bennosuke or, by his Buddhist name, Niten Dōraku, was a Japanese swordsman, philosopher, strategist, writer and rōnin. Musashi, as he was often simply known, became renowned through stories of his unique double-bladed swordsmanship and undefeated record in his 61 duels.

“It is said the warrior's is the twofold Way of pen and sword, and he should have a taste for both Ways. Even if a man has no natural ability he can be a warrior by sticking assiduously to both divisions of the Way.”

> A Ronin was a samurai warrior in feudal Japan without a master or lord — known as a daimyo. A samurai could become a ronin in several different ways: his master might die or fall from power or the samurai might lose his master's favor or patronage and be cast off.

“Know your enemy, know his sword.”

Be Your own MASTER!

# What is Samourai Dojo?
As stated by the Samourai Team:
>Samourai Dojo is the backing server for Samourai Wallet. Provides HD account & loose addresses (BIP47) balances & transactions lists. Provides unspent output lists to the wallet. PushTX endpoint broadcasts transactions through the backing bitcoind node.

This implementation connects to your wallet via Tor for increased privacy and allowing for connectivity anywhere without forwarding ports and exposing your home IP address.

For more information on Samourai Wallet, Dojo, and Whirlpool visit the [Samourai Wallet Github](https://github.com/Samourai-Wallet). 

For FAQs about all things Samourai Wallet, check out @PuraVida's [FAQ wiki](https://github.com/PuraVlda/samourai-wallet-android/wiki/Frequently-Asked-Questions).

## Recommended Hardware
The Full Dojo installation, which includes a fresh sync of the Bitcoin blockchain, requires a little over 3GB of RAM during the initial sync. Then it drops to a little less than 2GB after sync is complete. The setup will require about 350GB of data storage and growing daily.

### Devices 
* [Raspberry Pi4 w/4GB RAM](https://www.canakit.com/raspberry-pi-4-4gb.html?cid=usd&src=raspberrypi)
* [Odroid N2](https://www.hardkernel.com/shop/odroid-n2-with-4gbyte-ram/)

### Storage
Given the increased performance and longevity of use: we recommend 1TB SSD such as: 
* [Samsung T5](https://www.amazon.com/Samsung-T5-Portable-SSD-MU-PA1T0B/dp/B073H552FJ/ref=sr_1_1?fst=as%3Aoff&qid=1571081118&refinements=p_n_feature_three_browse-bin%3A6797521011&rnid=6797515011&s=pc&sr=1-1)
* [Seagate Fast SSD](https://www.amazon.com/Seagate-External-Reversible-Type-C-STCM1000400/dp/B07DX7D744)

Or internal 1TB SSD plus SATA-to-USB 3.0 cable:
* [Samsung EVO 860](https://www.amazon.com/dp/B078DPCY3T/)
* plus [Eluteng adapter cable](https://www.amazon.com/dp/B0716JKJ68/)

However, if you are looking to run a node a budget, you can use external HDDs such as: 
* [Toshiba Canvio 1TB](https://www.amazon.com/Toshiba-HDTB410XK3AA-Canvio-Portable-External/dp/B079D359S6/ref=sr_1_4?crid=27WAK2Y8TLQEX&keywords=external+hard+drive&qid=1571082291&refinements=p_n_feature_two_browse-bin%3A5446812011&rnid=562234011&sprefix=external%2Caps%2C234&sr=8-4)
* [Seagate Expansion 1TB](https://www.amazon.com/Seagate-Expansion-Portable-External-STEA1000400/dp/B00TKFEEAS/ref=sr_1_14?crid=27WAK2Y8TLQEX&keywords=external+hard+drive&qid=1571082291&refinements=p_n_feature_two_browse-bin%3A5446812011&rnid=562234011&sprefix=external%2Caps%2C234&sr=8-14)

>**Do your own research to find out which SSD/HDD you believe is best for you, these are recommendations.**

### SD cards
You'll need a SD card to flash the OS of choice (we will cover Raspbian and Manjaro-ARM).
For this we recommend: [Samsung EVO+ 64GB](https://www.amazon.com/Samsung-MicroSDXC-Memory-Adapter-MB-MC64GA/dp/B06XFWPXYD/ref=sr_1_4?keywords=EVO%2B+SD+card&qid=1571081610&s=electronics&sr=1-4). You'll need at least 16GB but for the price this is a great deal for a high quality SD card. 

## Flashing Operating System
Ronin is based on [Manjaro-ARM Minimal](https://osdn.net/projects/manjaro-arm/storage/rpi4/minimal/19.10/).

## Cases
We strongly recommend getting a case that keeps the Pi or Odroid cool. 
1. For RPi4: 
   - For a Custom Samourai Wallet Ronin Dojo Case, we highly recommend CrytpoCloak! Comes with storage for Pi4 AND external storage device (check size requirements). [Check it out here](https://thecryptocloak.com/product/samourai/).
      - NOTE: WE DO NOT RECEIVE COMPENSATION FOR THEIR PRODUCT, but an awesome product at that. 

<p align='center'>
  <a href='https://thecryptocloak.com/product/samourai/'>
    <img src='https://thecryptocloak.com/wp-content/uploads/2019/10/IMG_20191029_061006.jpg' alt='screenshot' />
  </a>
</p>

   - Case with passive cooling such as: [Flirc](https://www.amazon.com/Flirc-Raspberry-Pi-Case-Silver/dp/B07WG4DW52/ref=sr_1_8?keywords=pi4+case&qid=1571082492&sr=8-8) 
   - Case with a fan such as: [Miuzei](https://www.amazon.com/Miuzei-Raspberry-Cooling-Heat-Sinks-Supply/dp/B07TTN1M7G/ref=sr_1_5?crid=2FLR4GW4Y32PN&keywords=pi4%2Bcase%2Bwith%2Bfan&qid=1571082607&sprefix=pi4%2Bcase%2B%2Caps%2C222&sr=8-5&th=1) 

2. For Odroid:
   - Case with passive cooling such as: [KSSB Case](https://ameridroid.com/products/kksb-odroid-n2-case)
   - Original case: [ODROID-N2 Case](https://ameridroid.com/products/odroid-n2-case)

# Installation
Head to our [Install Guide](https://github.com/RoninDojo/RoninDojo/blob/development/Ronin-UI-Guide.md).

# Contributors
This list is continuously growing, I will do my best to update as much as I can. If you would like to contribute please feel free to pull or DM me to help!

@GuerraMoneta @BTCxZelko @Burcakbaskan @k3tan @kdmukai @crazyk031 @jaimefoo

@romanz - Electrs

@openoms, @rootzoll, and @bavarianledger - Raspiblitz team for inspiration and Electrs implementation. 

If we missed you please let me know.

## Support

If you appreciate our work and wish to support our continued efforts in providing free, unencumbered, open source code that enhances your sovereignty please consider a donation.

### Address

bc1ql06r3jjx3hmd09eexs7mawczayfqxpx7r3l20hvs3cuq5suv5hvswspdaz

[![address](http://api.qrserver.com/v1/create-qr-code/?color=000000&bgcolor=FFFFFF&data=bc1qma3vyljvz0n3n0e7czaewx8tq5heugv2kvrcq2&qzone=1&margin=0&size=200x200&ecc=L)](https://oxt.me/address/bc1ql06r3jjx3hmd09eexs7mawczayfqxpx7r3l20hvs3cuq5suv5hvswspdaz)

All donations will go to providing the team with more hardware for implementating new features.

## FINALLY, a huge Thanks to the Samourai Wallet Dev team!
### As long they continue to build we will continue to support!

Questions, discussion, etc?

Check out the Telegram groups:

[Samourai Wallet](https://t.me/SamouraiWallet)

[Dojo](https://t.me/samourai_dojo)

[Whirlpool](https://t.me/whirlpool_trollbox)

[Off Topic](https://t.me/samouraifunny)
