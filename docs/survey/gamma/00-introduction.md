---
title: Introduction
---
# :material-book-open-page-variant: Introduction

Set up the Gamma crystal pack and RadAssist to run gamma radiometric survey jobs in the
field, with Subsoil on the Getac for GPS and guidance. This manual is for Precision Ag
field techs.

!!! info "AT A GLANCE"
    Gamma is always run together with an EM survey. Gather the kit, mount the crystal pack,
    connect the gamma box, put the GPS **into the gamma box**, confirm the data in
    RadAssist, then survey with Subsoil's guidance. At the end of each survey day, copy the
    data off the gamma box with a USB, convert it in RadAssist and export it to the job
    folder. It syncs automatically like the rest of the job.

## What this manual covers

1. Gather and check your equipment.
2. Mount and power the Getac.
3. Mount the crystal pack and gamma box, connect the GPS, and connect in RadAssist.
4. Set up Subsoil and survey the paddock.
5. Copy the data off the gamma box and export it with RadAssist.
6. Pack down properly, the crystal pack is fragile and valuable.

## How the data flows

Crystal pack, to the gamma box, to the Getac, to RadAssist. RadAssist turns the raw data
into a file the GIS team can use. Subsoil does the guidance (swath, speed and the A-B
line) and uses the GPS that the gamma box passes across.

The gamma box records by itself whenever it is powered on. It holds 24 hours and then
records over itself, so the data must be copied off to a USB after **every** survey day.

## Key requirements

!!! danger "SWMS"
    - **Minimise shock to the gamma crystal pack.** It is worth over $100,000. Repairs go
      to Canada and take about six months.
    - **Pack up all equipment at the end of each day** into its boxes to avoid damage
      in transit.
    - **Do not drive with the gamma crystal pack unmounted or unsecured.**
    - **Do not travel over 25 km/h** while the crystal pack is mounted to the vehicle.
    - **Do not survey in the rain**, or until 24 hours after rain has passed.

!!! warning "WARNING"
    - If conducting an elevation survey, ensure the 12V battery has been charged the
      previous night.
    - Confirm the job is staged in **PA Survey - General** by Deal ID before heading out,
      including the **gamma folder**. GIS prepares the boundary, folders and files. If
      anything is missing, contact GIS. Do not create your own.
    - Bring the **Starlink**. You will need it.
      `[CONFIRM: is TeamViewer and a working LTE connection on the Getac still required
      as well?]`
    - Check there is **CORS coverage** at the job. If there is none, you need a second GPS
      configured as a base station. See [Gamma Rig Setup](03-gamma-setup.md#5-gps-and-corrections).

## How to read it

- Each chapter opens with an AT A GLANCE box. It states the one thing to remember.
- Ordered steps are the click-by-click procedure. Follow them in order.
- Screenshots show what you should see on the Getac and in RadAssist at each step.
- Anything written as `[CONFIRM: …]` is not yet finalised. Do not guess. Check with the
  contacts in [Support](07-support.md) first.
