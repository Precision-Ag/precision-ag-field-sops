---
title: Survey Setup (Subsoil on the Getac)
---
# :material-laptop: Survey Setup (Subsoil on the Getac)

The full click-by-click for setting up and running an EM38 survey in **Subsoil** on the
Getac, once the EM38 is calibrated (see [Calibration](04-calibration.md)). Exporting is
covered in the next chapter, [Exporting](06-exporting.md).

!!! info "AT A GLANCE"
    The core flow — scan for equipment, load the boundary, start/pause/resume/stop — is
    identical to the [DualEM Subsoil chapter](../dualem/04-survey-setup.md). This
    chapter covers that same flow plus the two things that are EM38-only: the
    **calibration line** and the **4-hour recal countdown**.

## Before you start

- [ ] EM38 calibrated for today / this location (see [Calibration](04-calibration.md))
- [ ] GPS connected and reading
- [ ] Boundary imported

## 1. Scan for equipment, load the boundary, run the survey

This part of Subsoil is identical for every instrument — the same scan, the same
Quick Start boundary load, the same Start/Pause/Resume/Stop. Rather than duplicate it
here, follow the [DualEM Subsoil chapter](../dualem/04-survey-setup.md) steps 1 through
5 exactly, then come back here for the two EM38-only steps below.

`[CONFIRM: once both books are reviewed, decide whether to keep this as a cross-link or
embed the DualEM steps directly — a field tech flipping between two chapters mid-survey
might be worse than the duplication.]`

## 2. Set the calibration line

Open **Guidance**. The EM38 gets an extra **Calibration line** section that a DualEM
survey never shows — DualEM self-calibrates, EM38 doesn't.

![Guidance sheet showing the Calibration line section, Set Cal A highlighted](img/calibration-line-section.png)
*Calibration line is a stretch of ground you drive back to every four hours, not a
point — the countdown lives in the top bar, not here.*

Press **Set Cal A** at one end of a known stretch of ground.

![Guidance sheet showing Set Cal B after the first point is dropped](img/calibration-line-set-a.png)
*Point A is set. Drive to the other end, then press **Set Cal B**.*

Press **Set Cal B** at the other end. The line is now complete and saved to the job
folder — pressing the button again starts a **New Cal Line** instead.

![Guidance sheet showing New Cal Line once both ends are set](img/calibration-line-complete.png)
*Line complete. Come back to drive this same stretch at every recalibration.*

!!! note "NOTE"
    Setting a complete line is what saves it. Nothing else needs to be pressed. If you
    replace an existing line, Subsoil asks you to hold to confirm first — the old line
    is what the job has been calibrated against since day one.

## 3. Watch the recal countdown

Once the calibration line is set, the header shows a **NEXT CAL** countdown.

![Shell header showing the NEXT CAL countdown timer](img/recal-countdown.png)
*NEXT CAL counts down from four hours. It reads "—" if no line has been set yet.*

!!! danger "SWMS"
    A wrongly-nulled or overdue EM38 gives readings that look completely plausible but
    are wrong — there is no error message to catch it. Do not let **NEXT CAL** reach
    zero mid-paddock. Drive back to the calibration line, re-null the EM38 (see
    [Calibration](04-calibration.md)), then set a fresh cal line before continuing.

---

Next: [Exporting](06-exporting.md). Get the data off the Getac and to the GIS team.
