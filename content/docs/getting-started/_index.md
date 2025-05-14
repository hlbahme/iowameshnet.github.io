---
title: Getting Started
weight: 10
description: >
  How to get your device setup so you can get on the mesh!
---

{{< blocks/section type="row" color="white" >}}
{{% blocks/feature icon="fa-walkie-talkie" title="Step 1" %}}
Get your hands on a device

[Read More](#choose-your-device)
{{% /blocks/feature %}}
{{% blocks/feature icon="fa-bolt" title="Step 2" %}}
Flash your device

[Read More](#flash-the-firmware)
{{% /blocks/feature %}}
{{% blocks/feature icon="fa-gears" title="Step 3" %}}
Configure your device

[Read More](#configure-your-device)
{{% /blocks/feature %}}
{{< /blocks/section >}}

## Choose Your Device

In order to use Meshtastic or join in the Iowa Mesh, you will need a device capable of running the Meshtastic firmware.
You should make sure your device includes at least an antenna, a battery if you want to operate portable, and a GPS if you want to share your position.
Some of our favorite starter devices are:

- Ready to go devices:
- Low cost devices: Heltec v3 from [Amazon](https://www.amazon.com/s?k=heltec+v3&crid=Z70PFM8OZVX6&sprefix=heltec+v3%2Caps%2C137&ref=nb_sb_noss_1) or [Rokland](https://store.rokland.com/pages/meshtastic-hardware-rak-lilygo)
- Development kits:

If you would like to explore other options check out our [hardware recommendations](/docs/hardware/radios). Some things to be aware of:

- Some devices are available for multiple frequency bands. The United States requires the 915 MHz band.
- nRF52 based devices are more power efficient than ESP32 based devices so they are better for portable use.
- Most devices do not have a built in GPS. If you are connected to the device with your phone, it can still use your phone's GPS if you want to track position.

## Flash the Firmware

After selecting your device, use the [Meshtastic web flasher](https://flasher.meshtastic.org/) to install the software.
It's quick, straightforward, and backed by excellent documentation.

## Configure Your Device

1. Connect to your device

   Install and open the Meshtastic app on your phone.
   From the main screen click on the connect button to pair with a new device.
   You will need to follow the pairing instructions for your specific device.
   Generally devices without a screen will have a fixed pin like "123456" and devices with a screen will present a pairing code on the screen.

   {{< blocks/section type="row" color="white" >}}
   {{% blocks/feature icon="fa-brands fa-android" title="Android" %}}
   {{< imgproc "pairing-android.png" Resize "400x" >}}
   {{% /blocks/feature %}}
   {{% blocks/feature icon="fa-brands fa-apple" title="Apple iOS" %}}
   {{< imgproc "paring-iphone.png" Resize "400x" >}}
   {{% /blocks/feature %}}
   {{< /blocks/section >}}

1. Set your Lora Region to United States

   {{< blocks/section type="row" color="white" >}}
   {{% blocks/feature icon="fa-brands fa-android" title="Android" %}}
   {{< imgproc "region-android.png" Resize "400x" >}}
   {{% /blocks/feature %}}
   {{% blocks/feature icon="fa-brands fa-apple" title="Apple iOS" %}}
   {{< imgproc "region-iphone.jpg" Resize "400x" >}}
   {{% /blocks/feature %}}
   {{< /blocks/section >}}

1. Name Your Device

   Be Found Easily by naming your device! If you are already a licensed Amateur Radio Operator you can opt to put in your call sign

   {{< blocks/section type="row" color="white" >}}
   {{% blocks/feature icon="fa-brands fa-android" title="Android" %}}
   {{< imgproc "device-name-android.png" Resize "400x" >}}
   {{% /blocks/feature %}}
   {{% blocks/feature icon="fa-brands fa-apple" title="Apple iOS" %}}
   {{< imgproc "device-name.jpg" Resize "500x" >}}
   {{% /blocks/feature %}}
   {{< /blocks/section >}}

1. LoRa Settings

   Currently in Iowa it's a bit sparse for coverage.
   It might be worth turning up for the recommended 3 hops

   Information on [Meshtastic's docs](https://meshtastic.org/docs/configuration/radio/lora/#max-hops).

   If you plan on participating in the meshmap you'll need to turn on Ok to MQTT.
   More information [here](https://meshtastic.org/docs/configuration/radio/lora/#ignore-mqtt).

   {{< blocks/section type="row" color="white" >}}
   {{% blocks/feature icon="fa-brands fa-android" title="Android" %}}
   {{< imgproc "lora-config-android.png" Resize "400x" >}}
   {{% /blocks/feature %}}
   {{% blocks/feature icon="fa-brands fa-apple" title="Apple iOS" %}}
   {{< imgproc "lora-wan-config.jpg" Resize "500x" >}}
   {{% /blocks/feature %}}
   {{< /blocks/section >}}

1. Add Channels for Private configuration

   The Public Channel is available to everyone, but the IROMesh Channel will give us a little better place to communicate among the group.

   Add the channel manually (Case Matters)

   Name: IROMesh
   
   PSK: 7V8jZEvMrVrEXx/c8UekOwE+tSlWaWNffKr6zBtQo/A=
   
   Key Size: 256

## Have Fun

You're now ready to have fun with Meshtastic and the Iowa Mesh!

## Join the Community

Have questions or want to connect? Find us on [Discord](https://discord.gg/jHBywwPJD8) and join the conversation with Iowa Radio Operators!
