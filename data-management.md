---
layout: default
title: Data Management
description: Importing, exporting, and managing your data in Practice!
---

# Data Management

Practice! provides tools to backup, restore, and manage your practice data.

We sync data via iCloud, so you can access your data on any device that has Practice! installed.

Also, you can use import and export to save regular backups of your practice data manually.

## Exporting Data

Exporting creates a backup of all your data that you can restore later or transfer to another device.

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Open Settings</strong>
    <p>Tap the gear icon in the bottom navigation bar.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>Open Backups</strong>
    <p>Scroll to the "iCloud Sync" section and tap "Backups".</p>
</div>

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Under "Move Your Data", tap "Export All Data"</strong>
    <p>This will create a JSON file containing all your tunes, practice sessions, goals, and settings.</p>
</div>

<div class="flow-step">
    <span class="step-number">4</span>
    <strong>Choose where to save</strong>
    <p>Use the share sheet to save the file to Files, email it, or save it to another app.</p>
</div>

<div class="info">
    <strong>What's included in the export:</strong>
    <ul>
        <li>All tunes and their metadata</li>
        <li>Practice sessions and ratings</li>
        <li>Goals and goal completions</li>
        <li>Exercises and exercise practice</li>
        <li>Custom fields</li>
        <li>Traditions and instruments</li>
        <li>Comfort Level settings</li>
    </ul>
</div>

## Importing Data

You can restore data from a previous export or import data from another device.

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Open Backups</strong>
    <p>Navigate to Settings > iCloud Sync > Backups.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>Under "Move Your Data", tap "Restore from File"</strong>
    <p>This opens the file picker.</p>
</div>

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Select the export file</strong>
    <p>Choose the JSON file you previously exported.</p>
</div>

<div class="flow-step">
    <span class="step-number">4</span>
    <strong>Review import results</strong>
    <p>The app will show you what was imported: how many tunes, sessions, etc.</p>
</div>

<div class="info">
    <strong>How merging works.</strong> Restoring adds to what's already on the device rather than replacing it, and it will not overwrite anything:
    <ul>
        <li>Tunes, sessions, exercises and ratings are matched by their internal identity, <em>not</em> by title. Anything already on the device is left exactly as it is and reported as skipped - so restoring the same file twice is harmless, and a tune you've since edited keeps your edits.</li>
        <li>Traditions and instruments are matched by name instead, case-insensitively. That's what stops a file from another device giving you two "Old Time" entries.</li>
    </ul>
    <p>Because titles are never used to match tunes, two different settings of a tune with the same name stay two separate tunes.</p>
</div>

<div class="warning">
    <strong>Before you import:</strong> the app takes an automatic backup immediately beforehand, so there's a way back if the result isn't what you expected.
</div>

## Automatic Backups

You don't have to remember to do any of this. The app backs itself up **every 7 days, and again before any import**, and keeps those backups on the device.

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Open Backups</strong>
    <p>Settings > iCloud Sync > Backups. The "Last Backup" row tells you when the most recent one was taken.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>Tap a backup to restore it</strong>
    <p>The list shows what's available. Tap one and confirm.</p>
</div>

<div class="info">
    Automatic backups live on the device, so they'll get you out of a bad import or a mistaken deletion - but they won't help if you lose the phone. For that, use <strong>Export All Data</strong> and keep the file somewhere else, or rely on iCloud sync.
</div>

## ForScore Import

Practice! can import tunes from ForScore 4SC files.

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Share from ForScore</strong>
    <p>In ForScore, share a 4SC file and select Practice! from the share options.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>Choose an action</strong>
    <p>The "Import from forScore" screen offers two:</p>
    <ul>
        <li><strong>Link to Existing</strong> - attach the forScore score to a tune you already have. You pick the tune.</li>
        <li><strong>Create New</strong> - make a new tune from the forScore metadata.</li>
    </ul>
</div>

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Finish</strong>
    <p>Tap <strong>Link</strong> or <strong>Create</strong> - the button changes to match the action you chose.</p>
</div>

## iCloud Sync

Practice! supports iCloud sync to keep your data synchronized across multiple devices.

### Checking iCloud Status

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Open Settings</strong>
    <p>Navigate to Settings > iCloud Sync.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>View sync status</strong>
    <p>The app displays your iCloud account status:</p>
    <ul>
        <li><strong>Connected</strong> - iCloud is enabled and working</li>
        <li><strong>No iCloud Account</strong> - no iCloud account is signed in on this device</li>
        <li><strong>Restricted</strong> - iCloud is restricted on this device</li>
        <li><strong>Temporarily Unavailable</strong> - iCloud is reachable but not answering right now; usually sorts itself out</li>
        <li><strong>Unknown</strong> - the app couldn't determine the status</li>
    </ul>
</div>

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Check status manually</strong>
    <p>If status is unclear, tap "Check Status" to refresh.</p>
</div>

<div class="info">
    <strong>Note:</strong> iCloud sync requires that iCloud Drive is enabled in your device settings. The sync happens automatically in the background.
</div>

## Deleting All Data

If you need to start fresh, you can delete all data from the app.

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Open Settings</strong>
    <p>Scroll to the very bottom of Settings.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>Tap "Delete All Data"</strong>
    <p>It sits on its own at the foot of the screen, in red.</p>
</div>

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Confirm deletion</strong>
    <p>You'll be asked to confirm. This action cannot be undone.</p>
</div>

<div class="warning">
    <strong>Warning:</strong> Deleting all data will permanently remove all tunes, practice sessions, goals, and settings. Make sure you have exported your data first if you want to keep it.
</div>



