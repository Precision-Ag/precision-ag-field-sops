---
title: Equipment Setup (Polaris)
---
# :material-motorbike: Equipment Setup (Polaris)

How to mount, wire and power the EM38 rig on the **Polaris** before you start a survey.

!!! info "AT A GLANCE"
    The EM38 sits in its cradle with the cable coming out, and the cable is secured to
    the cradle with cable ties, tape or velcro. Keep metal away from the unit. Cables
    break easily on brush, so route them clear. Connect by cable (wired is the standard),
    put the GPS on the roof, and let Subsoil find the equipment.

!!! danger "SWMS"
    Handle all equipment with care. Check the EM38, cables, cradle and GPS for damage
    before use. Do not use damaged equipment, contact support.

## Before you start: warm up the EM38

Take the EM38 out of its case **first**, place it away from any metal, and let it warm
up while you set up the rest of the rig. Then calibrate it, see
[Calibration](04-calibration.md). A wrongly nulled EM38 gives readings that look
plausible but are wrong.

!!! warning "WARNING"
    Remove the 9V battery from the EM38 after each use and reinstall it before your next
    use. Leaving it in flattens it between jobs.

## Mounting the EM38 in the cradle

Your Polaris is already fitted with a EM38 cradle (see [Equipment Required](01-equipment-needed.md)).


1. Place the EM38 in the cradle. `[CONFIRM: does the EM38 have an orientation requirement in the cradle?]`
2. Keep metal away from the EM38, including from your hands, wrists, pockets and neck
   while you handle it. Calibrate with the whole rig attached, see [Calibration](04-calibration.md).
3. Secure the EM38 in the cradle so it cannot move, with its cable coming out of the
   cradle.

## Securing the cable

1. Secure the cable to the cradle using **cable ties, tape or velcro**. Do not use metal
   fixings.
2. Route the cable so it cannot snag on brush, the tow frame or the wheels, and so it is
   not pulled tight when the vehicle turns.
3. Keep the cable away from the Polaris wheels and tow frame.

!!! warning "WARNING"
    Cables are easy to break on brush. A loose or hanging cable is the most likely thing
    to fail, so check it before every survey.

## Power

1. Connect power to the EM38 using the Polaris's **integrated power source**.
2. If there is no integrated power, use a 12V battery with the **Anderson-to-alligator-clamp**
   lead, and place it in its holder.

## Connecting to the Getac

1. Plug the EM38's Power & Data cable (**DB9** end) into a **DB9 to USB** cable.
2. Plug the USB end into **any USB port** on the Getac. It does not matter which one,
   Subsoil finds the equipment itself.
3. Wait several seconds for Windows to recognise the device.
4. Leave the cable connected for the entire survey.

!!! note "NOTE, wired is the standard"
    Wired is the standard connection. Newer equipment can run wirelessly if the digital
    team has confirmed it. They do all the settings, so there is nothing to change on the
    Getac. Do not change the settings yourself. Subsoil's **Scan for equipment** is best
    practice, there is a manual COM port option in Settings but only use it if support
    tells you to.

## GPS and corrections

Both **Emlid** and **Ag Leader** GPS units are used.

1. Mount the GPS on the **roof of the Polaris**. On the Polaris this is the metal plate. The Ag Leader power comes from the Anderson plug in the back tray.
2. Emlid: switch it on, powered from the portable charger bank via USB-C. Ag Leader:
   connect the antenna and its power.
3. Plug the GPS cable (**DB9** end) into the second **DB9 to USB** cable, then plug the
   USB end into any USB port on the Getac.
4. Secure the GPS cable with cable ties, tape or velcro so it cannot snag.

- **Emlid:** it connects to the **CORS network** to get its corrections. Check it shows
  connected before you start.
  `[CONFIRM: how the Emlid reaches the CORS network in the field (Starlink or a hotspot) and
  what the tech checks to see it is connected.]`
- **No CORS coverage:** you need a **second GPS configured as a base station**.
  `[CONFIRM: how the base station is set up, who configures it, and whether the Ag Leader
  uses CORS or the base.]`

When you survey, the green **RTK FIX** in Subsoil confirms the GPS has its corrections.

## Pre-drive checklist

- [ ] EM38 seated and secured in the cradle, no metal nearby
- [ ] Cable secured to the cradle and routed clear of brush
- [ ] Power connected
- [ ] EM38 cable connected to the Getac
- [ ] GPS on the roof, switched on, cable connected and secured
- [ ] CORS coverage checked, or the second GPS packed as a base station
- [ ] EM38 warmed up and calibrated (see [Calibration](04-calibration.md))
- [ ] 9V battery fitted, and spares packed