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
    <strong>Navigate to Data Management</strong>
    <p>Scroll to the "Data Management" section.</p>
</div>

![Settings screen showing Data Management section]({{ '/assets/images/settings-data-management.png' | relative_url }})

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Tap "Export All Data"</strong>
    <p>This will create a JSON file containing all your tunes, practice sessions, goals, and settings.</p>
</div>

<div class="flow-step">
    <span class="step-number">4</span>
    <strong>Choose where to save</strong>
    <p>Use the share sheet to save the file to Files, email it, or save it to another app.</p>
</div>

![Share sheet for exporting data]({{ '/assets/images/export-share-sheet.png' | relative_url }})

<div class="info">
    <strong>What's included in the export:</strong>
    <ul>
        <li>All tunes and their metadata</li>
        <li>Practice sessions and ratings</li>
        <li>Goals and goal completions</li>
        <li>Exercises and exercise practice</li>
        <li>Practice plans</li>
        <li>Custom fields and field visibility settings</li>
        <li>Genres and instruments</li>
        <li>Bucket settings</li>
    </ul>
</div>

## Importing Data

You can restore data from a previous export or import data from another device.

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Open Settings</strong>
    <p>Navigate to Settings > Data Management.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>Tap "Import Data"</strong>
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

![Import results screen]({{ '/assets/images/import-results.png' | relative_url }})

<div class="warning">
    <strong>Important:</strong> Importing data will merge with your existing data. Tunes with the same title may be updated. Make sure you have a recent backup before importing.
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
    <strong>Choose import option</strong>
    <p>You can either:</p>
    <ul>
        <li><strong>Associate with existing tune</strong> - Link the ForScore file to a tune already in your library</li>
        <li><strong>Create new tune</strong> - Create a new tune from the ForScore metadata</li>
    </ul>
</div>

![ForScore import options screen]({{ '/assets/images/forscore-import-options.png' | relative_url }})

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Complete the import</strong>
    <p>Fill in any additional tune information and tap "Import".</p>
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
        <li><strong>Available</strong> - iCloud is enabled and working</li>
        <li><strong>No Account</strong> - No iCloud account is signed in</li>
        <li><strong>Restricted</strong> - iCloud is restricted on this device</li>
        <li><strong>Could Not Determine</strong> - Unable to check status</li>
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
    <p>Navigate to Settings > Data Management.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>Tap "Delete All Data"</strong>
    <p>This is a destructive action, so it's in red text.</p>
</div>

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Confirm deletion</strong>
    <p>You'll be asked to confirm. This action cannot be undone.</p>
</div>

<div class="warning">
    <strong>Warning:</strong> Deleting all data will permanently remove all tunes, practice sessions, goals, and settings. Make sure you have exported your data first if you want to keep it.
</div>



