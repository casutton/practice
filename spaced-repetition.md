---
layout: default
title: Spaced Repetition
description: Understanding the spaced repetition system in FolkTunesApp
---

# Spaced Repetition

**Why spaced repetition works:** Research shows that you remember things better when you practice them right before you're about to forget them. Instead of practicing the same tunes every day (which wastes time on tunes you already know), spaced repetition schedules practice at the optimal time - when it will do the most good.

Practice! uses a spaced repetition system based on the Leitner method to help you learn tunes more effectively. The system organizes tunes into "buckets" and schedules reviews based on how well you know each tune. This means you spend more time on tunes that need work, and less time on tunes you've already mastered.

## How It Works

**The basic idea:** When you rate a tune after practicing, the app moves it to a different bucket. Each bucket has a different review interval - tunes in lower buckets (that you know less well) appear again soon, while tunes in higher buckets (that you know well) appear less frequently. This way, the app automatically focuses your practice on what needs the most work.

When you rate a tune after practicing, the app moves it to a different bucket. Each bucket has a different review interval, determining when the tune will appear again. The better you know a tune, the longer the interval before it appears again.

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

![Tune detail view showing current bucket and next review date]({{ '/assets/images/tune-detail-view.png' | relative_url }})

## The Bucket System

The app uses four buckets with increasing review intervals:

### Bucket 0: Next Session
- **Default interval:** 1 day
- **Purpose:** Tunes that need immediate review
- **When tunes are here:** After rating a tune as "Difficult"

![Bucket settings showing Next Session configuration]({{ '/assets/images/bucket-settings-intervals.png' | relative_url }})

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
- **Purpose:** Tunes you know very well
- **When tunes are here:** After consistently rating a tune as "Good" or "Easy"

## Customizing Bucket Intervals

**Why customize:** The default intervals work well for most people, but you might want to adjust them based on how often you practice or how quickly you learn. If you practice every day, shorter intervals might work better. If you practice less frequently, you might want longer intervals so tunes don't pile up.

You can customize how long each bucket waits before review. This lets you tailor the system to your practice schedule and learning style.

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

![Bucket settings screen with interval sliders]({{ '/assets/images/bucket-settings-intervals.png' | relative_url }})

<div class="flow-step">
    <span class="step-number">3</span>
    <strong>Adjust intervals</strong>
    <p>For each bucket, set the number of days before the next review. You can use the slider or enter a value directly.</p>
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


## How Tunes Are Selected for Practice

When you are choosing a tune, you can use the tune picker to find the tunes that are due for review. 

<p><img src="/practice/assets/images/tune-picker-with-search.png" alt="Tune picker screen with search and filter options" /></p>

Pressing the clock icon will show you the tunes that are due for review.

This is just a guideline to help you. Of course feel free to play whatever you like!


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

