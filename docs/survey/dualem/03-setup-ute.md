---
title: Equipment Setup (Ute)
---
# :material-truck: Equipment Setup (Ute)

How to mount, wire and power the DualEM rig on the **ute** before you start a survey.

!!! info "AT A GLANCE"
    The DualEM sits in its cradle with the cable coming out, and the cable is secured to
    the cradle with cable ties, tape or velcro. Keep metal away from the unit. Cables
    break easily on brush, so route them clear. Connect by cable (wired is the standard),
    put the GPS on the roof, and let Subsoil find the equipment.

!!! danger "SWMS"
    Handle all equipment with care. Check the DualEM, cables, cradle and GPS for damage
    before use. Do not use damaged equipment, contact support.

## Mounting the DualEM in the cradle

Your ute is already fitted with a DualEM cradle (see [Equipment Required](01-equipment-needed.md)).


1. Place the DualEM in the cradle. The arrow faces **down**.
2. Keep metal away from the DualEM, including from your hands, wrists, pockets and neck
   while you handle it. The DualEM must be **1.5m from any metal**.
3. Secure the DualEM in the cradle so it cannot move, with its cable coming out of the
   cradle.

## Securing the cable

1. Secure the cable to the cradle using **cable ties, tape or velcro**. Do not use metal
   fixings.
2. Route the cable so it cannot snag on brush, the tow frame or the wheels, and so it is
   not pulled tight when the vehicle turns.
3. Route cables through the passenger window so the door cannot pinch them.

!!! warning "WARNING"
    Cables are easy to break on brush. A loose or hanging cable is the most likely thing
    to fail, so check it before every survey.

## Power

1. Connect power to the DualEM using the ute's **integrated power source**.
2. If there is no integrated power, use a 12V battery with the **Anderson-to-alligator-clamp**
   lead, and place it in its holder.
3. Allow 20-40 seconds for the DualEM to fully boot.
   `[CONFIRM: older notes also said to let the DualEM self-calibrate for 20 minutes in its cradle. Is that still needed?]`

## Connecting to the Getac

1. Plug the DualEM's Power & Data cable (**DB9** end) into a **DB9 to USB** cable.
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

1. Mount the GPS on the **roof of the ute**.
2. Emlid: switch it on, powered from the portable charger bank via USB-C. Ag Leader:
   connect the antenna and its power.
3. Plug the GPS cable (**DB9** end) into the second **DB9 to USB** cable, then plug the
   USB end into any USB port on the Getac.
4. Secure the GPS cable with cable ties, tape or velcro so it cannot snag.

- **Emlid:** it reaches the **CORS network** for its corrections. About 90% of jobs are
  inside CORS coverage. Check the green **RTK FIX** shows in Subsoil before you start. If
  you lose contact with CORS, contact Brandon.
- **Elevation survey outside CORS:** you need a **base station**. Set up another Emlid or
  an Ag Leader as the base and give it a power source. Put it on a clear high point. It
  connects to the rover by **LoRa** to provide the elevation. A base station is only
  needed for elevation.
  `[CONFIRM: the base station setup steps, and how the Ag Leader gets its corrections.]`

Bring a **Starlink** when doing any surveying. LTE works in a pinch, but it is very slow
and drops out.

## Pre-drive checklist

- [ ] DualEM seated and secured in the cradle, no metal nearby
- [ ] Cable secured to the cradle and routed clear of brush
- [ ] Power connected
- [ ] DualEM cable connected to the Getac
- [ ] GPS on the roof, switched on, cable connected and secured
- [ ] Starlink packed
- [ ] Within CORS coverage, or a base station packed for an elevation survey
- [ ] Allowed the DualEM time to boot (and self-calibrate if required)