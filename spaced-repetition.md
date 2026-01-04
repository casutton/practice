---
layout: default
title: Spaced Repetition
description: Understanding the spaced repetition system in FolkTunesApp
---

# Spaced Repetition

FolkTunesApp uses a spaced repetition system based on the Leitner method to help you learn tunes more effectively. The system organizes tunes into "buckets" and schedules reviews based on how well you know each tune.

## How It Works

When you rate a tune after practicing, the app moves it to a different bucket. Each bucket has a different review interval, determining when the tune will appear again.

### Rating to Bucket Movement

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Rate a tune</strong>
    <p>After practicing, you rate the tune as Difficult, Good, or Easy.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>Bucket assignment</strong>
    <p>Based on your rating, the tune moves to a different bucket:</p>
    <ul>
        <li><strong>Difficult</strong> → Moves to "Next Session" bucket (Bin 0)</li>
        <li><strong>Good</strong> → Moves up one bucket</li>
        <li><strong>Easy</strong> → Moves up one bucket</li>
    </ul>
</div>

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Next review date</strong>
    <p>The app calculates when the tune should be reviewed again based on the bucket's interval.</p>
</div>

<div class="screenshot placeholder">
    <div class="caption">Screenshot: Tune detail view showing current bucket and next review date</div>
</div>

## The Bucket System

The app uses five buckets with increasing review intervals:

### Bucket 0: Next Session
- **Default interval:** 1 day
- **Purpose:** Tunes that need immediate review
- **When tunes are here:** After rating a tune as "Difficult"

<div class="screenshot placeholder">
    <div class="caption">Screenshot: Bucket settings showing "Next Session" configuration</div>
</div>

### Bucket 1: Next Week
- **Default interval:** 3 days
- **Purpose:** Tunes that are progressing well
- **When tunes are here:** After rating a tune as "Good" from Bucket 0

### Bucket 2: Next Month
- **Default interval:** 7 days
- **Purpose:** Tunes that are well-learned
- **When tunes are here:** After rating a tune as "Good" or "Easy" from lower buckets

### Bucket 3: Occasional
- **Default interval:** 14 days
- **Purpose:** Tunes that are mastered
- **When tunes are here:** After consistently rating a tune as "Good" or "Easy"

### Bucket 4: Mastered
- **Default interval:** 30 days
- **Purpose:** Tunes you know very well
- **When tunes are here:** After consistently rating a tune as "Easy"

## Customizing Bucket Intervals

You can customize how long each bucket waits before review.

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Open Settings</strong>
    <p>Tap the gear icon in the bottom navigation bar.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>Navigate to Bucket Settings</strong>
    <p>In the "Practice Settings" section, tap "Configure Bucket Intervals".</p>
</div>

<div class="screenshot placeholder">
    <div class="caption">Screenshot: Settings screen showing "Configure Bucket Intervals" option</div>
</div>

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Adjust intervals</strong>
    <p>For each bucket, set the number of days before the next review. You can use the slider or enter a value directly.</p>
</div>

<div class="screenshot placeholder">
    <div class="caption">Screenshot: Bucket settings screen with interval sliders</div>
</div>

<div class="flow-step">
    <span class="step-number">4</span>
    <strong>Save changes</strong>
    <p>Tap "Save" to apply the new intervals. Changes apply to all future practice sessions.</p>
</div>

<div class="info">
    <strong>Note:</strong> Existing tunes will continue using their current bucket assignments until their next review. New intervals only affect tunes after they are rated again.
</div>

## Viewing Tune Bucket Status

You can see which bucket a tune is in and when it's due for review.

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Open a tune</strong>
    <p>From the Tunes tab, tap on any tune to view its details.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>View bucket information</strong>
    <p>The tune detail view shows the current bucket and next review date.</p>
</div>

<div class="screenshot placeholder">
    <div class="caption">Screenshot: Tune detail view with bucket and next review information</div>
</div>

## How Tunes Are Selected for Practice

When you start a practice session, the app suggests tunes based on:

1. **Due for review** - Tunes whose next review date has passed
2. **Bucket priority** - Tunes in lower buckets (that need more practice) appear first
3. **Recent practice** - Tunes you haven't practiced recently

<div class="screenshot placeholder">
    <div class="caption">Screenshot: Practice view showing suggested tunes with bucket indicators</div>
</div>

## Understanding the Algorithm

The spaced repetition algorithm works as follows:

1. **New tunes** start in Bucket 0 (Next Session)
2. **Rating "Difficult"** always moves a tune back to Bucket 0, regardless of current bucket
3. **Rating "Good"** moves a tune up one bucket
4. **Rating "Easy"** moves a tune up one bucket
5. **Review timing** is calculated from the last practice date plus the bucket's interval

<div class="tip">
    <strong>Best Practice:</strong> Be honest with your ratings. The system works best when you accurately assess how well you know each tune. Rating something as "Difficult" when you struggle helps ensure you practice it more frequently.
</div>

## Resetting a Tune's Bucket

If you want to reset a tune's bucket status (for example, if you haven't played it in a long time):

<div class="flow-step">
    <span class="step-number">1</span>
    <strong>Open the tune</strong>
    <p>Navigate to the tune's detail view.</p>
</div>

<div class="flow-step">
    <span class="step-number">2</span>
    <strong>Practice the tune</strong>
    <p>Practice it and rate it as "Difficult" to move it back to Bucket 0.</p>
</div>

<div class="info">
    <strong>Alternative:</strong> You can also edit the tune's spaced repetition data directly if needed, though this is not recommended for normal use.
</div>

