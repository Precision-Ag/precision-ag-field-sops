---
title: Survey Setup (Subsoil on the Getac)
---
# :material-laptop: Survey Setup (Subsoil on the Getac)

The full click-by-click for setting up and running a DualEM survey in **Subsoil** on the
Getac. Exporting is covered in the next chapter, [Exporting](05-exporting.md), there
isn't much to it, because the GIS team already staged the job folder before you left.

!!! info "AT A GLANCE"
    Scan for equipment, find the job in **PA Survey - General** by Deal ID and Quick
    Start its boundary file, press **Start recording**, drive the paddock, then **Hold
    to stop** when done. Check the scan results before you trust them, a "not found"
    instrument keeps whatever it was last set to, silently.

## 1. Scan for equipment

Open Subsoil (double-click **run.bat**, or your desktop shortcut), then select
**Setup → Scan for equipment**.

![Scan for Equipment dialog scanning ports for GPS and DualEM](img/gear-search-searching.png)
*Scanning ports for GPS, DualEM and EM38, please wait.*

The scan lists what it found on each port, with its evidence, so you don't have to take
its word for it.

![Scan for Equipment dialog showing GPS and DualEM found with evidence](img/gear-search-detected.png)
*Scan complete, check the assignments, then **Apply**.*

!!! note "NOTE"
    An instrument the scan does **not** find keeps its existing manual settings. It is
    not cleared. If GPS or DualEM shows "not found", stop and check cabling and power
    before continuing, see [Troubleshooting](06-troubleshooting.md).

## 2. Find the job and load the boundary

The GIS team stages every job **before you leave**, you don't download, email, or ask
for anything. On the desktop is a shortcut straight into **PA Survey - General**. Open
it and find your paddock's folder by **Deal ID**.

`[CONFIRM: screenshot of the desktop shortcut and the Deal ID folder list in File
Explorer.]`

The boundary file (`.shp`, `.kml` or `.kmz`) sits in that folder already. In Subsoil,
open **Setup**, then select **Quick Start**.

![Setup sheet with the Quick Start row highlighted](img/setup-quick-start.png)
*Setup → **Quick Start** → pick the boundary file from the job's folder.*

Pick that file. The job name, save folder and boundary are all set from it, the save
folder becomes a **Survey Data** subfolder inside the same job folder GIS already
staged, so the CSV lands exactly where GIS expects it without you choosing anything.

![Map showing the loaded paddock boundary before the survey starts](img/map-with-boundary.png)
*The boundary loads onto the map with its area shown in the left-hand panel.*

## 3. Check before you drive

Before pressing Start, confirm the job name in the header matches the paddock you're in,
and that **FIX** in the left-hand panel is not stuck on *Waiting for GPS*.

![Shell ready to start, with the Start recording button highlighted](img/job-start-preflight.png)
*Job loaded, boundary in view. Confirm the details, then **Start recording**.*

## 4. Run the survey

Press **Start recording**. The header switches to **RECORDING**, and the left-hand panel
starts showing live EM and GPS values.

![Shell in RECORDING state with live EM values and a record count](img/lines-logging-coverage.png)
*Recording. **RECORDS** and **ELAPSED** in the top-right confirm data is landing.*

!!! warning "WARNING: SIMULATED DATA"
    If the orange **SIMULATED DATA** pill is showing, the file being written is marked
    as simulated, not real survey data. Confirm your instruments are actually connected
    before you drive.

### Pause and resume

Press **Pause** to hold the survey without ending the job, for a gate, a break, or to
reposition.

![Shell in PAUSED state, with the Resume button highlighted](img/survey-pause.png)
*Paused. No data is logged while paused.*

Press **Resume** to continue recording into the same file.

![Shell back in RECORDING state after Resume](img/survey-resume.png)
*Resumed, recording continues into the same CSV.*

## 5. End the job

When the paddock is finished, **hold** the **Hold to stop** button until it fills. This
is deliberate, a mistap here costs a re-drive, so a quick tap does nothing.

![Shell in STOPPED state, data saved](img/end-job.png)
*Stopped, data saved. The record count and save path are shown top-left.*

---

Next: [Exporting](05-exporting.md). Confirm the data reached the GIS team, there's
nothing to actually export.
