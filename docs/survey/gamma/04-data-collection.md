---
title: Data Collection & Export
---
# :material-database-export: Data Collection & Export

Back up the day's data off the gamma console, then load and export it in RadAssist. This
follows on from [Gamma Rig Setup](03-gamma-setup.md). Do this at the end of every
paddock or day.

!!! info "AT A GLANCE"
    USB backup off the console first, then load and export to shapefile in RadAssist,
    straight into the same **Survey Data** folder the EM survey already wrote its CSV
    into. No zip, no email. We don't run gamma without an EM survey on the same job, so
    that folder always exists by the time you export.

## 1. Back up to USB

When the paddock or day is done, place the USB thumbdrive into the gamma console. Go
into the **Event Log** at the bottom of RadAssist and check it says **USB HDD
Detected**, it will then start saving the files.

![USB thumbdrive plugged into the gamma console](img/usb-port-gamma-console.png)
*USB port for the gamma USB, on the console.*

![Event Log showing USB HDD Detected](img/radassist-event-log-usb-detected.png)
*USB HDD Detected (no UBL), the backup has started.*

After waiting 2–3 minutes, the transfer should be complete. The Event Log will say **USB
HDD Backup Done** and **Unmount Usb**, you can now remove the thumbdrive.

![Event Log showing USB HDD Backup Done and Unmount Usb](img/radassist-event-log-backup-done.png)
*Backup done and USB unmounted, safe to remove.*

## 2. Copy the file to today's job folder

Plug the USB thumbdrive into the Getac. Open its files and check the **RSI** folder for
a file named `RSX…_UTC_<date and time in UTC>`, you can also check this under **Date
Modified**.

!!! example
    `RSX272_UTC_20250813_044633` = file from 13 August 2025.

Copy this file into today's job folder on the desktop (see [Getac Setup](02-getac-setup.md)).

![File Explorer showing the RSX UTC folders on the USB](img/usb-port-gamma-console-with-files.png)
*Find today's RSX folder by its UTC timestamp.*

![Copying today's file to the job folder on the desktop](img/rsx-folder-copy-source.png)
*Copy today's file to your job folder on desktop.*

![Confirming the file has landed in today's gamma folder](img/rsx-folder-copy-confirm.png)
*File copied to today's gamma files.*

## 3. Load the data in RadAssist

Open RadAssist and click the **Data Processing** tab. Click **Load**, then **Load Raw
Files Directory**. Navigate to Desktop, find the folder for the current deal, select the
folder you copied from the USB, and press **OK**.

![RadAssist Data Processing tab, Browse For Folder dialog](img/radassist-browse-raw-files-folder.png)
*Data Processing → Load → browse to the copied RSX folder → OK.*

Once loaded, check that **RS-602 System Console** is set as the device type, then click
**Show Loaded Data**.

![RadAssist showing loaded files, ready to show loaded data](img/radassist-show-loaded-data.png)
*Files loaded successfully, confirm device type, then Show Loaded Data.*

## 4. Export to shapefile

Click **Export** in the bottom left.

![Clicking Export in RadAssist](img/radassist-click-export.png)
*Export, bottom left.*

Under **Data range**, select **All data**, then click **Next**.

![Exported Data Range dialog with All data selected](img/radassist-export-data-range.png)
*All data → Next.*

Under **Output format**, select **ESRI Shape File (SHP)**. Under **File Name**, click
the **…** button and browse to the paddock's **Survey Data** folder, the same
`Survey Data\<Paddock> - <date>` folder the EM survey's CSV is already sitting in,
inside the job's folder in **PA Survey - General**. Name the file **date + deal ID +
grower name + gamma export**.

!!! example
    `13-08 1019999 Test Grower gamma export`

`[CONFIRM: exact folder, same Survey Data\<Paddock> - <date> folder as the CSV, or a
sibling location inside it? Confirm with GIS before relying on this.]`

![Export Data Format dialog set to ESRI Shape File](img/radassist-export-format-shp.png)
*Output format: ESRI Shape File (SHP).*

Press **Save**, then **Next** back in RadAssist.

![Exported File Name save dialog](img/radassist-export-filename.png)
*Save with the date + deal ID + grower name + gamma export naming convention.*

Click **Next** through the remaining wizard pages, SHAPE File Export Options, Virtual
Detector Configuration, Ignore Errors, and Filter Samples, leaving the defaults unless
told otherwise, then **Finish**.

<div class="grid cards" markdown>

-   ![SHAPE File Export Options, Virtual Detector Selection](img/radassist-shape-export-options.png)
    Virtual Detector Selection, Next.

-   ![Virtual Detector Configuration](img/radassist-virtual-detector-config.png)
    Virtual Detector Configuration, Next.

-   ![Ignore Errors dialog](img/radassist-ignore-errors.png)
    Ignore Errors, Next.

-   ![Filter Samples dialog](img/radassist-filter-samples.png)
    Filter Samples, Finish.

</div>

Wait for the export to complete.

![RadAssist showing the export in progress](img/radassist-export-in-progress.png)
*Files exporting, wait for this to finish before closing RadAssist.*

## 5. Confirm it synced

That's it, there is no zip and no email. The shapefile is already inside the job's
**PA Survey - General** folder, which syncs automatically. Before you leave, confirm the
`.shp`/`.dbf`/`.shx` files are actually there alongside the EM CSV, and that the sync
status shows "up to date" rather than pending.

`[CONFIRM: screenshot of the Survey Data folder showing both the EM CSV and the gamma
shapefile together, and the OneDrive sync-status icon.]`

!!! warning "WARNING"
    A file that exists locally is not the same as a file GIS can see. If the sync-status
    icon shows pending rather than "up to date" when you're about to leave, wait for it.
    Don't leave the field assuming it synced, see [Troubleshooting](06-troubleshooting.md).

When the job is finished, move the job folder into the **Completed Jobs** folder on the
desktop.

---

Next: [Packup Procedure](05-packup.md). Pack down the rig at the end of the job.
