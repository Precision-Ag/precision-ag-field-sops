---
title: Troubleshooting
---
# :material-wrench: Troubleshooting

Quick fixes for the faults that stop a gamma survey. This table is seeded from the
verification cues in the procedure. It will grow as we hit and solve more faults in the
field.

!!! info "AT A GLANCE"
    Most field faults show up as one of the **three green boxes** in RadAssist not
    lighting, or no live data. Give the unit time before assuming it's broken.

## Symptom → likely cause → fix

| Symptom | Likely cause | Fix |
| --- | --- | --- |
| Three green boxes not lit, or no live data in RadAssist | The gamma unit needs time to configure, common after moving a long distance between jobs | Leave the unit connected and check back in a few minutes. See [Gamma Rig Setup](03-gamma-setup.md#8-verify-the-connection). |
| RadAssist won't connect to the RS-602AG | Ignition off, or cabling not seated | Confirm the vehicle ignition is on, re-check the 9-pin and green ethernet connections, then retry **Connect to Device**. |
| Event Log doesn't show "USB HDD Detected" | USB not seated, or a different USB port | Reseat the thumbdrive in the gamma console's USB port and re-check the Event Log. |
| Battery voltage low or elevation survey data missing | 12V battery not charged the night before | Confirm the 12V battery was charged; see [Introduction](00-introduction.md#key-requirements). |
| Exported shapefile isn't showing as synced | Poor LTE signal, or OneDrive hasn't caught up | Check the Getac has a working connection; wait, then confirm the sync-status icon shows "up to date" before packing up. See [Data Collection & Export](04-data-collection.md#5-confirm-it-synced). |
| `[CONFIRM: other common field faults techs have hit with the crystal pack, console, or RadAssist]` | | |

!!! warning "WARNING"
    Don't survey in the rain, or until 24 hours after rain has passed, see
    [Introduction](00-introduction.md).

## Escalation

If the checks above don't resolve it, contact the right person in
[Support](07-support.md) for the type of issue you're hitting.
