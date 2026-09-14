---
title: Exporting
---
# :material-database-export: Exporting

Get the completed EM38 survey off the Getac and confirm it has reached the GIS team.
This follows on from [Survey Setup](05-survey-setup.md).

!!! info "AT A GLANCE"
    Open **Files → Export**, confirm the point count and CSV path, choose the
    coordinate system, then **Export Shapefile**. The job folder is synced to
    SharePoint by OneDrive — there is no manual upload step, but the Getac needs a
    working internet connection for that sync to happen.

## 1. Export the shapefile

Once the survey is stopped, open **Files → Export**.

![Export dialog showing the survey CSV, output folder and coordinate system](img/export-dialog.png)
*Confirm the point count and CSV path, choose the coordinate system
(defaults to **GDA2020 / MGA Zone 55**), then **Export Shapefile**.*

`[CONFIRM: screenshot of the export-complete state, same gap as the DualEM chapter.]`

## 2. Confirm it reached the GIS team

The CSV and shapefile both save into the job's folder under **Survey Data**, inside the
same SharePoint job folder Quick Start loaded the boundary from. OneDrive syncs that
folder automatically — there is no separate "send to GIS" step.

!!! warning "WARNING — no wifi, no sync"
    The Getac needs a real internet connection for OneDrive to actually push the files
    up. Paddock wifi/mobile coverage is often not good enough. If you finish a job out
    of range, the data is still safe on the Getac's disk — connect it to a decent
    connection (back at the depot, home, wherever) as soon as you can, and don't
    consider the job delivered until the folder shows "up to date", not sync-pending.

!!! warning "WARNING"
    Do not leave the field assuming the sync worked if you haven't checked. If the job
    folder shows a sync-pending icon rather than "up to date", see
    [Troubleshooting](07-troubleshooting.md) before you pack up.
