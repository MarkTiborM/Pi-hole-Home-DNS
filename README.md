# Pi-hole-Home-DNS 
## In this project, I will show you how to assemble a Raspberry Pi that filters out unwanted ads through a DNS sinkhole on your router.



![Pi-hole_vector_logo](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/737c03a7-1794-41e3-90bd-015cd4fc64cd) 

(fig 1 wikipedia)
# What is a Pi-hole?
### A Pi-hole is a Raspberry Pi configured with a DNS sinkhole that protects devices on your network from unwanted content.
Here is a link to the documentation : https://docs.pi-hole.net

# Resources :
## Raspberry Pi
### In terms of price, the Pi Zero is the best bang for your buck as this server runs headless, so a better Raspberry Pi is optional. However, within this guide, I have used a Pi 3 B. I have had a great experience using the Raspberry Pi 3 B for other projects, so I recommend it.
https://www.raspberrypi.com/products/raspberry-pi-3-model-b/

![770A4980_sm__94390](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/cb353afe-4017-4679-8c49-c235d7429e25)

(fig 2 Pishop.us)

## Raspberry Pi Case
### I recommend this iUniker Raspberry Pi 3 b+ case. It comes with a fan, heatsink pads, and a power supply.
![case](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/581b2996-a8c6-470a-b174-25e14c7bbe0c)

(fig 3 amazon.com)

# Getting Started 
### Install the Headless Firmware onto your Raspberry Pi
### Please do this by first installing the Raspberry Pi Imager on their website: https://www.raspberrypi.com/software/
### After installing the imager, select the device you want to connect and your storage device, then install the lite version of the Raspi OS.
![image_2024-01-29_211341616](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/93bf7165-7a1c-4ba2-8987-8d0ddd749fd0)

# Installing Pi-hole
### First, update your raspberry Pi with, 
## sudo apt-get update && apt-get upgrade
### Then, input the following command to install Pi hole :
## curl -sSL https://install.pi-hole.net | bash
![vlcsnap-2022-09-01-11h04m47s566-ezgif com-webp-to-png-converter](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/34069502-f657-42e4-810a-f72a6136819e)

(fig 4 core-electronics.com.au)

# Next, You will have to complete the installation wizard that displays the required IP Addresses and Passwords to be able to access your Pihole remotely. 
## I recommend going with Cloudflare as a DNS provider and also make sure to allow the Pi-Hole to rely on third party lists to block ads! 

![Installation_Process_Step_by_Step_1](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/da27a7f9-e00b-456a-bbc5-4d13ebe6f136)
(fig 5 core-electronics.com.au)


# Now you can access your Pi-Hole Web Interface through your RaspberryPi's IP!
![PiholeAdmin](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/c08a5447-496b-4b6c-adb4-48049f2f349a)
## Here is what my Admin panel looks like, although you might be asking. Why is it so empty? It's because you must add your Pi-Hole as the default DNS route.
# Next, Here is how you add your Pihole as your preferred DNS server
## Step 1.) Go to your adapter options through your network status panel
![Adapter](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/cfc8e5c1-fe6a-4159-af14-a21e21f902ef)
## Step 2.) Go to your properties of your main wifi-adapter

## Step 3.) Double click on your IPv4 
![IPV4](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/dd94010b-b92a-4bba-9fd9-65fd5fc123a1)
## Step 4.) Add your Pi-Hole's IP address as your preffered DNS server and press OK
![DNS](https://github.com/MarkTiborM/Pi-hole-Home-DNS/assets/129571496/37656e25-3fe4-4433-b371-f131e91beab2)

# Congrats! Have fun blocking ADs on your devices through a DNS Sinkhole!
