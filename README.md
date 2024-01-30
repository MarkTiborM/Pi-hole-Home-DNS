# Pi-hole-Home-DNS 
## In this project, I will show you how to put together a raspberry pi that filters out unwanted ads through a DNS sinkhole on your router.



![Pi-hole_vector_logo](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/737c03a7-1794-41e3-90bd-015cd4fc64cd) 

(fig 1 wikipedia)
# What is a Pi-hole?
### A Pi-hole is a Raspberry Pi that has been configured with a DNS sinkhole that protects devices on your network from unwanted content.  
Here is a link to the documentation : https://docs.pi-hole.net

# Resources :
## Raspberry Pi
### In terms of price, the Pi zero is the best bang for your buck as this server runs headless, so a better raspberry pi is not needed. However within this guide I have used a Pi 3 B. I have personally had a great experience using the Raspberry Pi 3 B for other projects so I recommend it. 
https://www.raspberrypi.com/products/raspberry-pi-3-model-b/

![770A4980_sm__94390](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/cb353afe-4017-4679-8c49-c235d7429e25)

(fig 2 Pishop.us)

## Raspberry Pi Case
### I recommend this iUniker Raspberry Pi 3 b+ case. It comes with a fan, heatsink pads and a powersupply iwth a switch. 
![case](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/581b2996-a8c6-470a-b174-25e14c7bbe0c)

(fig 3 amazon.com)

# Getting Started 
### Install the Headless Firmware onto your Raspberry Pi
### Do this by first installing the Raspberry Pi Imager on their website : https://www.raspberrypi.com/software/
### After you install the imager, select the device that you want to connect and your storage device, then install the lite version of the raspi OS
![image_2024-01-29_211341616](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/93bf7165-7a1c-4ba2-8987-8d0ddd749fd0)

# Installing Pi-hole
### First, update your raspberry Pi with, 
## sudo apt-get update && apt-get upgrade
### Then, input the following command to install Pi hole :
## curl -sSL https://install.pi-hole.net | bash
![vlcsnap-2022-09-01-11h04m47s566-ezgif com-webp-to-png-converter](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/34069502-f657-42e4-810a-f72a6136819e)

(fig 4 core-electronics.com.au)
