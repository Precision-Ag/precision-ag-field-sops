---
title: Exporting
---
# :material-database-export: Exporting

There is nothing to export. This follows on from [Survey Setup](04-survey-setup.md).

!!! info "AT A GLANCE"
    Subsoil writes the CSV directly into the job folder GIS already staged, as you
    drive, not at the end, not on a button press. There is no zip, no email, and no
    "Export" step for DualEM/EM38 data. Just confirm the file is there before you pack
    up.

## Where the data actually goes

The job folder lives under **PA Survey - General → `<Deal ID> - <Client>`**, the same
folder you opened in [Survey Setup](04-survey-setup.md#2-find-the-job-and-load-the-boundary)
to Quick Start the boundary. Subsoil creates a **Survey Data** subfolder inside it, and
inside that, one folder per paddock per day:

```
PA Survey - General
└── <Deal ID> - <Client Name>
    ├── <paddock boundary file>.kml
    └── Survey Data
        └── <Paddock> - <date>
            └── <Paddock>_<timestamp>.csv
```

This folder is inside the OneDrive/SharePoint sync GIS already set up on the Getac.
That's the whole point of the pre-staged job folder. Nothing needs sending. The CSV
lands there live, during the survey, so the file already exists (and is growing) while
you're still driving.

## Confirm it landed

Before you leave the paddock, open the job's **Survey Data** folder and check today's
paddock folder has a CSV in it with a recent modified time.

`[CONFIRM: screenshot of the Survey Data folder showing a real CSV, and how to read the
OneDrive sync-status icon on the Getac to confirm it's actually synced rather than just
saved locally.]`

!!! warning "WARNING"
    A file that exists locally is not the same as a file GIS can see. If the sync-status
    icon shows pending rather than "up to date" when you're about to leave, wait for it.
    See [Troubleshooting](06-troubleshooting.md).

!!! note "NOTE"
    Subsoil does have its own **Files → Export** dialog that can write a shapefile
    locally. It is not part of the normal field workflow, GIS works from the CSV.
    `[CONFIRM: is there any real scenario a field tech should use this, or should it be
    left out of the SOP entirely?]`
