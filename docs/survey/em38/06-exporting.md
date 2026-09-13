---
title: Exporting
---
# :material-database-export: Exporting

Get the completed EM38 survey off the Getac and confirm it has reached the GIS team.
This follows on from [Survey Setup](05-survey-setup.md). The export mechanics are the
same Subsoil dialog as the DualEM workflow — see the
[DualEM Exporting chapter](../dualem/05-exporting.md) for the fuller version of this
page.

!!! info "AT A GLANCE"
    Open **Files → Export**, confirm the point count and CSV path, choose the
    coordinate system, then **Export Shapefile**. The job folder is synced by
    OneDrive — there is no manual upload step, but confirm it's actually syncing
    before you leave.

## 1. Export the shapefile

Once the survey is stopped, open **Files → Export**.

![Export dialog showing the survey CSV, output folder and coordinate system](img/export-dialog.png)
*Confirm the point count and CSV path, choose the coordinate system
(defaults to **GDA2020 / MGA Zone 55**), then **Export Shapefile**.*

`[CONFIRM: screenshot of the export-complete state, same gap as the DualEM chapter.]`

## 2. Confirm it reached the GIS team

The CSV and shapefile both save into the job's folder under **Survey Data**, which
OneDrive syncs automatically.

!!! warning "WARNING"
    Do not leave the field assuming the sync worked if you haven't checked. If the job
    folder shows a sync-pending icon rather than "up to date", see
    [Troubleshooting](07-troubleshooting.md) before you pack up.
