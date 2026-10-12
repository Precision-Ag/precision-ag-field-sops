---
title: Troubleshooting
---
# :material-wrench: Troubleshooting

Quick fixes for the faults that stop a gamma survey. This table is seeded from the
verification cues in the procedure. It will grow as we hit and solve more faults in the
field.

!!! info "AT A GLANCE"
    Most field faults show up as one of the **three green boxes** in RadAssist not
    lighting, or no live data. Check the **Getac cradle has power** first. Give the unit
    time before assuming it's broken.

## Symptom → likely cause → fix

| Symptom | Likely cause | Fix |
| --- | --- | --- |
| No live data in RadAssist | **Getac cradle not powered.** An unpowered cradle will not pass on the gamma data. This is the most common cause. | Plug the power into the **bottom of the cradle**, not the Getac. See [Getac Setup](02-getac-setup.md). |
| No live data in RadAssist | **IPv6 is turned on** on the Getac | Turn IPv6 off. If you are not sure how, contact Brandon. |
| Three green boxes not lit, or no live data | The gamma unit needs time to configure, common after moving a long distance between jobs | Leave the unit connected and check back in a few minutes. See [Gamma Rig Setup](03-gamma-setup.md#7-verify-the-connection). |
| RadAssist won't connect to the RS-602AG | Ignition off, or cabling not seated | Confirm the vehicle ignition is on, re-check the green data cable and the grey cable, then retry **Connect to Device**. |
| Alarm for no GPS | GPS not plugged into the gamma box, or the rover has no fix | Check the rover cable is in the **gamma box**, not the Getac. Check Subsoil shows the green RTK FIX. |
| No RTK FIX with an Emlid | Not connected to the CORS network | `[CONFIRM: what to check and how to reconnect.]` |
| No RTK FIX and no CORS coverage | No base station | Set up the second GPS as a base station. `[CONFIRM: steps.]` |
| Data cable damaged | Cable broken in the brush or pinched | The gamma box **still records** on its own. Connect the GPS to Subsoil using the **TCP** option and carry on. Contact Brandon. |
| Event Log doesn't show "USB HDD Detected" | USB not seated, or a different USB port | Reseat the thumbdrive in the gamma box's USB port and re-check the Event Log. |
| Battery voltage low or elevation survey data missing | 12V battery not charged the night before | Confirm the 12V battery was charged; see [Introduction](00-introduction.md#key-requirements). |
| Exported shapefile isn't showing as synced | Poor signal, or OneDrive hasn't caught up | Check the Getac has a working connection; wait, then confirm the sync-status icon shows "up to date" before packing up. See [Data Collection & Export](04-data-collection.md#6-confirm-it-synced). |

!!! warning "WARNING"
    Don't survey in the rain, or until 24 hours after rain has passed, see
    [Introduction](00-introduction.md).

## Escalation

If the data stream is still not flowing after the checks above, contact **Brandon**. He
can get it going. For anything else, contact the right person in
[Support](07-support.md) for the type of issue you're hitting.
