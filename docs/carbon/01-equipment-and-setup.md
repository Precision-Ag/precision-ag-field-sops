---
title: Equipment and App Setup
---
# :material-cellphone-cog: Equipment and App Setup

All carbon sampling is completed using ArcGIS Field Maps and Survey123 for in-field data
capture, plus ArcGIS QuickCapture for audit data. This keeps data quality and integrity
consistent and is critical for AgriProve's downstream systems to work.

!!! info "AT A GLANCE"
    Set up and test Field Maps, Survey123 and QuickCapture before you mobilise. A setup
    problem discovered in the paddock costs a lot more time than one caught in the
    office.

## Before you leave

1. Download ArcGIS Field Maps, ArcGIS Survey123 and ArcGIS QuickCapture from your
   device's app store.
2. Get your ArcGIS username and password from the AgriProve GIS administrator.

## Field Maps and Survey123 setup

1. Open both apps and log in with the supplied credentials.
2. In Survey123, go to **Download Surveys** and download the
   `AgriProve_Soil_Sampling_Survey` form.
3. Pair a Bluetooth connection with the GPS system you are using (see
   [Locating Sampling Points](02-locating-sampling-points.md) for the accuracy
   requirement).
4. Open **Settings** and confirm **Location** is set to the paired GPS system, not
   **Integrated Provider**.

!!! warning "WARNING"
    Integrated Provider is the device's own built-in GPS. It does not meet the accuracy
    requirement for this protocol. If Location is showing Integrated Provider, the GPS
    receiver is not correctly paired, fix this before sampling.

5. Leave all other Survey123 settings as default unless instructed otherwise. Close
   Survey123 and open Field Maps.
6. Tap the Profile button, then **Location**, then **Provider**. Select your paired GPS
   device's location profile using GDA2020, MGA zone (EPSG 7844 family).
7. Under **General Settings**, confirm units are set to metres. Exit Profile.
8. Download the relevant soil sampling map from the **Offline Map** list (there should
   only be one map available per project).

## QuickCapture setup

1. Open QuickCapture and log in with the same credentials used for Field Maps and
   Survey123.

Full setup and use of QuickCapture for audit data is covered in
[QuickCapture Audit Data](05-quickcapture-audit-data.md).

!!! tip "TIP"
    Test all three apps, including a live GPS fix, before you drive out. Fixing a login
    or pairing issue on a paddock with no signal wastes a field day.
