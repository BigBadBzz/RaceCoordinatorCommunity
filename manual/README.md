> **Download from Race Coordinator website                              
>  [<u>https://racecoordinator.net/download.html</u>](https://racecoordinator.net/download.html)                          **<img src=".\/media/image90.jpg"
> style="width:6.83895in;height:4.07969in" />
>
> **Race Coordinator is a free alternative slot car lap counting
> software package for the PC. It contains a wide range of racing
> options from the most basic Round Robin races to the most complicated
> multi-race events that include Practice time, one or more Qualifying
> races, and a Finals.**
>
> **Race Coordinator supports an unlimited number of drivers per race
> and an unlimited number of lanes on the track. Race Coordinator also
> provides an impressive list of features that will accommodate the
> smallest basement races to the largest club races.**

###### Race Coordinator User Manual

> © 2026 by Dave Aufderheide. All Rights Reserved. This document was
> created by the Race Coordinator community using Google Docs and edited
> by Paul Linton.
>
> Typefaces are from the open source Source® Sans, Source Serif and
> Source Code Pro families created by Adobe and licensed under the SIL
> Open Font License (OFL).
>
> Some images were created in total or in part with Fritzing.

###### Notice of liability

> The content of this guide is provided for informational use only and
> is supplied without warranty. The writer of this guide does not accept
> any liability to any person or entity with respect to any loss or
> damage caused or alleged to be caused by the instructions in this
> guide.

###### Trademarks

> “Serif” and “Affinity” are registered trademarks of Serif (Europe)
> Ltd.
>
> Microsoft and Windows are either registered trademarks or trademarks
> of Microsoft Corporation registered in the U.S. and other countries.
>
> All other trademarks are the property of their respective owners.

Table of Contents

[**Introduction 1**](#introduction)

> [Introduction to Race Coordinator
> 1](#introduction-to-race-coordinator)
>
> [Track Interface/Sensor Support 1](#track-interfacesensor-support)
>
> [Features 1](#features)
>
> [Easy Race Setup 2](#easy-race-setup)
>
> [Purpose 2](#purpose)
>
> [Scope 3](#scope)
>
> [Support / Further Resources 3](#support-further-resources)

[**System Overview 4**](#system-overview)

> [System Architecture 4](#system-architecture)
>
> [Hardware Requirements 4](#hardware-requirements)
>
> [Software Requirements 4](#software-requirements)

[**Installation 6**](#installation)

> [Hardware Installation 6](#hardware-installation)
>
> [Software Installation 6](#software-installation)
>
> [Download Race Coordinator Software
> 6](#download-race-coordinator-software)
>
> [Install Race Coordinator Software
> 6](#install-race-coordinator-software)
>
> [Network Configuration 6](#network-configuration)

[**Quick Start 7**](#quick-start)

> [Run a Demo Mode (simulated) Race 7](#run-a-demo-mode-simulated-race)
>
> [Preparing the Quick Start Arduino Track Interface
> 10](#preparing-the-quick-start-arduino-track-interface)
>
> [Wiring the Arduino to the track 11](#wiring-the-arduino-to-the-track)
>
> [Uploading the RC Sketch to the Arduino
> 13](#uploading-the-rc-sketch-to-the-arduino)
>
> [Configuring RC for the Quick Start Arduino Track Interface
> 15](#configuring-rc-for-the-quick-start-arduino-track-interface)
>
> [Manage Arduino - GENERAL Tab Settings
> 17](#manage-arduino---general-tab-settings)
>
> [Manage Arduino - ANALOG SETUP Tab Settings
> 18](#manage-arduino---analog-setup-tab-settings)
>
> [Manage Arduino - DIGITAL SETUP Tab Settings
> 19](#manage-arduino---digital-setup-tab-settings)
>
> [Run a Live Race 21](#run-a-live-race)

[**Track Setup 23**](#track-setup)

> [Expert Track Setup 23](#expert-track-setup)
>
> [Track Manager 24](#track-manager)
>
> [General 24](#general)
>
> [Lanes 25](#lanes)
>
> [Track Interface 26](#track-interface)
>
> [Trackmate 27](#trackmate)
>
> [Arduino 30](#arduino)
>
> [What is an Arduino? 30](#what-is-an-arduino)
>
> [A Race Coordinator + Arduino-based Race Management System
> 30](#a-race-coordinator-arduino-based-race-management-system)
>
> [Connecting Individually Addressable RGB LED Strip Lights
> 31](#connecting-individually-addressable-rgb-led-strip-lights)
>
> [Uploading the RC Sketch to the Arduino
> 32](#uploading-the-rc-sketch-to-the-arduino-1)
>
> [Parallel Port 36](#parallel-port)
>
> [Web Cam 36](#web-cam)
>
> [RC Configuration & Testing 36](#rc-configuration-testing)
>
> [Installing & Configuring Third-Party Motion Detection Software
> 37](#installing-configuring-third-party-motion-detection-software)
>
> [Hints / Suggestions / Troubleshooting Motion Detection
> 43](#hints-suggestions-troubleshooting-motion-detection)
>
> [Game Port 43](#game-port)
>
> [DS Electronics DSxx 44](#ds-electronics-dsxx)
>
> [What you need to get started 44](#what-you-need-to-get-started)
>
> [Setting up your DS - Setting the correct Control Mode
> 45](#setting-up-your-ds---setting-the-correct-control-mode)
>
> [Setting up your DS - Setting the Minimum Lap Time
> 47](#setting-up-your-ds---setting-the-minimum-lap-time)
>
> [Setting up your DS - Setting the Race Length in Time Mode
> 48](#setting-up-your-ds---setting-the-race-length-in-time-mode)
>
> [Setting up your DS - Setting the Race Length in Lap Mode
> 48](#setting-up-your-ds---setting-the-race-length-in-lap-mode)
>
> [Setting up Race Coordinator 49](#setting-up-race-coordinator)
>
> [Slot Master 54](#slot-master)
>
> [Bepfe/Titus 54](#bepfetitus)
>
> [Phidget 55](#phidget)

[**Car Setup 56**](#car-setup)

> [Expert Car Setup 56](#expert-car-setup)
>
> [Car Manager 57](#car-manager)
>
> [Adding a Car 58](#adding-a-car)
>
> [Updating a Car 58](#updating-a-car)
>
> [Removing a Car 58](#removing-a-car)

[**Driver Setup 60**](#driver-setup)

> [Driver Guided Setup 60](#driver-guided-setup)
>
> [Expert Driver Setup 61](#expert-driver-setup)

[**Race Setup 63**](#race-setup)

> [Race Setup 63](#race-setup-1)
>
> [Creating & Editing Race Formats 63](#creating-editing-race-formats)
>
> [Guided Race Setup 64](#guided-race-setup)
>
> [Basic Guided Setup 64](#basic-guided-setup)
>
> [Intermediate Guided Setup 64](#intermediate-guided-setup)
>
> [Expert Guided Setup 64](#expert-guided-setup)
>
> [Expert Race Setup 65](#expert-race-setup)
>
> [‘Main’ Tab 66](#main-tab)
>
> [Race Name 67](#race-name)
>
> [Car Filter 67](#car-filter)
>
> [Minimum Lap Time 67](#minimum-lap-time)
>
> [Callbutton Delay 67](#callbutton-delay)
>
> [Heat Auto Start Info 67](#heat-auto-start-info)
>
> [Auto Advance Warmup 67](#auto-advance-warmup)
>
> [Auto Advance Time 67](#auto-advance-time)
>
> [Auto Start Warmup 68](#auto-start-warmup)
>
> [Auto Start Callouts 68](#auto-start-callouts)
>
> [Heats 70](#heats)
>
> [Practice 70](#practice)
>
> [Custom Round Robin Sequence 71](#custom-round-robin-sequence)
>
> [Single Heat (Solo/Any Lane) 71](#single-heat-soloany-lane)
>
> [Single Lane 71](#single-lane)
>
> [Single Lane (Solo) 72](#single-lane-solo)
>
> [Round Robin Heat Rotation 72](#round-robin-heat-rotation)
>
> [Round Robin 72](#round-robin)
>
> [European Round Robin 72](#european-round-robin)
>
> [Friendly Round Robin 72](#friendly-round-robin)
>
> [Custom Rotation 72](#custom-rotation)
>
> [Scoring 75](#scoring)
>
> [Heat Ranking Method 75](#heat-ranking-method)
>
> [Ranking 76](#ranking)
>
> [Breakout Parameters 76](#breakout-parameters)
>
> [Breakout Time 76](#breakout-time)
>
> [Breakout Percentage 76](#breakout-percentage)
>
> [Tiebreaker 76](#tiebreaker)
>
> [Overall Ranking Method 77](#overall-ranking-method)
>
> [Accumulate Heats 77](#accumulate-heats)
>
> [Step Up 77](#step-up)
>
> [Number to Step Up 77](#number-to-step-up)
>
> [Drop Lowest N Heats 77](#drop-lowest-n-heats)
>
> [Tiebreaker 78](#tiebreaker-1)
>
> [Start Method 78](#start-method)
>
> [Hot Start 78](#hot-start)
>
> [Restart on False Start 78](#restart-on-false-start)
>
> [Start Behind Sensor 78](#start-behind-sensor)
>
> [Start Next At Current Position 79](#start-next-at-current-position)
>
> [Finish Method 79](#finish-method)
>
> [Drift Time 80](#drift-time)
>
> [Adjust Drift Laps 80](#adjust-drift-laps)
>
> [Points 81](#points)
>
> [Use Points 81](#use-points)
>
> [Carry Over Percentage 81](#carry-over-percentage)
>
> [Heat Points 81](#heat-points)
>
> [Fastest Lap Bonus 81](#fastest-lap-bonus)
>
> [Fastest Heat Lap Bonus 81](#fastest-heat-lap-bonus)
>
> [Fastest Lap Per Lane Bonus 82](#fastest-lap-per-lane-bonus)
>
> [Most Overall Laps Led 82](#most-overall-laps-led)
>
> [Led At Least One Overall Lap 82](#led-at-least-one-overall-lap)
>
> [Led At Least One Heat Lap 82](#led-at-least-one-heat-lap)
>
> [One Lane Bonus Per Driver 82](#one-lane-bonus-per-driver)
>
> [Season 83](#season)
>
> [Season Points 83](#season-points)
>
> [Carryover Percentage 83](#carryover-percentage)
>
> [Race Points 84](#race-points)
>
> [Heat Points 84](#heat-points-1)
>
> [Fastest Lap Bonus 84](#fastest-lap-bonus-1)
>
> [Fastest Heat Lap Bonus 84](#fastest-heat-lap-bonus-1)
>
> [Fastest Lap Per Lane Bonus 84](#fastest-lap-per-lane-bonus-1)
>
> [Bonus Points 84](#bonus-points)
>
> [Analog Fuel 84](#analog-fuel)
>
> [Fuel Usage 85](#fuel-usage)
>
> [Use Fuel 86](#use-fuel)
>
> [Heat Reset 86](#heat-reset)
>
> [End Heat 86](#end-heat)
>
> [Capacity 86](#capacity)
>
> [Usage Type 86](#usage-type)
>
> [Reference Lap Time 86](#reference-lap-time)
>
> [Usage Per Reference Time 86](#usage-per-reference-time)
>
> [Fuel Start Level 86](#fuel-start-level)
>
> [Refuel Rate 86](#refuel-rate)
>
> [Pit Delay 86](#pit-delay)
>
> [Pit Delay Max 86](#pit-delay-max)
>
> [Crash n Learn 88](#crash-n-learn)
>
> [General Preferences 88](#general-preferences)
>
> [Enabled 88](#enabled)
>
> [Crash Time 88](#crash-time)
>
> [Yellow on Crash 89](#yellow-on-crash)
>
> [Maximum Crashes 89](#maximum-crashes)
>
> [Multiple Crashes 89](#multiple-crashes)
>
> [Heat Reset Crashes 89](#heat-reset-crashes)
>
> [Heat Reset DQ 89](#heat-reset-dq)
>
> [Penalties 90](#penalties)
>
> [Heat Crash Lap Penalty 90](#heat-crash-lap-penalty)
>
> [Heat Crash Time Penalty 90](#heat-crash-time-penalty)
>
> [DQ Heat Score Pct 90](#dq-heat-score-pct)
>
> [DQ Heat Overall Score Pct 91](#dq-heat-overall-score-pct)
>
> [UI 92](#ui)
>
> [Show Images 92](#show-images)
>
> [Sort By Heat Standings 92](#sort-by-heat-standings)
>
> [RaceDay XAML File Prefix 92](#raceday-xaml-file-prefix)
>
> [Example Full File Name 93](#example-full-file-name)
>
> [Race Start XAML File 93](#race-start-xaml-file)
>
> [Restart XAML FIle 93](#restart-xaml-file)
>
> [Start Delay 93](#start-delay)
>
> [Restart Delay 93](#restart-delay)
>
> [Start Randomizer 93](#start-randomizer)
>
> [Restart Randomizer 93](#restart-randomizer)
>
> [Groups 94](#groups)
>
> [Use Groups 94](#use-groups)
>
> [Use Teams 94](#use-teams)
>
> [Max Groups 94](#max-groups)
>
> [Num Teams 95](#num-teams)
>
> [Min Advancing 95](#min-advancing)
>
> [Balance 95](#balance)
>
> [Allow Empty Lanes 95](#allow-empty-lanes)
>
> [Force Multiple of Max 96](#force-multiple-of-max)
>
> [Rotate Group Heats 96](#rotate-group-heats)
>
> [Images 97](#images)
>
> [Audio 98](#audio)
>
> [Heat Callouts 99](#heat-callouts)

[**Event Setup 100**](#event-setup)

> [Races and Events 101](#races-and-events)
>
> [Races Available 101](#races-available)
>
> [Drivers 101](#drivers)
>
> [Current Races 101](#current-races)
>
> [Current Events 101](#current-events)
>
> [Name 101](#name)
>
> [Auto Advance Time 101](#auto-advance-time-1)
>
> [Event Creation 101](#event-creation)

[**Season Setup 102**](#season-setup)

> [Season Name 102](#season-name)
>
> [Drop N Worst Races 102](#drop-n-worst-races)

[**Getting Ready for a Race 103**](#getting-ready-for-a-race)

> [Overview 103](#overview)
>
> [Cars Available 104](#cars-available)
>
> [Drivers Available / Drivers Racing
> 104](#drivers-available-drivers-racing)
>
> [Options 106](#options-1)
>
> [Quick Driver Assignment Controls
> 106](#quick-driver-assignment-controls)
>
> [Race Type / Race/Event Selection 107](#race-type-raceevent-selection)
>
> [Season Selection 107](#season-selection)
>
> [Demo Mode 108](#demo-mode)

[**Running a Race (Race Day) 109**](#running-a-race-race-day)

> [Overview 109](#overview-1)
>
> [File 109](#file-1)
>
> [Save / Save As 109](#save-save-as)
>
> [Export 110](#export)
>
> [Race Director 110](#race-director)
>
> [Track Power 111](#track-power)
>
> [Windows 111](#windows)

[**Race Screen Customization (XAML)
112**](#race-screen-customization-xaml)

> [What is XAML? 112](#what-is-xaml)
>
> [Why Does Race Coordinator Use XAML?
> 112](#why-does-race-coordinator-use-xaml)
>
> [How Does Race Coordinator Use XAML?
> 112](#how-does-race-coordinator-use-xaml)
>
> [Example Data Types 113](#example-data-types)
>
> [Element Numbering 116](#element-numbering)
>
> [Let’s Build a Real Layout, Step by Step
> 117](#lets-build-a-real-layout-step-by-step)
>
> [Step 1: Start with the base window
> 117](#step-1-start-with-the-base-window)
>
> [Step 2: Add a Viewbox to scale everything
> 117](#step-2-add-a-viewbox-to-scale-everything)
>
> [Step 3: Add a Grid for rows and columns
> 118](#step-3-add-a-grid-for-rows-and-columns)
>
> [Step 4: Add a Label to show the driver's name
> 118](#step-4-add-a-label-to-show-the-drivers-name)
>
> [Step 5: Add an Image for the driver’s avatar
> 118](#step-5-add-an-image-for-the-drivers-avatar)
>
> [Step 6: Add a Lap Count 118](#step-6-add-a-lap-count)
>
> [Putting It All Together 118](#putting-it-all-together)
>
> [Common Gotchas to Avoid 119](#common-gotchas-to-avoid)
>
> [Theme Dictionary 119](#theme-dictionary)
>
> [Why It's Important in RC Layouts
> 120](#why-its-important-in-rc-layouts)
>
> [Using Theme Dictionary 120](#using-theme-dictionary)
>
> [Race Coordinator XAML Layout Explanation – Line by Line
> 120](#race-coordinator-xaml-layout-explanation-line-by-line)
>
> [Field Names and Data Types 123](#field-names-and-data-types)
>
> [XAML Editing Software 130](#xaml-editing-software)

[**Appendices 132**](#appendices)

> [Appendix A - Definitions, Acronyms & Abbreviations
> 132](#appendix-a---definitions-acronyms-abbreviations)
>
> [Appendix B - Revision History 134](#appendix-b---revision-history)
>
> [Appendix C - Backup / Restore RC Database
> 136](#appendix-c---backup-restore-rc-database)
>
> [Backing up the RC Database 136](#backing-up-the-rc-database)
>
> [Restoring the RC Database 137](#restoring-the-rc-database)
>
> [Appendix D - XAML Keyboard Shortcuts
> 138](#appendix-d---xaml-keyboard-shortcuts)

# Introduction

## Introduction to Race Coordinator

Race Coordinator (RC) is a free alternative slot car lap counting
software package for the PC. It contains a wide range of racing options
from the most basic Round Robin races to the most complicated multi-race
events that include Practice time, one or more Qualifying races, and a
Finals.

Race Coordinator supports an unlimited number of drivers per race and an
unlimited number of lanes per track.

### Track Interface/Sensor Support

Race Coordinator supports all the common track interfaces and sensor
types:

- Trackmate

- Arduino

- Web Camera

- Parallel port

- Game Port

- DS Electronics DS200, DS300, DSxx

- Phidget sensors and relays

- Titus / Bfpe

- USB Slot Master

- IR Sensors

- Reed switches

- Dead strips

- Track call buttons and master / per lane power relays

### Features

Race Coordinator also provides an impressive list of features that will
accommodate the smallest basement races to the largest club races. Here
is a list of the most significant features:

- Skin-able race screens

- Several built in heat rotation formats, including round robin, solo
  racing, and single lane heats.

- Custom heat editor; any rotation you want to use you can, all you have
  to do is create it.

- Analog fuel support

- Per lane relay support

- F1 style scoring support, including bonus points for things like
  fastest lap in the race.

- Step-up race support

- Driver grouping

- Team racing

- False start detection and handling

- Permanent storage of race stats and the ability to export them to
  Microsoft Excel any time after the race has finished.

- Save/Load races, including auto saves in the event of a power outage
  or other issue during a race.

- Season/Championship mode in which race points accumulate across the
  entire season.

> 

There are many more*.* See the Race Formats section for more details on
how to set up various race formats.

### Easy Race Setup

Race Coordinator comes with a default database that has setup within it
a few drivers and cars, a four lane track, and a few races to try out
including a basic Round Robin race and a Practice race. For most users,
these races may be exactly what you're looking for.

In any event, once you configure your drivers and races, the Race Day
screen may be the only screen you ever use. It doesn't get any easier
than clicking on a race name or event and selecting race!

Race Coordinator supports a demonstration mode in which you don't need
to be hooked up to a track to run. Race Coordinator will run laps based
on current race settings so you can get a feel for how things work from
any PC you want.

## Purpose

Race Coordinator is designed to facilitate the management and
coordination of slot car races. This manual aims to provide
comprehensive instructions and guidelines for installing, configuring,
and operating Race Coordinator, ensuring a seamless and efficient racing
experience.

## Scope

This manual covers all aspects of Race Coordinator, including
installation, setup, race management, and troubleshooting. It is
intended for race organizers, administrators, and technical support
personnel.

## Support / Further Resources

Support is a big deal for any lap counting software - making sure it
works as needed and has the features the community requires. With that
said, in an effort to give a little back to the community, RC will
continue to be supported as long as there is need. There are no
guarantees a feature request gets put into RC, but if it makes sense and
works within the RC framework it will probably happen.

The team working on RC is small and as such testing every aspect of RC
thoroughly is a challenge. We've made every effort to make RC bug free,
however if issues do arise, once they are brought to our attention every
effort will be made to fix them quickly.

For additional support and resources, visit the Race Coordinator Support
web page:

[<u>http:</u>
<u>*/*www.racecoordinator.net/Support.html</u>](http://www.racecoordinator.net/Support.html)

> 

# System Overview

Race Coordinator has higher system requirements than most other lap
counting software packages. Make sure your PC meets all the requirements
listed below.

## System Architecture

Race Coordinator consists of a central software application running on a
PC that interfaces with various hardware components. The system
architecture includes the following:

- Race Coordinator software

- Windows PC

- Track sensors

- Slot Car controllers (analog or digital)

- Slot cars (analog or digital)

- (Optional) Relays to control track power

- (Optional) Local Area Network / Internet connection

## Hardware Requirements

- Track compatible with Race Coordinator software

- Analog slot cars or Digital slot cars fitted with the appropriate
  sensors

- Analog or Digital controllers compatible with RC

- Sensors: Lap counting, optional position, optional pit in/out

- Minimum PC hardware: 1 GHz processor, 1 GB RAM, 500 MB hard disk
  space.

- Although sound capability in the PC is not required for RC operation,
  it does enrich the race experience.

## Software Requirements

The current major version of RC, 1.15, requires a minimum Windows
Operating System (OS) of Windows XP. Thus Windows XP, Vista, 7, 8, 10,
and 11 are supported.

NOTE: The next major version of RC, 1.16, will require a minimum of
Windows 10.

Race Coordinator requires Microsoft .NET 4, and as such it has the
minimum system requirements of .NET 4. The Microsoft website indicates
that .NET 4 requires Windows XP or higher and the installer enforces
this. The installer should handle checking if .NET 4 is installed
already and install it for you if it is not.

For more information on .NET check out:

[<u>http://msdn.microsoft.com/en-us/netframework/aa569263.aspx</u>](http://msdn.microsoft.com/en-us/netframework/aa569263.aspx)

NOTE: Microsoft NET 4 imposes many requirements on the Operating System.
If it does not install, it is most likely because you need to perform
one or more Windows updates before you can install it. It is highly
recommended that your OS be fully updated before installing Race
Coordinator.

> 

# Installation

## Hardware Installation

- Assemble the track according to the manufacturer's instructions.

- Install & connect power control such as relays (master or per-lane).

- Install & connect lap counting sensors at the start/finish line.

- Connect car controllers to the track and ensure they are properly
  configured.

- (Optional) Install & connect position sensors at key points along the
  track.

- (Optional) Install & connect Lap In / Out sensors at desired pit
  locations.

- (Optional) Install & connect call button(s) and countdown / status
  LEDs.

## Software Installation

### Download Race Coordinator Software

Download Race Coordinator from the download page on the
racecoordinator.net website:

[<u>https://racecoordinator.net/download.html</u>](https://racecoordinator.net/download.html)

Select the latest version from the “Official Releases” table.

### Install Race Coordinator Software

- Run the RC installer and follow the on-screen instructions.

- Launch Race Coordinator and complete the initial setup wizard.

## Network Configuration

- Connect all hardware components to the same network (if applicable).

- Configure network settings within Race Coordinator to ensure proper
  communication between devices.

# Quick Start

This chapter is intended as a suggested how-to on getting started with
RC. The goal is to get the new user to the point where they can run a
short race on their own track.

> The step-by-step procedure is organized into three sections:

- The first section familiarizes the user with the RC interface by
  exploring a unique feature of RC — running a simulated (demo mode, in
  RC terminology) race.

- The second section instructs the user on wiring a basic 4-lane Arduino
  track interface to their track, and configuring Race Coordinator for
  that track interface. <u>If you use a different interface to tie</u>
  <u>Race Coordinator to your track, then skip this section.</u>

- The third section steps the user through running a short <u>live</u>
  race on their track.

## Run a Demo Mode (simulated) Race

1.  Make sure minimum hardware and software requirements are met as
    listed in [“<u>System Overview</u>”](#system-overview) [on page
    <u>3</u>](#system-overview).

2.  Install track hardware and the RC software as described in
    [“<u>Installation</u>” on page <u>4</u>](#installation).

3.  Get familiar with the terms listed in [“<u>Appendix A - Definitions,
    Acronyms & Abbreviations</u>” on page
    <u>38</u>](#appendix-a---definitions-acronyms-abbreviations). This
    should help to minimize confusion with the terms used in RC.

4.  In the Race Day Setup window, select “Round Robin” from the
    Race/Event Selection drop-down list. Now from the main menu bar
    along the top of the window click “Race Setup” and then click
    “Expert Race Setup”; this will open the Race Manager
    window.<img src=".\/media/image35.jpg"
    style="width:4.61597in;height:1.98681in" /><img src=".\/media/image17.jpg" style="width:5.2in;height:2.79771in" />

5.  Along the left side of the Race Manager window there are several
    tabs / buttons ; click on the “Scoring” tab. Within the “Finish
    Method” area of the screen, type “30” into the ”Finish Time” box as
    shown above. This will reduce the amount of race time per heat to 30
    seconds.<img src=".\/media/image63.png" style="width:4.98958in;height:4in" />

6.  Make sure to click on the “Update \>\>” button located approximately
    in the middle of the Race Manager window. This will save your
    changes to the Round Robin race format. Click the X in the upper
    right corner of the Race Manager window to exit and return to the
    Race Day Setup window.<img src=".\/media/image109.png"
    style="width:0.65972in;height:1.11944in" />

7.  Run a demo mode (simulated) race to get a feeling for how RC
    operates. The demo race will consist of 4 time-based heats, with
    each heat 30 seconds in duration. To configure and run a demo mode
    race:<img src=".\/media/image74.png"
    style="width:1.58958in;height:2.02986in" />

<!-- -->

1.  In the Race Day Setup window, assign 1 to 4 of the predefined
    drivers to the race, as described in [“Race Day Setup” starting on
    page 37](#getting-ready-for-a-race).

2.  Ensure “Round Robin” is still selected in the Race/Event Selection
    drop - down list.

3.  Click the “Demo Mode” box so that a check mark appears (i.e., Demo
    Mode is enabled).

4.  Click the “Start Race” button. This will cause the Race Day window
    to appear. The timer in the Race Day window will begin counting down
    from 10 minutes; this is called the Auto Start time, and it will
    continue to count down towards zero unless you manually end it.

5.  Press the spacebar to end the Auto Start time. Press the spacebar
    again to start the first heat. A small window titled “Start Your
    Engines” with five red start lights will appear. The five lights
    will each change from red to green; once all turn green Heat 1 will
    begin. RC will automatically begin assigning laps to each of the
    predefined drivers you added to the race, and the heat timer in the
    upper center of the window will show the time remaining. Racing for
    that heat ends when the heat timer reaches zero. The racing flags in
    the upper right corner of the window will change color from green to
    red, and the announcer voice will say “heat over”. Notice that
    operation does not automatically move on to Heat 2; this time allows
    the Race Director to make any modifications to the heat results,
    export information about the heat, etc. To move on to Heat 2, press
    the spacebar.

6.  Run heats 2 and 3 by pressing the space bar twice to start each
    heat. While one of the heats is running, press the spacebar; this
    will pause the heat. The Race Day window will show a yellow flag
    (track caution). Press the spacebar again to restart the heat.
    Again, after racing for each heat ends, press the spacebar to move
    onto the next heat.

7.  (Optional) Explore the other race information windows (Leader Board,
    Heat Results, On Deck, etc.) available via the Race Day Windows
    menu. You can't do any harm as these just give you information.

8.  Start heat 4 by pressing the spacebar twice. Notice that after
    racing for this heat ends, the racing flags in the upper right of
    the window will change color from green to <u>checkered</u>, and the
    announcer voice will say “<u>race over</u>”. Click the X in the
    upper right corner of the Race Day window; click Yes in the Warning
    dialog box that asks “Are you sure you want to end the race?”. This
    exits the Race Day window and returns you to the Race Day Setup
    window.

<!-- -->

8.  Congratulations - you have just completed running a simulated race!
    In the next section, you will connect your track to an Arduino-based
    interface.

## Preparing the Quick Start Arduino Track Interface

This section assumes an Arduino UNO will provide the interface between
RC and your track. **If you are planning to use a different interface,
skip this section and go to chapter [“Track Setup” on page
17](#track-setup) to configure your selected interface.**

According to the Arduino web site, “Arduino is an open-source
electronics platform based on easy-to-use hardware and software”. An
Arduino consists of a small circuit board with a microcontroller,
volatile memory (RAM), nonvolatile memory (EEPROM, otherwise commonly
known as “flash”), input-output channels and some supporting hardware
such as a power regulator. Users can store instructions in the flash
memory to implement a wide variety of functions. A two-way USB interface
is provided for linking to a PC; the USB link enables uploading firmware
into flash and/or communicating with PC application software (i.e., Race
Coordinator).

The Arduino is unique in Race Coordinator track interfaces in that it is
the only one in which special Race Coordinator-specific firmware must be
programmed into it before it can be used with RC. In Arduino parlance,
this code / firmware is called a *sketch*.

Preparing the Quick Start Arduino Track Interface consists of three
tasks:

- Wiring the Arduino to the track

- Uploading the RC Sketch to the Arduino

- Configuring RC for the Quick Start Arduino Track Interface

#### Wiring the Arduino to the track

The diagram below shows a basic 4-lane lap track interface made with an
Arduino UNO R3. One infrared phototransistor is mounted in each track
lane for sensing the laps. In addition to the lap counting sensors you
will also need a light source above the track to ensure sufficient light
to correctly detect cars. Power to each lane is controlled by a relay. A
pushbutton is added to control heats & races and to request track calls
(i.e., bring out the yellow flag). For the optional start LEDs, low
power LEDs may be powered from the Arduino I/O pins.

<img src=".\/media/image105.jpg"
style="width:6.79948in;height:7.80208in" />

The design can easily be scaled down to support tracks of less than 4
lanes. To support more lanes or add features such as pit sensors, then
an Arduino Mega would be used instead of an UNO.

The parts list and Arduino pin assignments for the Quick Start circuit
appear below:

<table>
<colgroup>
<col style="width: 7%" />
<col style="width: 16%" />
<col style="width: 23%" />
<col style="width: 53%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>QTY</strong></th>
<th style="text-align: center;"><strong>PART NUMBER</strong></th>
<th style="text-align: center;"><strong>DESCRIPTION</strong></th>
<th style="text-align: center;"><strong>NOTES</strong></th>
</tr>
<tr>
<th style="text-align: center;">1</th>
<th>Arduino UNO R3</th>
<th>Microcontroller</th>
<th>Refer to note in the LED current limiting resistor text below if
considering use of the Arduino UNO R4 Minima or UNO R4 WiFi</th>
</tr>
<tr>
<th style="text-align: center;">1</th>
<th>Sunfounder TS0011</th>
<th>4-channel 5V relay module</th>
<th>Similar parts are Sainsmart 101-70-101 and HL-54S (generic part
number, many seller names).</th>
</tr>
<tr>
<th style="text-align: center;">1</th>
<th>Various</th>
<th>5VDC, 500 mA power source</th>
<th>5V DC power source for relay coils. A “wall wart” type of AC to DC
power adapter is sufficient. The output current should be at least 500
mA. There are many suppliers of this type of power source.</th>
</tr>
<tr>
<th style="text-align: center;">4</th>
<th>Vishay BPW85</th>
<th>Infrared NPN Phototransistor, through-hole, 3mm, peak detection at
light wavelength = 850 nm</th>
<th>A similar part number is Würth Elektronik 1540032NA3090. 3mm devices
are better for the smaller dimensions of HO track; 5mm phototransistors
can be used for larger track scales, or a different sensor technology
can be implemented.</th>
</tr>
<tr>
<th style="text-align: center;">4</th>
<th>KOA Speer CFS1/ 4CT52R103J</th>
<th>Through hole resistor, 10K ohms, 5%, ¼ watt</th>
<th>Resistors for phototransistors: Many similar part numbers.</th>
</tr>
<tr>
<th style="text-align: center;">1</th>
<th>Various</th>
<th>Overhead source of 850 nm infrared light</th>
<th>This could be a light bridge, light bar, strip of infrared LEDs,
etc. Among the slot car businesses offering such products are Trackmate
Racing and 132SlotCar.us (DS Electronics). You can also easily make your
own structure.</th>
</tr>
<tr>
<th style="text-align: center;">1</th>
<th>Suzohapp 58- 9100-L</th>
<th>Momentary pushbutton switch</th>
<th>For track calls. “Arcade buttons” are often used. Similar part
numbers are Adafruit 3430, Sparkfun COM-09336, Slot Car Corner
RM-02000.</th>
</tr>
<tr>
<th style="text-align: center;">5</th>
<th>American Bright BL-BJE5V4V-AT-ND</th>
<th>5mm through hole LED, Red</th>
<th>[OPTIONAL] LEDs for Formula 1-style start lights. The sample circuit
uses 5mm (also known as T-1 3/4) red LEDs. Many similar part
numbers.</th>
</tr>
<tr>
<th style="text-align: center;">5</th>
<th>KOA Speer CFS1/ 4CT52R471J</th>
<th>Through hole resistor, 470 ohms, 5%, ¼ watt</th>
<th><p>[OPTIONAL] Through-hole resistors for Formula 1-style start
lights:</p>
<p>Adjust resistor value to obtain desired light output from your
chosen</p>
<p>LEDs. Many similar part numbers.</p>
<p><strong>Note:</strong> The two new R4 versions of the Arduino UNO
have reduced I/O pin current capacity compared to the UNO R3. If an UNO
R4 is being considered, the maximum current that can be provided to any
LED is 8 mA, and thus the minimum R value = 375 ohms.</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

| **ARDUINO PINS** | **USE** | **DESCRIPTION** |
|----|----|----|
| **2, 3, 4, 5** | Track power relays for lanes 1-4 | Arduino-compatible relay module(s) enable Race Coordinator to individually control power to each lane. |
| **8. 9, 10, 11** | Lap sensors for lanes 1-4 | Inputs from the infrared phototransistor track sensors, to record laps from each lane. |
| **12** | Track Call Button | A momentary push button provides a way to control RC operation and issue track calls |
| **A4, A5, 6, 7, 13** | (OPTIONAL) Start LEDs 1 - 5 | Formula 1 - style starting lights. The LEDs should be connected to these pins via a suitable resistor. The Arduino UNO R3 I/O pin high state voltage is 5V; a typical value of current limiting resistor is in the range of 220 to 470 ohms. |

The infrared sensors must be mounted to your track, one for each lane.
The Trackmate Racing folks created a short YouTube video on how to do
this for HO track; the procedure would be very similar for other makes
and scales of plastic track.
<u>https:/[/www.youtube.com/watch?v=dx1atB4k-J4](http://www.youtube.com/watch?v=dx1atB4k-J4)</u>

Infrared phototransistors can detect visible light, but they are more
sensitive to infrared light. The suggested phototransistors are most
sensitive to 850 nm light, so an 850 nm overheard light source (IR LEDs
or LED strips in a bridge or gantry) should be used for best
performance.

The collector leads of the infrared phototransistors are connected
through 10K ohm resistors to the 5V supply.

This operates the transistors in “switch mode”; the output of the
transistor is either all the way off or all the way on - it operates
very much like a switch. Switch mode is more compatible with the digital
input pins of the Arduino. When wired as shown in the diagram, the
Arduino pins will see a logic LOW when sufficient light is hitting the
top of the phototransistor, and a logic HIGH when the light is blocked
(i.e., by a slot car).

Note that a separate 5V DC power supply provides power to the coils of
the track power relays. The Arduino’s power circuit cannot provide
sufficient current for the relay coils. If using the suggested 4-channel
relay module, remove the jumper bridging the JD-VCC pins to VCC, and
connect the external source to the JD-VCC pin. Ensure that the Ground
(GND) of the Arduino and of the separate power supply are connected
together.

For each lane, connect the corresponding channel of the relay module
inline between the trackʼs power supply positive (+) terminal and the
controller. Use the Common (COM) and either the Normally Closed (NC) or
Normally Open (NO) terminals of the relay channel. NC is usually
preferred as you can still have power to the track if you decide to run
laps without Race Coordinator running. You’ll need to know whether you
chose NC or NO when you configure RC for the track interface.

### Uploading the RC Sketch to the Arduino

The second step in getting your Arduino ready for RC is to upload the RC
sketch to it. For this you will need to install the Arduino development
software (itʼs free). Note that the descriptions below show Arduino
development software that was current as of the release date of this
document; newer Arduino software may look different. Always check the
Arduino web site to obtain the most current software. You can also find
more detailed information there, if you need it.

**NOTE:** You donʼt have to use the same PC to upload sketches that you
use to run Race Coordinator. Some users have a separate laptop for
Arduino sketch editing / uploading.

1.  Connect a USB cable between the PC and Arduino. The specific cable
    needed is a USB 2.0 Type A male to Type B male (this type of cable
    is often used with printers). The B (square-ish shape) connector
    plugs into the
    Arduino.<img src=".\/media/image69.jpg" style="width:1.92in;height:1.41in" />

2.  If you haven’t already done so, boot up your PC. Your Arduino will
    receive power from the PC via the USB cable. The Power / ON LED of
    the Arduino should be lighted (green).

3.  Download the Arduino Integrated Development Environment (IDE)
    Software from the Arduino web site:

> <u>https:
> */*[www.arduino.cc/en/software](http://www.arduino.cc/en/software)</u>

4.  Launch the Arduino IDE.

5.  <u>Select your Arduino board.</u> To avoid any error while uploading
    your sketch to the board, the selected name must match the board
    connected to your computer. From the menu bar
    select:<img src=".\/media/image56.jpg"
    style="width:4.1475in;height:3.26624in" />

> Tools → Board and click on your board. In the screen shot to the
> right, an Arduino Uno is selected. The picture will look very similar
> when selecting the other supported Arduino models.

6.  <u>Add the FastLED library.</u> This will tell the Arduino how to
    communicate with RGB LEDs.

    1.  From the menu bar select: Sketch → Include Library → Manage
        Libraries.

    2.  In the Library Manager window, type ʻfastLEDʼ in the search box.

    3.  Wherever *FastLED by Daniel Garcia* appears, click on INSTALL.

7.  <u>Select the Arduino serial port.</u> From

> the menu bar select: Sketch → Serial Port. Click on the PCʼs serial
> (COM) port that your Arduino is connected to. This is likely to be
> COM3 or higher as COM1 and COM2 are usually reserved for a PCʼs
> built-in hardware serial ports. To determine the correct port, you can
> disconnect your Arduino board, close the Serial Port menu and then
> re-open the menu. The COMx entry that disappears should be that of the
> Arduino board. Reconnect the Arduino and select that serial port.

8.  <u>Select the RC sketch file.</u> From the menu bar select: File →
    Open and navigate to the RC Arduino folder (usually C:\Program Files
    (x86)\Race Coordinator\data\arduino\lapCounter) and select file
    lapCounter.ino. The sketch takes care of everything needed for the
    Quick Start Arduino without needing any modifications. **NOTE**: The
    RC sketch version at the time of writing was V1.0.0.13.

9.  <u>Verify and Upload the RC sketch</u>. If everything is set up
    correctly, you should be able to click on the Verify icon to check
    the code, and then click the Upload icon to send the code to the
    Arduino.<img src=".\/media/image13.jpg"
    style="width:0.26042in;height:0.30208in" /><img src=".\/media/image122.png"
    style="width:0.26042in;height:0.30208in" />

10. <u>Troubleshoot, if necessary</u>. If there are errors in the
    message box at the bottom of the IDE window, chances are that you
    have made a mistake in one of the steps above. Check the wiring
    carefully, the com port is correct, you have the FastLED library
    installed, and your specific Arduino selected.

### Configuring RC for the Quick Start Arduino Track Interface

In the Race Day Setup window, from the menu bar click “Track Setup” and
then click “Expert Track Setup”; this will open the Track Manager
window.

<img src=".\/media/image25.jpg" style="width:7.4in;height:3.98135in" />

The Track Manager window is used to configure general information about
the track (name, scale, number of lanes, etc.), and to select a specific
hardware interface. The window has two tabs – “General” and “Lanes”.

<img src=".\/media/image22.jpg" style="width:7.4in;height:3.98135in" />

For the Quick Start interface, values in the Lanes tab will not be
changed. Settings for the General tab of the Track Manager are:

- <u>Track Name</u>: Type in whatever name you refer to your track by –
  e.g., “Oscarʼs Oval”, “Elm Grove”, “Scottsboro Raceway”, etc.

- <u>Num Track Sections</u>: The number of virtual sections the track is
  divided into. Sections are used in determining partial lap scoring for
  time-based heats. RC uses this value to determine fractional laps at
  the end of a heat. Leave at the default value of 100.

- <u>Image</u>: (Optional) Click within the box to select an image file
  (.jpg, .bmp, .png, or .gif format) that shows your track. This image
  will appear on some race day screens.

- <u>Track Scale</u>: Type in the denominator of the fractional scale of
  your track – typical values are 24 (for 1/24 scale), 32 (for 1/32
  scale), 43 (for 1/43 scale) and 64 (for HO scale) The scale
  information is used to calculate scaled race performance values such
  as miles per hour.

Now while still on the General tab of the Track Manager window, select
“Arduino” from the list of radio buttons grouped under “Track Interface”
on the left side of the window, and then click the “Configure” button.
This will bring up the “Manage Arduino” window. From this window you
configure each signal in the Quick Start Arduino
interface.<img src=".\/media/image124.jpg"
style="width:1.61in;height:2.04269in" />

The Manage Arduino window has eight tabs listed across the top —
General, Analog Setup, Digital Setup, Led General, and Led String 1, 2,
3 and 4. For the Quick Start interface, only the first three tabs need
to be configured.

#### Manage Arduino - GENERAL Tab Settings

Click on the “General” tab that is along the top of the window. Settings
for this tab
are:<img src=".\/media/image92.jpg" style="width:5.34in;height:2.94204in" />

- <u>Name</u>: Unique identifier for this specific track interface.
  Leave at default value of “Arduino 1”.

- <u>Com Port</u>: Select the PC serial communications port the Arduino
  is connected to. This should be the same port used to connect to the
  Arduino IDE. If multiple ports are listed, you can always click each
  listed COM port, one at a time, then wait 5-10 seconds. If the
  "Connection" LED goes green you have found the correct port.

- Options :

  - <u>Trigger Laps on Low: Setting determines what logic signal level
    (low or high) at the Arduino pin signifies a lap. When enabled
    (checked), a lap will be counted when the input signal goes to a
    logic low level. Leave at default value of disabled (not checked;
    lap counted when signal goes high).</u>

  - <u>Invert Relays: Selects use of normally open (NO) or normally
    closed (NC) power relays. For the Quick Start circuit, set to
    disabled (not checked) if lanes are connected as NO, or enabled
    (checked) if lanes are connected as NC.</u>

  - <u>Invert LEDs: Setting determines what logic signal level (low or
    high) the Arduino pin is driven to when LEDs (Start Led 1 through 5
    for this circuit) are ON. Leave at default value of disabled (not
    checked; when LED is on the output pin is set to a logic high).</u>

  - <u>Lap Sensor For Pits Usage: This setting determines how and if the
    lap sensors are used in pit detection. There are three choices in
    the drop-down box: “Lap Pin as Pit”, “Lap Pin as Pit End” and “Lap
    Pin as Lap Only”. Select “Lap Pin as Lap Only”.</u>

  - <u>Use Pit Sensor as Lap: This setting determines if the pit sensors
    are also used as the lap sensors. Leave at default value of disabled
    (not checked).</u>

  - <u>Use Laps for Segments: This setting determines if the pit sensors
    are used to detect segments (partial laps). Leave at default value
    of disabled (not checked).</u>

  - <u>Debounce: The time, measured in microseconds, that RC waits after
    first sensing a change in an input signalʼs state before capturing
    the value. Leave at default value of 200.</u>

  - <u>Arduino Hardware: Multiple models of Arduino are supported. Make
    sure “Uno” is selected.</u>

- <u>Image Map</u>: It is a static graphic intended to show what colors
  of the virtual LEDs signify open and closed inputs / outputs.

- <u>Connection</u>: Turns green when the PC is communicating with the
  Arduino. If not green, you will need to debug the connection before
  continuing.

#### Manage Arduino - ANALOG SETUP Tab Settings

Click on the “Analog Setup” tab that is along the top of the window.
Settings for this tab
are:<img src=".\/media/image16.jpg" style="width:5.6in;height:2.97in" />

- <u>Pins A0 through</u> <u>A3</u>: Set to “Reserved”. By default the RC
  sketch uses these pins for strings of Neopixel (RGB) LEDs. Refer to
  the Arduino section of the Track Setup chapter for details on
  connecting and configuring RGB LED strings.

- <u>Pin A4</u>: Set to “Start Led 1”.

- <u>Pin A5</u>: Set to “Start Led 2”.

One very useful feature of RC is that it allows testing of track
interface inputs and outputs directly from the configuration window. The
interface configuration screen is a "live connection" to the track. Thus
you can make changes and immediately test on the track to make sure
they're working.

It is easy to test whether the Start LEDs are working. By default the
virtual LEDs for all Start LEDs should be red. Now move the mouse cursor
over each Start LED virtual LED and click it; the virtual LED should
change color to green. If the Arduino to LED connections are working,
when the virtual LED is green, the real Start LEDs should be lit.

#### Manage Arduino - DIGITAL SETUP Tab Settings

Click on the “Digital Setup” tab that is along the top of the window.
Settings for this tab are:

- <u>Pins 2, 3, 4 and 5</u>: Set to “Relay L1”, “Relay L2”, “Relay L3”
  and “Relay L4”,
  respectively.<img src=".\/media/image37.jpg" style="width:5.6in;height:2.97in" />

- <u>Pins 6 and 7</u>: Set to “Start Led 3” and “Start Led 4”,
  respectively.

- <u>Pins 8, 9, 10 and</u> <u>11</u>: Set to “Lap L1”, “Lap L2”,

- “Lap L3” and “Lap L4”, respectively.

- <u>Pin 12</u>: Set to “Callbutton”.

- <u>Pin 13</u>: Set to “Start Led 5”.

For this discussion it is assumed the relays have been connected as NC
(and the Manage Arduino-General tab has “Invert Relays” checked). By
default the virtual LEDs for all the lane relays should be red and all
the IN LEDs (IN1 through IN4) on the relay module should be lit. Now
move the mouse cursor over the Relay L1 virtual LED and click it. What
should happen is shown in the figure above —Relay L1ʼs virtual LED
changes color to green. This indicates the Arduino pin 2 state has
changed from OFF to ON. If the Arduino to relay module connections are
working, the relay moduleʼs IN1 LED should change from being lit to not
lit, and lane 1ʼs power should turn ON.

Make sure to perform “lap checks” of lap counting sensors Lap L1 through
L4. This is another instance where RCʼs “live connection” feature comes
in handy. If things are connected correctly, the overhead infrared light
source is on and the light is hitting the sensors in the track, all four
lap counting virtual LEDs will show red.

Each virtual LED should change color to green when the light to the
corresponding track sensor is blocked.

**IMPORTANT! → Once all configuration information has been entered, make
sure to click the “Accept” button in lower center of the window to save
the information into the RC database.**

Clicking the “Accept” button causes RC to exit the “Manage Arduino”
window and return to the “Track Manager \> General” window. Make any
additional changes needed in the Track Manager.

**IMPORTANT! → Once all information has been entered, make sure to
select the track the Arduino information is applicable to in the
rightmost column (most users have only one defined track, but multiple
tracks can be defined) and then click the “Update \>\>” button in middle
of the window to save the information.**

Congratulations - you have just completed connecting your track to an
Arduino-based interface and configuring it! In the next section, you
will run a live race on your track using Race Coordinator.

## Run a Live Race

1.  If you are using the Quick Start Arduino Track Interface described
    above, skip to step 3.

2.  If you are NOT using the Quick Start Arduino Track Interface
    described above, then configure your specific track interface per
    the detailed instructions in [“<u>Track Setup</u>” starting on page
    <u>17</u>](#track-setup).

    1.  Making sure lap counting sensors work is crucial. In the
        configuration window for your specific track interface, do “lap
        checks” to make sure the screen indicates the sensor change. For
        example, if your lap sensors are optical, wave your finger
        between the optical light source and the sensor.

    2.  When the track interface is fully working, click "Accept" in the
        track interfaceʼs configuration window to save any changes made.
        This will bring you back to the Track Manager window.

    3.  You must click "Update" in the Track Manager window to save any
        changes made. You may now exit from the Track Manager window.

3.  Make sure the track, overhead light source (if needed), and Arduino
    interface are powered.

4.  In the Race Day Setup window, click the “Demo Mode” box so that the
    check mark is not present (i.e., Demo Mode is disabled).

5.  Ensure “Round Robin” is still selected in the Race/Event Selection
    drop-down list.

6.  If needed, update the number of drivers assigned to the race to the
    number that will be actually (physically) racing. Even if only one
    driver is assigned, the round robin race format will test each of
    the four lanes.

7.  Click the “Start Race” button. This will cause the Race Day window
    to appear. The timer in the Race Day window will begin counting down
    from 10 minutes; this is called the Auto Start time, and it will
    continue to count down towards zero unless you manually end it.

8.  Place the slot cars in their assigned lanes.

9.  In all subsequent steps, “press the space bar” can mean just that OR
    if you wired one to your Arduino, press the call button. Press the
    space bar to end the Auto Start time. Press the space bar again to
    start the first heat. A small window titled “Start Your Engines”
    with five red start lights will appear. The five lights will each
    change from red to green; once all turn green Heat 1 will begin. The
    heat timer in the upper center of the window will show the time
    remaining. Racing for that heat ends when the heat timer reaches
    zero. The racing flags in the upper right corner of the window will
    change color from green to red, and the announcer voice will say
    “heat over”. Notice that operation does not automatically move on to
    Heat 2; this time allows the Race Director to make any modifications
    to the heat results, export information about the heat, etc.

10. To move on to Heat 2, press the space bar.

11. Move the slot cars to their new lane assignments.

12. Start Heat 2 by pressing the space bar twice. While the heat is
    running, press the space bar; this will pause the heat. The Race Day
    window will show a yellow flag (track caution). Press the space bar
    again to restart the heat. After racing for the heat ends, press the
    space bar to move on to Heat 3.

13. Move the slot cars to their new lane assignments.

14. Start Heat 3 by pressing the space bar twice.

15. (Optional) Explore the other race information windows (Leader Board,
    Heat Results, On Deck, etc.) available via the Race Day Windows
    menu. You can't do any harm as these just give you information.

16. After racing for the heat ends, press the space bar to move on to
    Heat 4.

17. Move the slot cars to their new lane assignments.

18. Start Heat 4 by pressing the space bar twice. Notice that after
    racing for this heat ends, the racing flags in the upper right of
    the window will change color from green to checkered, and the
    announcer voice will say “race over”. Click the X in the upper right
    corner of the Race Day window; click Yes in the Warning dialog box
    that asks “Are you sure you want to end the race?”. This exits the
    Race Day window and returns you to the Race Day Setup window.

Congratulations - you have just completed running a race on your track
using Race Coordinator!

> 

# Main Screen

<img src=".\/media/image33.png" style="width:7.5in;height:4.54167in" />

The main screen is where the from which the program is controlled. From
here, you can configure all aspects of the race, add cars, drivers,
tracks and events. You also start races from here, either real or
simulated.

The screen is broken into several areas: menus; Cars Available; Drivers
Available; Options; Race Control (not labelled) and Drivers Racing. Each
of these sections will be covered in more detail in the chapters to
follow and the format of the manual will be to follow the menu at the
top.

<img src=".\/media/image7.png" style="width:7.5in;height:0.41667in" />

# File

<img src=".\/media/image68.png"
style="width:3.61979in;height:1.44151in" />

Under the bonnet, Race Coordinator uses a complicated database. It can
be accessed by the user but it is highly likely that the database could
be corrupted if accessed by someone other than an expert. The only time
that a user would open this menu, is if requested for information to
track a bug and only at the express request of an administrator of RC.

# Car Setup

Car Setup is used to maintain a database of slot cars raced on the
track. Cars defined by Car Setup can be assigned to drivers in the Race
Day Setup window. There is one option for creating, modifying, and
deleting cars – Expert Car Setup.

## Expert Car Setup

In the Race Day Setup window, from the menu bar click “Car Setup” and
then click “Expert Car Setup”; this will open the Car Manager window.

<img src=".\/media/image110.jpg" style="width:7.4in;height:3.98135in" />

## Car Manager

> The Car Manager window provides a way to update the portion of the RC
> database pertaining to cars. Cars can be added, modified or deleted.
> The left side of the window shows all the information about one car
> and the right side lists all defined cars.

<img src=".\/media/image127.jpg" style="width:7.4in;height:3.98135in" />

> The left side of the Car Manager is where the information about each
> car is entered / edited. There are four database fields per car. The
> top three fields are text, and the fourth points to an image file of
> the car. The following descriptions of the car database fields are
> only suggestions, as what gets entered into the database should be
> whatever makes the most sense to the users.

- Name: The name you use to refer to the car – e.g., “Ford GT40”, “Lola
  T70”, “Alʼs Jalopy”, etc.

- Info: Optional secondary information about the car, such as itʼs
  number, livery, etc. In the list of cars shown on the right side of
  the window, this information is appended to the end of the Name.

- Type: The class / generation / vendor / etc. of the slot car. As an
  example, for HO cars this value could be “T-Jet” (Thunderjet),
  “Super-G+”, “SG+”, “Mega-G+”, etc.

- Image: A picture of the car. This image will appear on some race day
  screens. The image file format can be .jpg, .bmp, .png, or .gif.

### Adding a Car

To add a car, fill in all the desired information about the car in the
text and image fields on the left side of the screen. Click within the
Image box to select an image file (.jpg, .bmp, .png, or .gif format) of
the car. The default directory for car images is C:\Program Files
(x86)\Race Coordinator\data\images\cars. **<u>NOTE</u>**: In Windows 10
and above, Administrator privileges are required to move or copy a file
into the default car image directory.

<img src=".\/media/image40.jpg" style="width:6.4in;height:3.6in" />

Once all fields are entered, click the “Add \> \>” button in the middle
of the window. You will note that after clicking the button, the new
entry will appear at the bottom of the “Cars Available” list on the
right side. The new entry has now been saved into the RC database.

### Updating a Car

To update the details of an existing car in the “Cars Available” list:

- Click on the car in the “Cars Available” list (right side of the
  window). This will populate its information in the editing fields in
  the left side of the window.

- Edit the Name, Info, Type and Image fields as desired.

- Click the “Update \> \>” button in the middle of the window. The carʼs
  entry has now been updated and saved in the RC database.

### Removing a Car

To delete the entry of an existing car in the “Cars Available” list:

- Click on the car in the “Cars Available” list (right side of the
  window). This will populate its information in the editing fields in
  the left side of the window.

- Click the “Remove \< \<” button in the middle of the window. The carʼs
  entry has now been deleted from the RC database. **<u>Note</u>**: you
  are not asked to confirm the removal, so make sure this is what you
  want to do!

> 

# Driver Setup

Driver Setup is used to maintain a database of drivers that race on the
track. Drivers defined by Driver Setup are assigned to track lanes in
the Race Day Setup window. There are two options for creating,
modifying, and deleting drivers – Driver Guided Setup and Expert Driver
Setup.

## Driver Guided Setup

In the Race Day Setup window, from the menu bar click “Driver Setup” and
then click “Driver Guided Setup”; this will begin a series of dialog
boxes that prompt for all the database information associated with a
driver.

<img src=".\/media/image27.jpg" style="width:7.4in;height:3.98135in" />

## 

##  

## Expert Driver Setup

<img src=".\/media/image12.png"
style="width:6.81771in;height:3.89177in" />

Select the Driver Name box and remove any existing name. Add in the
*real* name of the driver.

In the Driver Nickname, choose a fun name to be known by in the race
itself.

Click on the Image box and navigate to an image you want for the driver.

<img src=".\/media/image66.png"
style="width:6.73523in;height:2.38508in" />

The audio can be personalised to the driver. So, each driver could have
their own Personal Best sound or phrase, for example. To change the
default audio, double-click on the appropriate box and navigate to the
wav file required. Only wav files are supported.

<img src=".\/media/image50.png"
style="width:5.46145in;height:5.65108in" />

Remember to Add \>\> if introducing a new driver or Update\>\> if making
changes to an existing one.

# Track Setup

Race Coordinator supports the following hardware track interfaces:

- Trackmate

- Arduino

- PC Parallel Port

- Web Cam

- DS Electronics DSxx

- Slot Master

- Bepfe/Titus

- Phidget

For Trackmate, Arduino, DS Electronics and Phidget, only certain models
are supported. Refer to each interfaceʼs configuration section for more
details.

Track Setup is used to configure Race Coordinator for your specific
track interface(s). There is one option for entering track configuration
– Expert Track Setup.

**Note**: If more than one track interface is required, ‘Multi-Track”
must be selected in the Options/Preferences menu. See section on Options

## Expert Track Setup

In the Race Day Setup window, from the menu bar click “Track Setup” and
then click “Expert Track Setup”; this will open the Track Manager
window.

<img src=".\/media/image25.jpg" style="width:7.4in;height:3.98135in" />

## Track Manager

The Track Manager window is used to configure general information about
the track (name, scale, number of lanes, etc.), and to select a specific
hardware interface. The window has two tabs – General and Lanes.

<img src=".\/media/image22.jpg" style="width:7.4in;height:3.98135in" />

### General

The General tab of the Track Manager is where the following information
is entered:

- Track Name: Type in whatever name you refer to your track by – e.g.,
  “Oscarʼs Oval”, “Elm Grove”, “Scottsboro Raceway”, etc. The default
  name is “Bright Plume Raceway”.

- Num Track Sections: Type in the number of sections the track is
  divided into. Sections are used in determining partial lap scoring for
  time-based heats. RC uses this value to determine fractional laps at
  the end of a heat. The default value is 100.

- Image: (Optional) Click within the box to select an image file (.jpg,
  .bmp, .png, or .gif format) that shows your track. This image will
  appear on some race day screens.

- Track Scale: Type in the denominator of the fractional scale of your
  track – typical values are 24 (for 1/24 scale), 32 (for 1/32 scale),
  43 (for 1/43 scale) and 64 (for HO scale) The scale information is
  used to calculate scaled race performance values such as miles per
  hour. The default value is 64.

- Track Interface: Click the “radio button” corresponding to the
  interface hardware used to connect the PC to your track. Refer to the
  Track Interface sections for details on configuring specific track
  interfaces.

**IMPORTANT! → Once all information has been entered, make sure to
select the track the information is applicable to in the rightmost
column (most users have only one defined track, but many can be defined)
and then click the “Update \>\>” button in the middle of the window to
save the information.**

### Lanes

The Lanes tab of the Track Manager is where information pertaining to
each track lane is entered. The top- most colored rectangle in the
“Current Lanes” list box on the left side of the window is Lane 1; the
colored rectangle underneath it is lane 2, etc. \[In the screen capture
shown below, Lane 1 has a lane color of Tomato\]. Clicking on a colored
rectangle in the “Current Lanes” box fills in the Lane Color, Lane Font
Color, and Lane Length (actual physical length) values that have been
set for that lane.
<img src=".\/media/image123.png" style="width:7.4in;height:3.98135in" />

Double-clicking on the Lane Color and Lane Font Color boxes brings up a
color picker dialog that makes it easier to choose the desired color.

Enter the physical length, in feet, of the lane in the Lane Length box.
This information is used by RC for calculations such as the partial
number of laps completed.

To add a lane, click the “Add Lane” button on the left side of the
window. The new lane will be added to the bottom of the list. It will
have the same color and length values as the currently selected lane.

To modify the values of an already defined lane, first select the lane
in the “Current lanes” box. Modify any or all of the parameters, and
then click the “Update Lane” button on the left side of the window.

To delete a lane, select the lane in the “Current lanes” box and then
click the “Remove Lane” button on the left side of the window.

**IMPORTANT! →** Once all information has been entered, make sure to
select the track the information is applicable to in the rightmost
column (most users have only one defined track, but many can be defined)
and then click the “Update \>\>” button in the middle of the window to
save the information.

## Track Interface

RC must be configured to use the hardware providing the communication
interface between your track to the PC. Although most tracks use one
track interface, multiple interfaces can be configured for a single
track.

One very useful feature of RC is that it allows testing of track
interface inputs and outputs directly from the configuration window. The
interface configuration screen is a "live connection" to the track. Thus
you can make changes and immediately test on the track to make sure
they're working. <u>Some interfaces have a live on-</u> <u>screen
“virtual Connection LED”. If that virtual LED is red, even the most
basic interface setup is not working.</u>

For some interfaces it's always green because RC has no way to know if
it is working or not.

Details on configuring a track interface are specific to that hardware.
Refer to the detailed configuration instructions for each specific
interface that follow. Some of the sections are rather lengthy, so use
the page numbers (hyperlinks) listed in the table below to jump to the
desired section.

<img src=".\/media/image109.png"
style="width:2.71875in;height:2.72361in" />

### Trackmate

RC supports any Trackmate interface that connects to a PC via either a
physical or a virtual serial communications (COM) port. The Trackmate
interfaces that meet this requirement are shown in the table below

<table>
<colgroup>
<col style="width: 8%" />
<col style="width: 11%" />
<col style="width: 9%" />
<col style="width: 19%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr>
<th style="text-align: left;"><blockquote>
<p><strong>MODEL #</strong></p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p><strong>NICKNAME</strong></p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p><strong>DATE DESIGNED</strong></p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p><strong>PC INTERFACE</strong></p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p><strong>DESCRIPTION / NOTES</strong></p>
</blockquote></th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>SCL-R</p>
</blockquote></th>
<th style="text-align: left;">Red Board</th>
<th style="text-align: left;">2008</th>
<th style="text-align: left;"><blockquote>
<p>9-pin serial / COM port</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Supports 8 lanes of lap count, 1 track relay, call button(s). In
newer PCs, requires USB to serial adapter cable. Compatible with 25-pin
sensor cables.</p>
</blockquote></th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>SCL3-USB</p>
</blockquote></th>
<th style="text-align: left;">Black Board</th>
<th style="text-align: left;">March 2014</th>
<th style="text-align: left;"><blockquote>
<p>USB / virtual USB COM port</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Supports 8 lanes of lap count, 1 track relay, call button(s).
Trackmate software version ≥ 9.61 already has a USB driver built in;
click Help &gt; Install USB Driver from within the Trackmate Software.
Compatible with RJ45 sensor cables.</p>
</blockquote></th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>SCL81</p>
</blockquote></th>
<th style="text-align: left;">Blue Box</th>
<th style="text-align: left;">March 2022</th>
<th><blockquote>
<p>USB / virtual USB COM port</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Supports 8 lanes of lap count, 1 track relay, call button(s). In
blue-ish plastic enclosure. Trackmate software version ≥ 9.61 already
has a USB driver built in; click Help &gt; Install USB Driver from
within the Trackmate Software. Compatible with RJ45 sensor cables.</p>
</blockquote></th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>SCL45</p>
</blockquote></th>
<th style="text-align: left;">Blue Box</th>
<th style="text-align: left;">March 2022</th>
<th><blockquote>
<p>USB / virtual USB COM port</p>
</blockquote></th>
<th><blockquote>
<p>Supports 4 lanes of lap count, 5 relays (1 master + 4 per-lane via
separate relay board*), call button(s). In blue-ish plastic enclosure.
Trackmate software version ≥ 9.61 already has USB driver built in; click
Help &gt; Install USB Driver from within the Trackmate Software.
Compatible with RJ45 sensor cables.</p>
</blockquote></th>
</tr>
<tr>
<th style="text-align: left;"></th>
<th style="text-align: left;"></th>
<th style="text-align: left;"></th>
<th style="text-align: left;"></th>
<th style="text-align: left;"><blockquote>
<p><strong>* Race Coordinator does not support Trackmate
per-lane</strong></p>
<p><strong>relays</strong></p>
</blockquote></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

The “Red Board” interface hardware connects to a PC via a 9-pin serial
connection. If the PC does not have a 9- pin serial port, then it may
work using a USB-to-serial converter cable based on the FTDI chipset.
Refer to Trackmateʼs web site for details:

<u>https:
*/*trackmateracing.com/shop/en/content/14-slot-car-lap-counter</u>

The first steps are to set up the Trackmate system per the Trackmate
User Manual. This includes:

- Install the Trackmate software

- Plug in hardware interface

- Install Track Call button

- Install lap count sensors (and overhead infrared lights if using
  infrared sensors)

- Install track power relay

- Configure the Trackmate interface via the Settings \> Installation
  Settings window.

Refer to the Trackmate User Manual for details. Make sure everything is
working per Trackmateʼs instructions before attempting to configure RC.
**NOTE: Make sure to write down what COM Port the Trackmate Installation
Settings window shows is being used - you will want to have this when
configuring RC.**

To configure RC for a Trackmate interface, go to the General tab of the
Track Manager window, select “Serial Trakmate” from the list of Radio
Buttons grouped under “Track Interface” on the left side of the window,
and then click the “Configure” button. This will bring up the “Manage
Serial Trakmate Port” window. From this window you configure the
Trackmate interface. You can also manually control track power and check
status of the lap count sensors and Track Call
button.<img src=".\/media/image44.png" style="width:1.29in;height:1.64in" />

**Note: RC only supports a MASTER track power relay with Trackmate; it
does not support per-lane relays.** If independent per lane power
control is desired, then adding either an Arduino or Phidget to control
the relays is suggested.

Configurable parameters, controls and status indicators for Trackmate
are as follows:

- Name: Unique identifier for this specific track interface. Default
  value is “Trakmate
  1”.<img src=".\/media/image42.jpg" style="width:5.59in;height:3.01in" />

<!-- -->

- Com Port: Select the PC serial communications port the Trackmate is
  connected to. You can find the COM Port number from the Trackmate
  Installation Settings window. If you donʼt have that, click each
  listed COM port, one at a time, wait 5-10 seconds. If the "Connection"
  LED goes green you have found the correct port.

- IR Sensors: When checked, enables connection of infrared (IR) lap
  counting sensors. Default is enabled (checked).

- Invert Relays: Allows use of normally open (NO) or normally closed
  (NC) power relays. Default is enabled (checked). Does checked mean NO
  or NC, or is it not that simple?

- Debounce: Sensor debounce value. Leave set at the Trackmate default
  value of 1.

- Track Power On: Click the button to turn track power on via the
  Trackmate interface.

- Track Power Off: Click the button to turn track power off via the
  Trackmate interface.

- Connection: Turns green when the PC is communicating with Trackmate.

- Lane 1 - Lane 8: Turns green when the corresponding lap counting
  sensor has detected a lap.

- Callbutton: Turns green when the call button connected to the
  Trackmate is pressed.

- Image Map: It is a static graphic intended to show what colors of the
  virtual LEDs signify open and closed inputs / outputs.

**IMPORTANT! → Once all configuration information has been entered, make
sure to click the “Accept” button in lower center of the window to save
the information into the RC database.**

Clicking the “Accept” button causes RC to exit the “Manage Serial
Trakmate Port” window and return to the “Track Manager \> General”
window. Make any additional changes needed in the Track Manager.

**IMPORTANT! → Once all information has been entered, make sure to
select the track the Trackmate information is applicable to in the
rightmost column (most users have only one defined track, but many can
be defined) and then click the “Update \>\>” button in the middle of the
window to save the information.**

### Arduino

The Arduino is unique in Race Coordinator track interfaces in that it is
the only one in which special firmware must be programmed into it before
it can be used with RC. In Arduino parlance, this code / firmware is
called a *sketch*.

There are many Arduino models, clones of those models and variations;
three models of Arduino / Arduino- based products are supported by RC:

- Arduino UNO\* (and clones)

- Arduino Mega (and clones)

- Viasue Hub

**NOTE: \* Arduino UNO R4 Minima and UNO R4 WiFi are not currently
supported; the different processors in the R4 models cause communication
errors with RC.**

#### What is an Arduino?

According to the Arduino web site, “Arduino is an open-source
electronics platform based on easy-to-use hardware and software”. It is
similar to the Raspberry Pi but more hardware / control oriented. An
Arduino consists of a small circuit board with a microcontroller,
volatile memory (RAM), nonvolatile memory (EEPROM, otherwise commonly
known as “flash”), input-output channels and some supporting hardware
such as a power regulator. Users can store instructions (again, called a
sketch) in the flash memory to implement a wide variety of functions. A
two-way USB interface is provided for linking to a PC; the USB link
enables uploading a sketch into flash and/or communicating with
application software on the PC.

#### A Race Coordinator + Arduino-based Race Management System

A Race Management System (RMS) based around Race Coordinator and an
Arduino provides tremendous flexibility. A block diagram of a basic
example system is shown below:

<img src=".\/media/image115.png"
style="width:7.46875in;height:1.89244in" />

All of this will be explained in more detail later, but in general:

- The Race Coordinator software application runs on the PC.

- The PC connects to the Arduino via USB. The USB port is assigned a
  Communication (COM) port by Microsoft Windows. Race Coordinator needs
  to be told which COM port has been assigned, as it “talks” to the
  Arduino via this COM port.

- The Race Coordinator-specific “sketch” (also known as code, firmware,
  etc.) runs on the Arduino. This code controls the flow of information
  between Race Coordinator and the track.

- Physical wiring connections are made between the Arduino and the
  track. Devices such as sensors, LEDs, relays, and call buttons can be
  connected to the Arduino. Support of additional devices can be
  accomplished by adding custom code to the Arduino sketch.

#### Connecting Individually Addressable RGB LED Strip Lights

Optional (and fun) devices to connect to your Arduino are individually
addressable RGB LED strip lights. Each strip consists of multiple RGB
LED “chips” mounted on a flexible circuit board. RC supports the
connection of up to four addressable LED strips. By default, the RC
Arduino sketch software assigns pins A0 - A3 to these.

These pins correspond to Led String 1 - 4 within RCʼs Track Setup for an
Arduino (you will learn how to assign functions to the individual LEDs
later).

- **NOTE: The RC Arduino sketch supports a maximum of 25 LEDS per LED
  string.**

- **NOTE: You can connect the LED strips to pins other than A0 - A3, but
  if you do then you must make some slight changes to the RC sketch
  code. Refer to section *YYYY* to find out how to do that.**

The RGB LED chips go by many names — NeoPixel, WS2811, WS2812, SK6812,
etc. Each RGB LED chip can use up to 60 milliamps of current, so it
doesn’t take too many of them to overwhelm the Arduino’s power
capabilities. To prevent that possibility, connect a separate 5V DC
power supply\* to the LED strip. Ensure that Grounds (GND) of the
Arduino and of the separate power supply are connected together. Refer
to the diagram below. The 470 ohm resistor and the 500 to 1000
microfarad capacitor are not strictly needed, but are considered best
practices to maintain data signal integrity and to protect against
sudden supply voltage changes. The resistor should be located as close
to the Arduino as possible. The capacitor should have a voltage rating
of at least 6.3V DC; 10V is preferred. Capacitors in this capacitance
value range are typically polarized - i.e., they have positive and
negative pins. Make sure you wire the polarity of the capacitor
correctly! The side of the capacitor near the negative pin usually has
ʻ–ʼ text printed on a white / light colored
band.<img src=".\/media/image6.jpg"
style="width:5.28646in;height:2.92014in" />

#### Uploading the RC Sketch to the Arduino

In order to get the Arduino ready for RC, it must have a special RC
sketch programmed into it. The term for programming the sketch into an
Arduino is called uploading; Arduino development software (it is free)
is used to carry out the uploading. Note that the descriptions below
show Arduino development software that was current as of the release
date of this document; newer Arduino software may look different. Always
check the Arduino web site to obtain the most current software. You can
also find more detailed information there, if you need it.

**NOTE:** You donʼt have to use the same PC to upload sketches that you
use to run Race Coordinator. Some users have a separate laptop for
Arduino sketch editing / uploading.

The steps to upload a sketch to an Arduino are as follows:

1.  Connect a USB cable between the PC and Arduino. The specific cable
    needed is a USB 2.0 Type A male to Type B male (this type of cable
    is often used with printers). The B (square-ish shape) connector
    plugs into the Arduino.<img src=".\/media/image69.jpg"
    style="width:1.91742in;height:1.41231in" />

2.  If you havenʼt already done so, boot up your PC. Your Arduino will
    receive power from the PC via the USB cable. The Power / ON LED of
    the Arduino should be lighted (green).

3.  Download the Arduino Integrated Development Environment (IDE)
    Software from the Arduino web site:

> <u>https:
> */*[www.arduino.cc/en/software](http://www.arduino.cc/en/software)</u>

4.  Launch the Arduino IDE.

5.  <u>Select your Arduino board.</u> To avoid any error while uploading
    your sketch to the board, the selected name must match the board
    connected to your computer. From the menu bar
    select:<img src=".\/media/image56.jpg"
    style="width:4.08689in;height:3.21851in" />

> Tools → Board and click on your board. In the screen shot to the
> right, an Arduino Uno is selected. The picture will look very similar
> when selecting the other supported Arduino models.

6.  <u>Add the FastLED library.</u> This will tell the Arduino how to
    communicate with RGB LEDs.

    1.  From the menu bar select: Sketch → Include Library → Manage
        Libraries.

    2.  In the Library Manager window, type ʻfastLEDʼ in the search box.

    3.  Wherever *FastLED by Daniel Garcia* appears, click on INSTALL.

7.  <u>Select the Arduino serial port.</u> From the menu bar select:
    Sketch → Serial Port. Click on the PCʼs serial (COM) port that your
    Arduino is connected to. This is likely to be COM3 or higher as COM1
    and COM2 are usually reserved for hardware serial ports. To
    determine the correct port, you can disconnect your Arduino board,
    close the Serial Port menu and then re-open the menu. The COMx entry
    that disappears should be that of the Arduino board. Reconnect the
    board and select that serial port.

8.  <u>Copy the RC sketch file to a writable directory.</u> The supplied
    sketch takes care of pretty much everything for an initial setup,
    but depending on your setup there may be a few things that need to
    be configured differently. This means the sketch file needs to be
    edited. RC installs the sketch file in a directory that users do not
    have write access to, and thus you canʼt save an edited version of
    the file there. In a windows explorer window go to directory
    C:\Program Files (x86)\Race Coordinator\data\arduino\lapCounter and
    select file lapCounter.ino. Copy that file to a directory where you
    have write access (the userʼs Documents folder is a suggestion, but
    it can be any writable directory). **NOTE**: The RC sketch version
    at the time of writing is V1.0.0.13.

9.  <u>Edit the RC sketch file.</u> xxxx

10. <u>Upload the sketch to the Arduino.</u> From the menu bar select:
    File → Open and navigate to the writable directory where xxx…

To make life a bit easier, click on File/Preferences and tick ʻDisplay
line numbersʼ and click OK.

On line 34, uncomment the \#define WITH_FAST_LED.

The default assignment for the LED strings is to use Arduino pins A0-A3.
If you do not use these pins, you will need to redefine the pins in this
section (lines 164-167, on the current version of the sketch). Donʼt
change the MAX_RGB_LED_STRINGS, even if you donʼt use them all.

> \#ifdef WITH_FAST_LED
>
> // RGB pixels
>
> \#define MAX_RGB_LED_STRINGS 4 \#define STRING_PIN_1 A0 \#define
> STRING_PIN_2 A1 \#define STRING_PIN_3 A2 \#define STRING_PIN_4 A3

On lines 171 to 181 are the types of LED strips that are currently
supported:

> // \#define LED_TYPE_1 TM1803
>
> // \#define LED_TYPE_1 TM1804
>
> // \#define LED_TYPE_1 TM1809
>
> // \#define LED_TYPE_1 WS2811
>
> // \#define LED_TYPE_1 WS2812
>
> // \#define LED_TYPE_1 WS2812B
>
> // \#define LED_TYPE_1 APA104
>
> // \#define LED_TYPE_1 UCS1903
>
> // \#define LED_TYPE_1 UCS1903B
>
> // \#define LED_TYPE_1 GW6205
>
> // \#define LED_TYPE_1 GW6205_400

Find your one and ensure that lines 183 to 186 have the correct type.
The Default is WS2811, as it is the most common.

> \#define LED_TYPE_1 WS2811  
> \#define LED_TYPE_2 WS2811  
> \#define LED_TYPE_3 WS2811  
> \#define LED_TYPE_4 WS2811

If you have Neopixels, then leave lines 196 to 199 as is. If you donʼt,
remove the ʻ/ʼ from lines 191 to 194 and add the, to lines 196 to 199.

> //#define SETUP_LED_1(leds, numLeds) FastLED.addLeds\<LED_TYPE_1,
> STRING_PIN_1, RGB\>(leds, numLeds);
>
> //#define SETUP_LED_2(leds, numLeds) FastLED.addLeds\<LED_TYPE_2,
> STRING_PIN_2, RGB\>(leds, numLeds);
>
> //#define SETUP_LED_3(leds, numLeds) FastLED.addLeds\<LED_TYPE_3,
> STRING_PIN_3, RGB\>(leds, numLeds);
>
> //#define SETUP_LED_4(leds, numLeds) FastLED.addLeds\<LED_TYPE_4,
> STRING_PIN_4, RGB\>(leds, numLeds);
>
> \#define SETUP_LED_1(leds, numLeds) FastLED.addLeds\<NEOPIXEL,
> STRING_PIN_1\>(leds, numLeds); \#define SETUP_LED_2(leds, numLeds)
> FastLED.addLeds\<NEOPIXEL, STRING_PIN_2\>(leds, numLeds);
>
> \#define SETUP_LED_3(leds, numLeds) FastLED.addLeds\<NEOPIXEL,
> STRING_PIN_3\>(leds, numLeds); \#define SETUP_LED_4(leds, numLeds)
> FastLED.addLeds\<NEOPIXEL, STRING_PIN_4\>(leds, numLeds);

That should be it.

If everything is set up correctly, you should be able to click on the
\[VERIFY SYMBOL\] to verify the code, then the \[UPLOAD SYMBOL\] to
upload the code to the Arduino.

If there are problems in the message box below, chances are that you
have made a mistake in one of the steps above. Check the wiring
carefully, verify the com port is correct, you have the FastLED library
installed and your specific Arduino is selected.

Note: Some LED strings have multiple (usually three) LEDs per address,
others have only one. When there are three LEDs per address, for every
RC command that is sent to the LED, three will light up instead of one.

### Parallel Port

To be added.

### Web Cam

RC works in conjunction with 3rd party motion detection software to
count laps, detect pit entry & exit, and to signal track calls. RC
provides a command line executable program that gets called by the
motion detection software whenever motion is detected in configured
areas within the webcam picture called “zones” or “hot spots”.

#### **RC Configuration & Testing**

There is no configuration information to be entered into RC when using a
webcam as a track interface; all that needs to be done within RC is to
select the webcam as the desired interface. To select the webcam
interface, go to the General tab of the Track Manager window, then
select “Web Cam” from the list of Radio Buttons grouped under “Track
Interface” on the left side of the window. Click the “Accept” button in
the lower center of the window to save the information into the RC
database.<img src=".\/media/image34.png"
style="width:1.28958in;height:1.63958in" />

> If you click on the “Configure” button after selecting “Web Cam” from
> the list of “Track Interface” Radio buttons, an informational dialog
> box will appear as a reminder that the interface does not need to be
> configured.<img src=".\/media/image112.png"
> style="width:2.81229in;height:1.15324in" />

**IMPORTANT!** **→ Once “Web Cam” has been selected, make sure to click
the “Accept” button in the lower center of the window to save the
selection into the RC database.**

That's all the configuration you need to do within RC. Before moving on
let's test that everything is working right so far. RC install comes
with an application called "Webcam.exe" in RCʼs install directory
C:\Program Files (x86)\Race Coordinator. It accepts the following
command lines:

- "Webcam.exe -lap \#" : Trigger a lap, where "#" is the lane number in
  the range 1 to 8.

- "Webcam.exe -callbutton" : Signal a track call. This has various
  results depending on the race state.

- "Webcam.exe -pitenter \#" : If you want to do fuel races, put a
  trigger point at the same location as your Start/Finish line trigger
  and use this command line. The "#" is the lane you wish to enter the
  pits and ranges from 1 to 8.

- "Webcam.exe -pitexit \#" : When you want a car to exit the pits in a
  fuel race, put a second trigger point right after the Start/Finish
  line and run this command. Again, "#" is the lane number between 1 and
  8.

- "Webcam.exe -noerrordisplay" : Disable any error messages from the
  webcam interface. Once configured properly this is useful to do if you
  wish to run in situations that would generate errors (like racing
  without RC running).

Create a shortcut to the Webcam.exe program that will trigger a lap on
Lane 1. How to create a shortcut varies from OS to OS, but on Windows 7
simply right click the webcam.exe program located in RC's install
directory and select "Create Shortcut". Now right click on your shortcut
and select "properties". You have to change the target line to include
the command line for generating a lap. The target line to trigger a lap
on Lane 1 looks exactly as follows:

"C:\Program Files (x86)\Race Coordinator\Webcam.exe" -lap 1

You will now test manually triggering laps using the shortcut you just
created. Start up RC and run your race. Make sure you are NOT in demo
mode. Note: On some operating systems you must run RC with administrator
rights in order for the webcam interface to work. Once RC is running and
your race is under the green flag, simply double click your shortcut to
Webcam.exe. If you don't get an error message, it most likely worked. Do
it a few more times to simulate the "reaction time" and actual laps. If
you do this 5 or so times over 30 seconds, you should see laps being
counted. If you get an error message, hopefully the error message makes
it clear what might be the issue.

Hopefully you've been able to manually trigger laps using the shortcut.
Now that you know things are working, install and configure your 3rd
party motion detection software.

#### **Installing & Configuring Third-Party Motion Detection Software**

Any Windows-based motion detection software that can call an external
application when it detects motion will work with RC. The motion
detection software also needs to be able to support a sufficient number
of cameras and / or zones / hot spots to support your track’s number of
lanes. Most software supports webcams with a USB connection; if your
camera is IP-based, make sure to choose software that supports your
camera.

Webcam Zone Trigger (<http://www.zonetrigger.com/>) is a widely known
instance of such software. There is a free 15 day trial; after the trial
expires the Standard Edition license costs \$45USD. The configuration
description below is based on Webcam Zone Trigger version 3.7; the
procedure for configuring other motion detection software should be
similar.

After installing Webcam Zone Trigger, a window stating that the software
is operating as a trial appears. From this screen you can either
continue the trial (up until the trial period expires) or enter a
license code for the Standard or Pro editions of the program. After
accepting either of those options, the main Zone Trigger window appears:

<img src=".\/media/image61.png" style="width:6.65in;height:4.20573in" />

Note that these windows are for the Standard version of the program; the
Pro version’s main window is slightly different. The first thing to do
is to add & configure your camera. Clicking on the “Connect Camera”
button in the left center of the main screen brings up the “Add a New
Video Source” window:

<img src=".\/media/image85.png" style="width:7in;height:2.6069in" />

Click on the type of camera within the list in the upper left area of
the window; cameras already connected to your computer will appear in
the upper right area of the window. Click on the desired camera, leaving
the Video Resolution and Frames per second settings at their default
values. Click on the “Connect” button. The main window will return, but
now showing your camera view:

<img src=".\/media/image78.png" style="width:6.65in;height:4.18594in" />

This example shows how to set up lap counting on a two-lane HO scale
track. You can also use the software with RC to monitor pit entries, pit
exits, and a call button.

Adjust the height of your camera above the track surface until you get a
good view of all desired lanes. You may need to adjust or add lighting
until a good picture is obtained. Once that is done, you are ready to
add & configure Hot Spots.

To add the first Hot Spot, click on the “Add Hot Spot” button located in
the center column of icons (it is the only button that is active until
at least one Hot Spot has been created). Hot Spot number 1 is created,
as shown in the screen capture below:<img src=".\/media/image29.png"
style="width:0.79688in;height:0.59766in" />

<img src=".\/media/image82.png" style="width:6.65in;height:4.20573in" />

By default, this creates a round Hot Spot. The shape can be changed, but
it is suggested to try the round shape first. Move the mouse cursor
inside the Hot Spot and use the mouse to drag Hot Spot 1 to its desired
location within the webcam’s view; in this case, lane 1:

<img src=".\/media/image102.png"
style="width:6.65in;height:4.20573in" />

Now to assign an action to when motion is detected within Hot Spot 1.
Click on the “Choose an action…” dropbox and choose “Run a command or
program”. The Run File or Command… dialog window will open:

<img src=".\/media/image3.png" style="width:7.125in;height:4.48281in" />

Click on the browse button to locate the Webcam.exe application within
the RC installation directory, and type ‘-lap 1’ into the Parameters
line.

<img src=".\/media/image96.png"
style="width:7.125in;height:4.48281in" />

Click “OK”. The action has now been assigned to Hot Spot 1:

<img src=".\/media/image9.png" style="width:7.125in;height:4.48281in" />

You can assign additional actions to the Hot Spot as desired, such as
playing a specific sound. There is also an option in Settings \> General
to play a chime sound each time ANY Hot Spot detects motion.

At this point, repeat the procedure for adding as many additional Hot
Spots as lanes to be counted.

**IMPORTANT!** **→ Once all Hot Spots have been defined, it is important
to call up the RC and Zone Trigger programs in the proper sequence. RC
should be started before Zone Trigger, and Zone Trigger should be exited
prior to exiting RC. If the programs are not started and exited in this
order, Zone Trigger can quickly create enough error dialogs to fill up
your screen.**

#### **Hints / Suggestions / Troubleshooting Motion Detection**

You'll need to tweak your hot spot locations and camera sensitivity to
get things just right. It is strongly recommended to do one lane at a
time. If you have trouble with your webcam software, you can post on any
of the support forums as there are a lot of users willing to help out
that actually have the same software you are trying to use.

Dark cars may not want to trigger. You can increase the hot spot
sensitivity and/or place white strips of tape in each lane to provide
contrast.

Light shadows as well as people bumping the table can inadvertently
cause triggers. Audible sounds are handy for solving these sensitivity
problems both in setup and during racing. Have good lighting above the
track even if it means adding LEDs to your start line bridge. Make a
sturdy mount for your camera. Mount the camera straight above the
desired spot (e.g., start/finish line) rather than at an angle if at all
possible.

Camera height doesn't seem to be that critical as long as it can focus
at the chosen height. Setting it to just where all lanes are covered or
slightly higher so you can zoom/pan a bit for centering works fine. 7
inches above the track is a good starting point.

### Game Port

To be added.

### DS Electronics DSxx

DS Electronics makes stand-alone lap counting systems. DS lap counting
systems serve as lap count sensors when used with Race Coordinator. Race
Coordinator supports the following DS Electronics lap counter products:

- DS-030 (older product, supports up to 4 lanes)

- DS-200 (supports 2 lanes)

- DS-300 / 300RC (supports up to 2 lanes in base unit; expandable up to
  8 lanes)

Pendle Slot Racing, a slot car vendor in the UK, has a detailed blog
entry on how to use DS lap counting systems with Race Coordinator:

[<u>https://www.pendleslotracing.co.uk/blog/cat/features/post/ds-lap-counters-race-cordinator/</u>](https://www.pendleslotracing.co.uk/blog/cat/features/post/ds-lap-counters-race-cordinator/)

They have graciously allowed reproduction of that blog entry in the
ensuing paragraphs.

The DS range of lap counters is one of the best aftermarket upgrade
systems available for use with Scalextric, Ninco, SCX, Carrera and club
tracks. It provides all the race information, various race type setups
and pin-point accuracy you need while being very simple to use.

<img src=".\/media/image8.jpg" style="width:7.5in;height:4.22222in" />While
the DS lap counting system does all the vital race timings and positions
really well, the one thing that we have found when using it for more
than two lanes is that the data at the end of a race is a little
limited. This is where Race Coordinator comes in.

#### **What you need to get started**

- DS200 or 300/334+
  \<[<u>http://www.pendleslotracing.co.uk/brand/ds-racing.html</u>](http://www.pendleslotracing.co.uk/brand/ds-racing.html)\>

- DS lap timing gantry
  \<[<u>http://www.pendleslotracing.co.uk/brand/ds-racing.html</u>](http://www.pendleslotracing.co.uk/brand/ds-racing.html)\>

- Power supply for your DS system

- Serial to USB adaptor cable

- Download of RC software on a laptop or computer

#### **Setting up your DS - Setting the correct Control Mode**

Before powering up your DS lap counting boxes you need to set it so that
it is programmed for individual mode. We do this by the following
method.

- Press and hold the Yellow memory/Pause button on the right and side
  while powering up the box.

- There will be two modes to choose from:

  - Ctrl Indi = Individual control

  - Ctrl Ttal = Total Control

- You can choose the option by pressing the Mode button left center.

- You will want to save it so that Ctrl Indi is our default setting and
  to do this you press the Yellow memory/pause button on the option
  displayed and that will store it as a default setting for future
  use.<img src=".\/media/image43.jpg" style="width:7.5in;height:4.22222in" />

<img src=".\/media/image32.jpg" style="width:7.5in;height:4.22222in" />

#### **Setting up your DS - Setting the Minimum Lap Time**

Scroll through the modes until you find the setting option Pt as shown
below. Then using the 2 programming buttons you can set your minimum lap
time. Here we have set ours to 7 seconds.

To set your minimum lap time you need to work out what the lap record is
on your circuit and then take anything from 0.5 to 1 second off that
time.

Setting the minimum lap time stops lanes from clocking up dubious laps
if more than one car crosses that lane sensor. To save this as your
default lap time, you press the memory/pause button to confirm. This
applies for the next two
settings.<img src=".\/media/image31.jpg" style="width:7.5in;height:4.22222in" />

#### **Setting up your DS - Setting the Race Length in Time Mode**

Scroll through the modes until you find the setting option P-ti as shown
below. Then using the 2 programming buttons you can set your race time.
Here we have set ours to 1 minute and 20 seconds.

When using with RC you will need to set this higher than the race time
in RC; i.e.,

- RC set for 1 minute race = DS 1.20 minutes

- RC set for 2 minute race = DS 2.20 minutes

#### **Setting up your DS - Setting the Race Length in Lap Mode**<img src=".\/media/image26.jpg" style="width:7.5in;height:4.22222in" />

Scroll through the modes until you find the setting option P-LA as shown
below. Then using the 2 programming buttons you can set the race length
in laps. Here we have set ours to 10 laps.

**NOTE:** When using with RC you will need to set this 1 lap higher than
the number of laps in RC; i.e.,

- RC set for 10 lap race = DS 11 laps

- RC set for 15 lap race = DS 16 laps

- RC set for 20 lap race = DS 21 laps

<img src=".\/media/image86.jpg" style="width:7.5in;height:4.22222in" />

#### **Setting up Race Coordinator**

The following screenshots show what settings were used while testing out
the software with the
DS300.<img src=".\/media/image93.jpg" style="width:7.00564in;height:3.8in" />

RC Race day Screen

RC Track Setup \> Track Manager \| General Screen

<img src=".\/media/image21.jpg" style="width:7.00564in;height:3.8in" />

RC Track Setup \> Manage SSD (Configure DS) Screen

<img src=".\/media/image30.jpg" style="width:7.00564in;height:3.8in" />

RC Track Setup \> Track Manager \| Lanes Screen

<img src=".\/media/image62.jpg" style="width:7.5in;height:4.06944in" />

RC Race Manager \| Main Setup Screen

<img src=".\/media/image4.jpg" style="width:7.5in;height:4.06944in" />

RC Race Manager \| Heats Setup Screen

<img src=".\/media/image79.jpg" style="width:7.5in;height:4.06944in" />

RC Race Manager \| Scoring Setup Screen

<img src=".\/media/image20.jpg" style="width:7.5in;height:4.06944in" />

RC Race Manager \| Points Setup Screen

<img src=".\/media/image10.jpg" style="width:7.5in;height:4.06944in" />

It is suggested to first test using the settings shown above. Once
successfully running with those, then adjust the settings to meet your
needs.

###  

### Slot Master

To be added.

### Bepfe/Titus

To be added.

###  

### Phidget

The Phidgets web site describes them as “electrical building blocks for
sensing and control using a computer, tablet, or phone”. Phidget boards
provide sensors, controllers (motors, relays, LEDs, LCDs, etc.) and
generic I/O interfaces. For more information on Phidgets, refer to their
web site: [<u>https://www.phidgets.com/</u>](https://www.phidgets.com/)

Relay boards and generic I/O interfaces are the Phidgets supported by
Race Coordinator - specifically the ones whose names start with
“Interface Kit”. There are a number of mechanical and solid state relay
boards available that provide various current / voltage capacities;
these are used for RC master or per-lane track power control. The
generic I/O interfaces support Race Coordinator lap counting, pit
detection, call buttons and stop / go LEDs. Phidgets connect to the host
PC via USB.

**NOTE: Be careful with using Phidgets for lap timing. It can't read the
sensor data very fast (digital inputs are sampled 125 times a second)
and therefore you get less than 0.001 second timing accuracy. Phidgets
are great for relays and call buttons, but if you're going to build your
own interface, use an Arduino.**

The first step is to connect your Phidget boards(s) to your PC’s USB
port(s) via either USB A to B or USB A to mini-B cables . Even though
Phidgets do provide a Windows driver, you do not need to install it - RC
uses its own built-in Phidget software library.

To configure RC for a Phidget interface, go to the General tab of the
Track Manager window, select “Phidget” from the list of Radio Buttons
grouped under “Track Interface” on the left side of the window, and then
click the “Configure” button below it. This will bring up the “Manage
Phidget Interface Kit” window. From this window you configure the
Phidget
interface.<img src=".\/media/image95.png" style="width:1.3in;height:1.768in" />

> 

# Race Setup

## Race Setup

Race Setup (or Race Manager, as it is called when you open the Expert
Race Setup page) is the fine detail of how the race is configured. It
covers the name, type of race, heats, types of heats, scoring, fuel and
a lot more. This section is the key to how your racing will be done.

When you click on the Race Setup option on the main window, you will see
three types of guided setup (wizard): Basic, Intermediate and Expert.
You will also see ‘Expert Race Setup’. This takes you to the
configuration page itself, if you are proficient enough to not need the
wizards (or have particular needs that aren’t on the wizard.

<img src=".\/media/image52.png" style="width:7.5in;height:4.47222in" />

## Creating & Editing Race Formats

Creating Races: Navigate to the Race Setup window to create new or edit
existing race formats. New race formats can be created using either
guided setups (i.e., wizards) or expert setup (i.e., manual entry).

Setting Parameters: Configure race parameters such as laps, time limits,
and rules.

### Guided Race Setup

Guided setups present a series of dialog boxes that step through each of
the settings for creating a Race Setup.

#### Basic Guided Setup

Introduction: Welcome to the basic guided race setup. This setup will
walk you through setting up a race using only the most common race
configurations. Everything else will be handled for you. This guide is
useful for those users who just want to race but are unhappy with the
default race setups the RMS provides.

More Information: Some questions will have a 'more' button visible at
the bottom. Use this button to get more information on the configuration
option being asked about.

#### Intermediate Guided Setup

Introduction: Welcome to the intermediate guided race setup. This setup
will walk you through setting up every race feature the RMS supports.
All major features will be covered in this guide, however many of the
more obscure options that most users will not need to configure will be
skipped. This guide is useful for users with more complex race formats.

More Information: Some questions will have a 'more' button visible at
the bottom. Use this button to get more information on the configuration
option being asked about.

#### Expert Guided Setup

Introduction: Welcome to the expert guided race setup. This setup will
walk you through setting up every single configuration option possible
for a race. This guide is useful for users who need absolute control
over their configuration.

More Information: Some questions will have a 'more' button visible at
the bottom. Use this button to get more information on the configuration
option being asked about.

## Expert Race Setup

<img src=".\/media/image55.png" style="width:7.5in;height:4.45833in" />

On this screen you set up the ‘container’(better description?). On the
right, under Current Races, you will see any races that have already
been set up. Clicking on one will bring up the details for that race for
the tab (down the left) that you are configuring. So, If you select, in
this example, Fuel Round Robin, you can then select any of the tabs and
see the configuration for Fuel Round Robin.

On every tab, the Current Races configured will be shown. If you want to
edit an existing race, select the race and move on to the parameters you
want to configure. When you have finished, click on Update\>\>. If you
don’t, your changes will be lost.

<img src=".\/media/image73.png"
style="width:3.66667in;height:3.54167in" />

If you want to make a new race, over-type an existing race name (see
Race Name below) and press Add\>\>. **NB** if ‘Add’ a race that exists
already, a message will pop up, explaining you need a unique name.

<img src=".\/media/image19.png"
style="width:3.86458in;height:2.125in" />

To remove a race, select the race and press ‘\<\<Remove’. The ‘Help’
button will take you to the wizard.

### ‘Main’ Tab

If there are Current Races configured on the right hand side but you
want to create a new one, you could use one of the configured races as
your starting point. ie choose the race that is closest to your
requirement and start from there.

#### Race Name

Enter your Race Name in the top left box then press Add\> to save your
new race, rather than overwriting an existing race.

#### Car Filter

\[No idea what this is\]

#### Minimum Lap Time

Measured in seconds, any lap triggered under this value will be ignored.

### Callbutton Delay

Measured in seconds, the time after the call button is pressed before
the yellow flag is triggered and the heat is paused.

#### Heat Auto Start Info

Auto Advance Time

The time to wait (in seconds) at the end of each heat before
automatically advancing to the next heat screen. 0 disables the
auto-advance.

#### Auto Advance Warmup

Select how long you would like track power on for before the RMS
automatically advances to the next heat.

#### Auto Advance Time

The time to wait (in seconds) before automatically starting the current
heat. 0 disables the auto-start.

Track power will remain off until the auto advance timer reaches this
value at which time power will come on as the heat auto advances. Warmup
time only affects track power, no laps or lap times will be reported.

As an example, if the auto advance timer is set to 30 seconds, and the
auto advance warmup time is set to 20 seconds, track power will come on
10 seconds after the heat ends.

The auto advance warmup time plus the auto start warmup time will equal
the total continuous time track power is turned on allowing for drivers
to warm up between heats.

#### Auto Start Warmup

Select how long you would like track power on for before the heat
starts.

Track power will turn on as soon as the RMS advances to the next heat
and power stays on while the auto start time is counting down. Warmup
time only affects track power, no laps or lap times will be reported.

As an example, if the auto start timer is set to 30 seconds, and the
auto start warmup time is set to 20 seconds, track power will be on
until 10 seconds before the heat starts.

The auto advance warmup time plus the auto start warmup time will equal
the total continuous time track power is turned on allowing for drivers
to warm up between heats.

#### Auto Start Callouts

These are the audible messages used to, in this example, to call out how
long before the next heat will start and when to play the message.

<img src=".\/media/image47.png"
style="width:3.08333in;height:4.40625in" />

To add a new callout, double -click on the Auto Start Callout box at the
bottom, navigate to your desired callout and press ‘open’. Then enter
the time, in seconds, when you want the callout to be played. Click
‘Add’. To remove a callout, select the callout from the list at the top
and click ‘Remove’ below.

In this example, a file named rs_300w.wav (“race starts in five
minutes”) will be played when the timer gets to 301 seconds before the
race starts.

###  

### Heats

<img src=".\/media/image97.png" style="width:7.5in;height:4.43056in" />

If you are running heats, you can select from many different options:

- Practice

- Custom Round Robin Sequence

- Single Heat (Solo/Any Lane)

- Single Lane

- Single Lane (Solo)

- Round Robin

- Euro Round Robin

- Friendly Round Robin

- Custom Rotation

#### Practice

A Practice race is a very specific race format that allows free for all
access to the track. By-default laps and lap times are displayed for
each lane and the data can be reset per lane as drivers are on and off
the track. If this format is selected, a small set of guided questions
will be asked specific to the Practice format. \[I didn’t see that\]

Practice races can be only time based. However, setting the time to 0
will allow them to run until the Race Director ends the session.

#### Custom Round Robin Sequence 

Create your own simple custom round robin. Enter the drivers in the
format of:

\[driver,driver,driver,driver…..driver\]

#### Single Heat (Solo/Any Lane)

A single lane (solo any lane) heat rotation is one where each driver
races alone on the track but can race on any lane the driver chooses.
The best score put in on a single lane is the score that counts for the
driver. This type of rotation is great for Sprint races, in which you
rank the drivers by their fastest lap time. \[ don’t understand the
example\]

<img src=".\/media/image5.png" style="width:2.64583in;height:3.75in" />

#### Single Lane

A single lane heat rotation is one in which each driver races on a
single lane in a single heat, but with others on the track at the same
time. Typically, with this rotation type, the drivers are allowed to
choose which lane they race on, by their seeding, thus giving the best
seeded driver in the heat a slight advantage.

To allow the drivers to choose their own lanes, the Race Director must
use the Manage Heats interface to change the lane assignments before the
heat starts.

#### Single Lane (Solo) 

A rally heat rotation is one in which each driver races on a single lane
in a single heat, with nobody else on the track. The driver is only
allowed to race in the lap they are assigned, which can be changed by
the Race Director before the heat begins.

### Round Robin Heat Rotation 

The most common heat rotations are round robins in which each driver
races once on every lane. Each round robin differs only by how the
drivers rotate from lane to lane, which includes both when a driver is
on the track and when they sit out, making them available to marshal or
work on their cars.

#### Round Robin 

A standard round robin rotation has every driver race in each lane once,
starting the first heat with the top seeds racing against each other.
After the heat ends, each driver moves over one lane with the driver in
the last lane moving to a sit out position. In a standard round robin,
the empty lane (lane 1) is then filler by the worst seeded driver
currently sitting out. This rotation continues until each driver has
raced on each lane.

#### European Round Robin 

A European round robin rotation has every driver race in each exactly,
such that no driver will ever drive next to the same driver twice.

#### Friendly Round Robin

A friendly round robin is considered ‘friendly’ to late joiners as, if a
driver is late, it affords then the longest time possible for the Race
Director to easily/automatically add the late driver into the race. \[I
don’t understand why this is the case…\]

A friendly round robin rotation has every driver race in each lane once,
starting the first heat with the top seeds racing against each other.
After the heat ends, each driver moves over one lane with the driver in
the last lane moving to a sit out position. In a friendly round robin,
the empty lane (lane 1) is then filled by the best seeded driver
currently sitting out. This rotation continues until each driver has
raced on each lane.

#### Custom Rotation

Custom Rotations are defined by the user in whichever format they
require.

Custom heat files define the heat rotation for a specified number of
drivers. Although the custom heat will work for any number of drivers,
if there are more drivers in the race than the custom heat supports,
some drivers will be left out of the race. Similarly if there are fewer
drivers in the race than the custom heat is set up for, some lanes will
be left unintentionally empty during the race.

To overcome this, the RMS supports supplying any number of custom heat
files to a race configuration. The RMS will select the custom heat file
that best matches the number of drivers in the actual race being run. If
there is a custom heat file with exactly the number of drivers in the
race that custom rotation will be used, otherwise it selects one as
close as possible.

If the race is configured for custom heat rotations, at least one custom
heat file must be added to the configuration.

Custom Round Robin rotations use a string of lane numbers to specify a
custom round robin format. Each value in the list represents the actual
lane the driver should be placed in (0 or a number greater than the
actual lanes on the track indicates a sit out). A lane number can not
appear more than once in the list as that would assign two drivers the
same lane in a given heat. If a lane does not appear in the list, that
lane will be empty for the entire race.

For example, using a 4 lane track as an example, \[1, 2, 3, 4\]
represents a straight round robin, \[1, 3, 4, 2\] represents a European
round robin, \[1, 0, 2, 0, 3, 0, 4, 0\] indicates a straight round
robin, but each driver will sit out every other heat, and finally \[1,
3\] indicates a straight round robin, but only using lanes 1 and 3 on
the track.

\[this needs someone cleverer than me to check this and perhaps write
out a formatted spreadsheet or whatever, as an example\]

\[this section needs a manual by itself\]

When you have chosen a heat type, the heats and groups (see below) will
be updated and visible in the window.

<img src=".\/media/image98.png"
style="width:5.08333in;height:5.30208in" />

Clicking on the Reverse Rotation will update your chosen heat type but
in reverse.

Click Update\>\> to save.

## Scoring

<img src=".\/media/image57.png" style="width:7.5in;height:4.69444in" />

The scoring tab allows you to determine how the driver positions are
decided.

###  **Heat Ranking Method**

<img src=".\/media/image53.png"
style="width:2.92046in;height:2.71025in" />

#### Ranking

This option determines what is used to decide the ranking of the drivers
for a heat:

- Lap

- Fastest Lap

- Total Time

#### Breakout Parameters

##### Breakout Time

Set the breakout time for a race. This time is the minimum lap time a
driver can achieve and have the lap be counted. If the driver
undershoots the breakout time, the driver is penalised as the lap will
not be counted. This differs from the 'Min Lap Time' in that the 'Min
Lap Time' protects against false laps being triggered for some reason.
The breakout time evens the playing field by forcing faster cars to run
slower laps allowing you to race any class car against any other class
car. 0 means this setting is disabled.

##### Breakout Percentage

The breakout percentage defines the breakout time relative to the
fastest lap. For example:

- If the fastest lap is 5.00 seconds

- And the breakout percentage is set to 90%

- Then the breakout time is 5.00 × 0.90 = **4.50 seconds**

So any lap faster than 4.50 seconds would “break out” and be
disqualified or penalized, depending on your settings.

#### Tiebreaker

In the case of two or more drivers finishing on the same number of
points, a tiebreaker may be deployed. The options available are:

- None

- Fastest Lap Time

- Average Lap Time

- Median Lap Time

- Total Lap Time

### Overall Ranking Method

###  <img src=".\/media/image125.png"
style="width:2.52067in;height:3.33142in" />

This option determines what is used to decide the ranking of the drivers
overall.

#### Accumulate Heats

If you want to accumulate the score a driver gets in each heat, to
compose the driver’s overall standings score, select the box. Not
selecting it will mean that the driver's *best* heat will be taken to
determine their overall score.

#### Step Up

A step up race is one in which the winner(s) of a sub-race advance
forward, stepping up to the next sub-race. Ultimately the winner of the
last sub-race is the winner of the entire race. This type of race is
typically used after a qualifying race and allows the lowest seeded
drivers to win their way up to the winners circle.

Tick the box to enable Step-Up races.

##### Number to Step Up

Set the number of drivers to step up to the next race. This number must
be at least one but must be fewer than the number of drivers
participating in each sub-race.

##### Drop Lowest N Heats

When accumulating heat scores to determine a driver's overall score,
it's possible to drop the lowest N number of heats for each driver. This
allows a driver to have a bad heat(s) and still have a good overall
standing ranking by doing well in the other heats the driver is in.

##### Tiebreaker

In the case of two or more drivers finishing on the same number of
points, a tiebreaker may be deployed. The options available are:

- None

- Fastest Lap Time

- Average Lap Time

- Median Lap Time

- Total Lap Time

### Start Method

###  <img src=".\/media/image77.png"
style="width:3.17812in;height:2.96326in" />

Select a start method, as required

##### Hot Start

If you have track power connected to Race Coordinator, you can use this
option to disable power until the heat start sequence. This means that
false starts are not possible. If you want to enable false starts,
select this option, which leaves power on during the heat start
sequence.

##### Restart on False Start

If a driver has a false start, you have the option to restart the heat.
You can assign the false starting driver a penalty and setup for a clean
heat start.

Time penalty: assign a false starting driver a time penalty. This *only*
works if you have per-lane relays installed. The driver’s power will be
turned off for the time stated.

Lap penalty: assign a false starting driver a penalty in laps.

##### Start Behind Sensor

Start each heat behind the start/finish line. This means that the first
trigger of the sensor will be discounted, so that the lap counter
doesn’t start at one.

##### Start Next At Current Position

Start each heat at the track location where the driver left off in their
previous heat.

### Finish Method

<img src=".\/media/image71.png"
style="width:3.03657in;height:2.51704in" />

You can select the method you would like to end each heat.

- Time Limit: Select this option to set a time limit for the race.

- Lap Limit: Select this option to set a number of laps for the race.

You can end the heat as soon as the conditions are met.

<img src=".\/media/image59.png"
style="width:3.42188in;height:1.74421in" />

Allow drivers to finish a single lap, or race until every driver reaches
the end condition. If you allow each driver to complete a single lap you
can also have RC estimate the fractional lap the driver had achieved.

If you have chosen to score the heat by total time, it is strongly
recommended that you choose one of the allow finish methods, otherwise
drivers end up being ranked by who finished their last lap first.

##### Drift Time

Drift laps can only affect the outcome of a heat or a race if you are
using the race point system or season scoring AND those points systems
are configured to allocate bonus points based on fastest laps.

If you want laps that were completed by a driver that included
‘drifting’ to be eligible lap times for driver and race records, set the
amount of time immediately following a heat stoppage that a lap can
still be counted.

Setting this time to 0 means the moment a stoppage occurs (yellow flag,
heat end, etc.) no laps will be recorded.

##### Adjust Drift Laps

Discount laps that occurred with any yellow or red flags as potential
best laps. The lap itself still counts.

## Points

<img src=".\/media/image101.png"
style="width:3.99479in;height:3.06267in" />

### Use Points

Assign points to each driver, each heat to determine overall standings
by selecting the Use points box.

### Carry Over Percentage

The percentage of a driver’s heat score to carry over into the points
total for the driver. This can be used to award a driver for winning by
the largest margin possible.

For example, if this value is set to 50% and a driver had 30 laps in
their heat, they would be awarded an additional 15 points for their
overall point total.

### Heat Points

Enter the points you wish to give each based on their heat ranking. The
first entry in the list will be the points given to the first place
driver, the second entry to the second place driver, etc. – for example,
\[20, 18, 16, 15\]

If you specify fewer values than drivers in the race, all unspecified
placings will receive 0 points. More than likely this is the primary
source of points for the heat.

### Fastest Lap Bonus

The number of bonus points to assign the driver with the fastest lap
time in the race.

### Fastest Heat Lap Bonus

The number of bonus points to assign the driver with the fastest lap
time in each heat.

### Fastest Lap Per Lane Bonus

Set the number of bonus points to assign the driver with the fastest lap
time on each lane.

### Most Overall Laps Led

Set the number of bonus points to assign the driver with the most laps
led in the entire race.

### Led At Least One Overall Lap

Please set the number of bonus points to assign any driver who led at
least one lap in the overall standings.

### Led At Least One Heat Lap

Set the number of bonus points to assign every driver that led at least
one lap in each heat.

### One Lane Bonus Per Driver

Allow only a single lane bonus per driver, thus preventing the same
driver from getting all the lane bonuses. If selected, a driver with the
multiple lane bonuses will be awarded the one bonus they did the best in
and the second bonus will go to the next best driver on the second lane.

### Season

#### Season Points

To configure the race to use season points based on the overall
standings, you need to configure a season before you run the race. If
you don’t, 0 points will be awarded, even if you select a season when
you run the race.

<img src=".\/media/image28.png" style="width:3.3414in;height:5.416in" />

Enter the season points you wish to give each based on their overall
ranking. The first entry in the list will be given to the first place
driver, the second entry to the second place driver, etc.

If you specify fewer values than drivers in the race, all unspecified
placings will receive 0 points. More than likely this is the primary
source of season points for the race.

The points are administered in the following format:

\[20, 18, 16, 15, 14, 13, 12, 11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1\]

##### Carryover Percentage

Select the percentage of a driver's overall score to carry over into the
drivers season points total. This can be used to award a driver for
winning by the largest margin possible. For example, if this value is
set to 50% and a driver had 80 total laps in the race, they would be
awarded an additional 40 points to their season point total.

##### Race Points

Points given based on their ranking in each heat they race in.

##### Heat Points

Points given based on their ranking in each heat they race in.

##### Fastest Lap Bonus

Assign bonus points to the driver with the fastest lap time in the race.

##### Fastest Heat Lap Bonus

Assign bonus points to assign the driver with the fastest lap time in
each heat.

##### Fastest Lap Per Lane Bonus

Assign bonus points to the driver with the fastest lap time on each lane
in the race.

##### Bonus Points

Allow a single lane bonus per driver, thus preventing the same driver
from getting all the lane bonuses If selected, a driver with the
multiple lane bonuses will be awarded the one bonus they did the best
in, and the second bonus will go to the next best driver on the second
lane.

## Analog Fuel

The RMS can be configured to simulate fuel usage. When fuel races are
enabled, cars will use fuel after each lap they complete. You can
configure both how much fuel is used per lap, where faster lap times use
more fuel than slower lap times and you also get to configure how fast
you refuel when a car makes a pit stop. So how often you need to refuel
and how long you need to refuel for are completely up to you.

Depending on your track interface you can either make a pit stop by
stopping the car at the lane sensor (IR, photo, reeds) or in more
advanced interface setups you can create pit ranges in which you only
have to stop between two sets of sensors.

### <img src=".\/media/image81.png"
style="width:5.48711in;height:6.00208in" />

#### 

#### Fuel Usage

How often a driver must make a pit stop is determined by a combination
of the car’s fuel capacity, how much fuel a car uses, a reference lap
time and which usage curve that is chosen. Drivers running faster laps
use more fuel than drivers running slower laps.

Using the default configuration as an example, the first graph will show
a driver running a lap of about 3.5 seconds, which will use about 40
units of fuel. Similarly, the graph shows that a driver running a 6.95
second lap shows that they will use about 10 units of fuel.

The second graph shows approximately how long it will take a driver to
run out of fuel, if they run the same exact lap time each lap. For
example, it shows that under the default configuration, a driver running
a constant lap time of 6.95 seconds will have to make a pit stop after
about 60 seconds. Using these two graphs you can tune how often other
drivers running various lap times will need to refuel.

Using a linear fuel usage curve, fuel is used at a rate of:

(\[reference lap time\]/\[actual lap time\]) \* \[usage per reference
time\]

#### Use Fuel

Select this option if you want this race to be a fuel race.

#### Heat Reset

Select this to reset fuel levels at the start of each heat

#### End Heat

Select this to end a driver’s heat when they run out of fuel.

#### Capacity

Set how much fuel each car can hold after refueling. The actual fuel
consumed will be calculated by taking the ratio of the drivers actual
lap time to one second and this value.

#### Usage Type

Linear, Quadratic, Cubic. \[needs more information\]

#### Reference Lap Time

Time in seconds to use the maximum fuel per lap allowed.

#### Usage Per Reference Time

Maximum fuel to be used per lap time. For example, if a driver's lap
time is 3 seconds, the actual consumption will be this value multiplied
by (1.0 / 3.0).

#### Fuel Start Level

Set how much fuel each car will start with. This value can be higher or
lower than the cars’ capacity and is only used for the driver’s first
heat and if you chose to reset fuel levels at the start of each heat.

#### Refuel Rate

Set the refuel rate in units per second.

#### Pit Delay

Set the minimum amount of time, in seconds, before beginning a pit stop.

#### Pit Delay Max

Set the maximum amount of time, in seconds, before beginning a pit stop.

Fuel Usage \[I don’t know what these paragraphs refer to\]

How much fuel would you like at full throttle per second? The actual
fuel consumed will be calculated by multiplying this value by the
throttle percentage and scaling that value to the amount of time the
throttle is at that level.

For example, if a driver is at half throttle for 0.25 seconds, the
actual consumption will be this value multiplied by 0.5 and then scaled
to a per second value by multiplying it by 0.25",

Pit Lane Throttle Percentage

Please set the maximum speed allowed when driving down the pit lane. If
set to 100%, drivers can go full speed through the pit lane, but if set
lower, the driver's throttle level will be reduced by this percentage."

Fuel Weight Throttle Curve

For added realism, a car's maximum speed can be adjusted by the amount
of fuel the car currently carries. The two values below control at what
fuel level the car will be allowed to go full speed and how much to
reduce the car's speed at full fuel. The graph shows how various fuel
levels affect the throttle based on these parameters.

## Crash n Learn

A crash and learn race is a race in which a driver can be penalised
and/or disqualified from the race/heat if they crash too often.
Hopefully, after enough penalties, they will learn to drive the track
without deslotting.

Crashes are detected either by lap times that are too long or by a
driver using an installed per-lane callbutton.

<img src=".\/media/image60.png"
style="width:3.90319in;height:5.44305in" />

### General Preferences

#### Enabled

Tick to enable the Crash n Learn options.

#### Crash Time

Set the maximum time, in seconds, allowed for a driver to pass the
start/finish line before the driver is assumed to have crashed. If set
to 0, no automatic crash calculations will be done.

#### Yellow on Crash

Automatically trigger a yellow flag anytime a driver crashes.

#### Maximum Crashes

Set the maximum number of times a driver can crash before being
disqualified. Once disqualified, a driver will not be credited with any
further laps and is subject to other penalties based on configuration.
Setting this value to 0 will allow a driver to crash without ever being
disqualified.

#### Multiple Crashes

Allow multiple crashes for a driver in a single lap.

#### Heat Reset Crashes

Reset a driver's crash count at the start of each heat.

#### Heat Reset DQ

Reset a drivers DQ (disqualified) state at the start of each heat.

###  

### Penalties

<img src=".\/media/image70.png"
style="width:3.73887in;height:5.6335in" />

#### Heat Crash Lap Penalty

Set the number of laps to penalize a driver when they crash. This
penalty is above and beyond any delays in the detection of the crash
itself.

#### Heat Crash Time Penalty

Set the time to penalize a driver when they crash. This penalty is above
and beyond any delays in the detection of the crash itself. If you have
per lane relays installed, lane power for the driver will be turned off
for this amount of time. If not, this time will be applied to the
drivers score, which depending on the race configuration may or may not
be meaningful.

#### DQ Heat Score Pct

Set the percentage of a driver's heat score to use for the driver when a
driver DQ's. This value only affects the position of the heat itself and
does not directly impact the overall standings unless the driver's heat
position affects the overall standings as it does in a points race.
Setting this value to 100% will not penalize the driver for a DQ.

#### DQ Heat Overall Score Pct

Set the percentage of a driver's heat score to use towards the overall
standings. If set to 100%, the driver will not be directly penalized in
the overall standings for a DQ.

## UI

The User interface is where the driver-facing screens are defined. These
appear when the Race Director starts the race.

The RMS supports configuration options for displaying images and sorting
the driver heat data by the drivers heat positions. It does this by
providing different XAML files for each possible configuration option
chosen. Each file provided uses a naming convention so the RMS can find
it.

If the file chosen here has an '\_' in it, then it is assumed you are
using set files that correspond to the various questions you've already
answered and the RMS will choose the correct file from the set. If the
correct file from the set can not be found, or the file does not contain
any '\_' in it, the file will be used exactly as selected here.

<img src=".\/media/image18.png"
style="width:4.44271in;height:4.29385in" />

### Show Images

This will display extra images like driver and car images on your Race
Day screen.

### Sort By Heat Standings

Selecting this will sort the driver rows by heat standings on your Race
Day screen in realtime.

### RaceDay XAML File Prefix

Select the Race Day Xaml file you would like to use to display heat data
for this race.

### Example Full File Name

\[never really understood this\]

### Race Start XAML File

Path to the XAML Race Start file.

### Restart XAML FIle

Path to the XAML Race Restart file.

### Start Delay

Time, in seconds, to wait before starting the race start countdown.

### Restart Delay

Time, in seconds, to wait before starting the race restart countdown.

### Start Randomizer

Maximum time, in seconds, to randomly wait before starting the race
starts after the countdown.

### Restart Randomizer

Maximum time, in seconds, to randomly wait before starting the race
restarts after the countdown.

## Groups

Groups allow you to separate drivers from each other so that no matter
what other race configurations you have set up, drivers in separate
groups will not race head to head together in a heat. Using groups also
allows you to force one or more drivers from each group to be placed at
the top of the leader board regardless of the actual scores for the
drivers, which can be very useful for specific types of qualifying
races.

Driver group assignments are made strictly by the drivers seeds and the
number of groups created by your configurations.

<img src=".\/media/image88.png" style="width:7.5in;height:4.84722in" />

### Use Groups

Select this box, if you want to run this race using driver groups.

### Use Teams

\[?????\]

### Max Groups

Select the maximum number of groups to use. Once this number of groups
is created, drivers will be distributed between the groups rather than
creating new groups.

### Num Teams

Number of teams the race consists of. \[????\]

### Min Advancing

Select the number of drivers from each group to always rank highest in
the overall standings despite their actual overall score.

The number of drivers to advance is the number of drivers from each
group to force to the top of the standings. These drivers are forced to
the top in a round robin fashion by group.

For example, if this value is set to 2 and there are 4 groups in the
race, the 1st and 5th place drivers in the overall standings will be the
top 2 drivers from group 1. The 2nd and 6th place drivers will be the
top 2 from group 2, the 3rd and 7th place drivers will be from group 3,
and the 4th and 8th place drivers will be from group 4. The remaining
drivers in the overall standings will be taken from the remaining
drivers based on their scores regardless of the group they are in.

The overall standings always show the standings in this fashion, however
there is a group leader board that shows only the standings for a
particular group.

### Balance

Select this if you would like to balance driver seeds within the groups.

The RMS can assign drivers to groups in two ways. If you choose to
balance seeds then the RMS will round robin the drivers into the groups
used. If you choose not to balance the seeds the top seeds will be used
to fill the first group, then the next highest seeds will be used to
fill each remaining group.

For example, if your max groups setting is 2, selecting balancing seeds
will cause all the even seeds to be in one group and all the odd seeds
to be in the other. On the other hand if you do not balance seeds, the
top X drivers are assigned to the first group, then the next Y drivers
are assigned to the second group.

### Allow Empty Lanes

Select this if you want to allow groups to race heats with empty lanes.

Allowing empty lanes means that when setting up the groups, there can be
fewer drivers in the group than lanes on the track, thus creating heats
with empty lanes in one or more heats for the group.

If not allowed, the number of drivers in each group is forced to be at
least the number of lanes on the track. New groups will not get created
until there are enough drivers in each group such that there would be no
empty lanes in a heat.

Allowing empty lanes will have the effect of creating more groups with
fewer drivers in each group. Not allowing empty lanes will create fewer
groups with more drivers in each group.

### Force Multiple of Max

Select if you want to force the number of groups to be a factor of the
maximum number of groups allowed. The actual number of groups will
depend on the number of drivers and your other configuration options. If
you do not force a factor of the max, your group count will be between 2
and the maximum number set. For example, if it is set for a maximum of 6
groups, then ???? \[I still can’t get my head round this\].

This is a very useful option if this group race is not the final race in
your event and you want to advance an even number of drivers from each
group to the next race.

### Rotate Group Heats

Select this if you like to run your heat rotation by rotating each group
on and off the track.

## Images

Select the image you want to use for particular aspects of the race.

<img src=".\/media/image104.png"
style="width:4.41146in;height:6.03125in" />

Double click on the image you want to change and navigate to your new
image.

## Audio

<img src=".\/media/image76.png"
style="width:5.92768in;height:6.41342in" />

For any audio resource in the RMS, if the entry specified is not a valid
file to play, the text will be spoken using Text to Speech technology.

If the audio resource is one that plays from a sequence of files, such
as the 'Fuel Warning Prefix' or the 'Audio Start Prefix', you can
specify a series of Text to Speech entries as a json array. The array
format is \["First sound", "Second sound", ... \]. Each sound in the
list will be played as if they were the \_0, \_1, \_2, etc entries the
normal prefix file represents and each entry can be either a valid file
to play or Text to Speech text.

If you do not want a sound to play for a particular resource simply put
an empty string ("") as the configuration value.

Text to Speech can play callout times and other information relevant to
the sound being played. If the following exists in the configuration
they will be replaced with data from the Race:

- %n : Will play the drivers name

- %nn : Will play the drivers nickname

- %l : Will call out the lane number the driver is in

- %c : Will call out the lane color the driver is in

- %t : Will call out the relevant time for the callout

NOTE: For the 'Practice Best Lap Audio Prefix', if you want Text to
Speech you MUST specify it as a json array with a single value in it.
For example \[\\Lane %l best lap %t\\\] will call out 'Lane 2 best lap
3.134' when the driver in lane 2 gets their best lap.

***\[I think we need to go in to more detail on this section\]***

### Heat Callouts

These are the audible messages used to, in this example, to call out how
long before the next heat will start and when to play the message.

<img src=".\/media/image89.png"
style="width:4.09916in;height:1.79338in" />

To add a new callout, double click on the Heat Callout Info box,
navigate to your desired callout and click ‘open’. Then enter the time,
in seconds, when you want the callout to be played and click ‘Add’. To
remove a callout, select the callout from the list at the top and click
‘Remove’ below.

# Event Setup

In the RMS an Event is a series or races run in succession. The outcome
of each race seeds the next race in the event until the final race is
completed and an overall event winner is determined.

<img src=".\/media/image72.png"
style="width:3.35938in;height:1.02435in" />

Some races (like Practice) do not affect the next race. Others will
determine seeding for the next race, while still others will determine
both seeding and how many drivers actually move on to the next race.
While winning the intermediate races is important for seeding the next
race and qualifying a driver to move on to the next race, the winner of
the last race in the event is the overall event winner.

The first race in the event will have its seeding taken from the order
the drivers appear in the Drivers Racing list on the Race Day Setup
screen. All subsequent races will take their seeding from the standings
of the previous race. No more drivers can participate in a race for an
event than are specified by the race in the event. If there are too many
drivers, the field will be reduced by dropping the lowest seeds from the
previous race. This is very useful for advancing drivers from a
qualifying race to a finals race.

<img src=".\/media/image108.png" style="width:7.5in;height:4.31944in" />

This Wizard will walk you through setting up all aspects of an Event.
The table of contents to the left provides both quick access to the
different properties of an event as well as color codings that indicate
those properties' status. A red property indicates that the property
contains an invalid value. For text properties this is most likely
caused by the field needing to be unique or it is left empty. For
numeric values, either the value contains invalid characters (like
letters), the value is out of the expected range, or the value is a
decimal when an integer value is expected. A blue property in the table
of contents indicates the current property being viewed and a yellow
property indicates a property that has been changed from its default
value. If a property is red, this wizard will not let the event be
created.

## Races and Events

### Races Available

This is the list of races that have been created already that can be
used for an event. See Race Setup to create new races.

### Drivers

Number of drivers advancing to this race. 0 for all drivers.

### Current Races

These are the races that have already been selected for a race. Clicking
on a current race will show the number of drivers advancing to this
race. Over-typing the number of drivers and pressing “Update\>\>” will
set the new value.

### Current Events

This is a list of the events already created.

### Name

Give your event a unique name before clicking “Add\>\>” at the bottom
right.

### Auto Advance Time

Time, in seconds, to automatically advance to the next race in the
event. 0 for no auto advance.

## Event Creation

To create an event:

1.  Select a race from the races available:

    1.  Type a number of drivers to advance from that race to the next
        race in the event. (use 0 for all drivers).

    2.  Click “Add\>\>” in the middle. The race selected will appear on
        the right.

2.  Repeat 1) as often as required for the number of races required for
    your event.

3.  Type a unique event name in the Name box.

4.  Set the auto advance time (0 for no auto advance).

5.  Click “Add\>\>” in the bottom right hand corner. Your new event will
    appear in the top right, with the number of races in your event.

# Season Setup

<img src=".\/media/image114.png"
style="width:3.87267in;height:1.07116in" />

Similar to event setup, a season is a number of events (think number of
grand prix in a year). When all the boxes are complete, click “Add\>\>”
to save the new
season.<img src=".\/media/image99.png" style="width:7.5in;height:4.26389in" />

## Season Name

A unique name for the season.

## Drop N Worst Races

How many of a driver’s lowest scores will be dropped from their total
score.

# Options

<img src=".\/media/image87.png"
style="width:3.32813in;height:1.72178in" />

Under the Options menu, there are various ‘choices’ that can be made
about RC.

##  

## Stats

Stats show various aspects of races that have been run already.

<img src=".\/media/image45.png"
style="width:7.36979in;height:4.95911in" />

To export data, select a race, and press ‘Export’

The data is exported in .xlsx format.

<img src=".\/media/image49.png"
style="width:6.32813in;height:4.1748in" />

All aspects of the race are saved:

<img src=".\/media/image54.png"
style="width:3.40602in;height:1.36408in" /><img src=".\/media/image58.png"
style="width:3.42188in;height:1.45716in" />

<img src=".\/media/image48.png"
style="width:3.38511in;height:1.49575in" /><img src=".\/media/image39.png"
style="width:3.42188in;height:1.78934in" />

Lane data can be edited from RC: <img src=".\/media/image84.png"
style="width:5.45812in;height:5.81441in" />

Select the appropriate lane and increase the Number of Rejected Laps.
This will remove the hughes result for that lap.

##  

## Reset Windows

If you want to clear ALL the data stored on RC back to its default, then
select Reset Windows. Note: **This deletes ALL information and
configuration.**

##  

## Show Tips

At the start up of RC, the “Tip of the Day” is displayed. If you no
longer wish to see these tips, they can be switched of here.

<img src=".\/media/image15.png"
style="width:5.24016in;height:4.75561in" />

##  

## Preferences

<img src=".\/media/image46.png"
style="width:4.86196in;height:5.13733in" />

Preferences allow the configuration of four aspects of RC: Demo
Settings; Multi-Track; Debugging; and Web Server (RCLive).

###  

### Demo Settings

Minimum and Maximum reaction times can be set. This is the time taken
between the start of the race and the time the car moves. It is only
used on race screens, where reaction times are shown.

Minimum and Maximum lap times can be set. This means that you can
control approximately how long the demo race will last. So if you have a
max lap time of 10 seconds and the number of laps in the race as 5, each
demo race will take no more than 50 seconds.

###  

### Multi-Track

Tick this if you have more than one track to be used in an event or if
you have one track but multiple connections to it (see Race Setup), you
must enableMulti-Track.

###  

### Debug

This should be changed only if requested by the administrator of RC.

###  

### Web Server (RC Live)

As well as the ‘normal’ race page, shown when pressing Start on the main
screen, a web screen is available.

RC has its own web server and can, therefore, allow connections to it.
Information on RCLive can be found in the RC Live Section but, to enable
it, and use it, these options must be set.

Web Server - enables the web server

Listener port - is the port on the pc that the browser connects to

Server Base Directory - where the home screen can be found on the pc

Default Page - the home screen file name

Server Cache Size - cache size in MB (0 means no cache stored)

Race Director Password - this can be changed from the default.

Press Accept to update these options.

Note: After selecting the Web Server option and accepting, you may get
the following ‘error’

<img src=".\/media/image75.png"
style="width:3.70833in;height:1.36671in" />

If this happens, restart RC as an administrator by right-clicking Race
and selecting ‘Run as administrator.

<img src=".\/media/image2.png"
style="width:2.41146in;height:1.81586in" />

> 

# Getting Ready for a Race

## Overview

**T**he Race Day Setup (RDS) module (window) in Race Coordinator is
designed to facilitate the configuration and management of race day
events, allowing users to select cars, drivers, and the type of race /
event. The module includes various features and options to customize the
race experience.

This main dialog puts all the data entered together to configure the
particular race you want to run. Drivers are added or removed as needed.
Drivers that are added to the race can be assigned a car. Race selection
is made and the heats are assigned.

All data entered in this dialog is saved from run to run, so as long as
the data entered exists, you can run the same race over and over again
just by clicking ʻStart Raceʼ.

<img src=".\/media/image51.png" style="width:7.5in;height:4.55556in" />

##  

Note: No configuration takes place on the RDS screen. That is all done
in the various menus, selectable in the top row of the screen.

## Cars Available

This section lists all the cars available for the race. Users can add or
remove cars as needed by dragging the car to the Drivers Racing section.
Assigning cars is optional.

<img src=".\/media/image64.png"
style="width:2.54282in;height:3.54681in" />

## Drivers Available / Drivers Racing

The Drivers Available section shows all drivers available to participate
in the race that have not already been assigned; Drivers Racing shows
all drivers assigned to the race. Drivers can be added to or removed
from the race by either dragging and dropping or by the provided
controls in the Options section of the
window.<img src=".\/media/image80.png"
style="width:3.18117in;height:2.56441in" />

You can drag each driver you want in the race from the "Available
Drivers" pane to the "Drivers Racing" pane in the desired seed position.
If you drag a new driver on top of an existing one, all the drivers will
be pushed down to make room. To remove a driver from the race, simply
drag the driver from the "Drivers Racing" pane to anywhere outside the
pane. The driver removed will reappear in the "Available Drivers" pane.
All drivers seeded lower than the removed driver will automatically move
up one seed.

You can change the drivers initial seed by dragging the driver in the
"Drivers Racing" pane to the new seed location. If the new seed location
is taken, the two drivers will swap seed
positions.<img src=".\/media/image38.png"
style="width:4.36904in;height:2.27797in" />

To use ghost drivers in a race you must create one or more using the
Driver Wizard or Expert Driver Setup. You can create as many different
ghost drivers as you want. And a race can have up to as many as you
create added to the race at one time.

Ghost drivers can be added to a race in two ways. First, if the race is
configured to "Add Ghost Cars" any heat that has fewer drivers than the
track allows will have ghost drivers added. You can also manually add a
ghost driver to any race making them part of the actual heat rotation.

The drivers, their avatars and cars (if assigned) can be seen in the
race screen, if the race screen is configured to display them.

<img src=".\/media/image103.png" style="width:7.5in;height:4.47222in" />

## Options

This section provides some quick ways to assign drivers, as well as
various options to customize the race setup, including demo mode and
debug options.

### Quick Driver Assignment Controls

The four buttons at the top of the Options section provide quick ways to
assign drivers.

<img src=".\/media/image41.png"
style="width:2.48028in;height:2.40441in" />

Add All\>\> This empties “Drivers Available” and adds all the drivers to
the “Drivers Racing”.

Randomize\>\> Randomises the drivers in “Drivers Racing”.

\<\<Remove All This empties “Drivers Racing” and adds all the drivers to
the “Drivers Available”.

\<\<Remove All Cars If car images have been added to the drivers in
“Drivers Racing”, this will remove the cars.

###  

### Race Type / Race/Event Selection

<u>Single Race</u>: An individual race, with the drivers selected.

<img src=".\/media/image36.png"
style="width:2.60533in;height:2.54775in" />

Any races set up may be chosen from the drop down list, selectable when
Single Race is selected in the Race Type.

<u>Event</u>: An event describes multiple races and is configured in
Event Setup.

<img src=".\/media/image23.png"
style="width:2.46224in;height:1.65066in" />

Any events set up may be chosen from the drop down list, selectable when
Event is selected in the Race Type.

### 

### Season Selection

This dropdown allows users to select the racing season for the event.

<img src=".\/media/image65.png"
style="width:2.86979in;height:1.28345in" />

### 

### Demo Mode

<img src=".\/media/image11.png"
style="width:2.34178in;height:1.52344in" />

If Demo Mode is selected, then all the drivers, race/events and screens
can be seen in action, without having to connect to a track. This gives
the user a feel for how it will look with real drivers.

Note: Demo Mode does NOT support connection to external devices, such as
lights or track relays. This can be done ONLY if Demo Mode is unchecked.

To see the race start, press Start Race or keyboard shortcuts Ctrl R or
Alt R.

# Running a Race (Race Day)

## Overview

Once the track, cars, drivers and race format are configured, it’s time
to run a race! Clicking the ‘Start Race' button in the Race Day Setup
screen opens the Race Day window - one example of this screen is shown
below:

<img src=".\/media/image14.png" style="width:7.5in;height:4.02778in" />

Your Race Day window will vary, depending what you have chosen for
number of lanes, analog fuel, etc. The screen can also be customized -
see chapter [<u>Race Screen Customization
(XAML)</u>](#race-screen-customization-xaml) for details. It is from
this window where the racers can view the status of heats, and where the
Race Director can control the race. Additional windows can be displayed
to show overall race leaders, the list of heats, heat results, etc.

## File

Races can be saved or exported via the File menu.

### Save / Save As

You can save a race anytime during the race as long as the race is
paused. From a stat point of view only the last time you complete the
race will be saved and recorded. You DO NOT have to manually save a race
to preserve its stats. Race Coordinator saves your stats automatically
when you get the checkered flag. Saved races are in JSON format.

### Export

Use Race Day File \> Export to export race information <u>during</u> the
race. Use the Race Day Setup window’s Options \> Stats menu to export
them <u>after</u> the race is over. Exported races are saved in
Microsoft Excel .xls files. The amount and format of information in
exported .xls files is determined by the template file. A default
template file, defaultTemplate.xlsx, is provided; it is located in
directory C:\Program Files (x86)\Race Coordinator\data\xls. The default
template organizes the exported data across several tabs:

- Heat List

- Overall

- \#Heats

- Fastest Laps

- Season

- \#SeasonRaces

- Graph Data

## Race Director

The Race Director menu provides the Race Director control over the heats
and the overall race. You can modify race heats at any point during the
race; the only limitation is that you can not change heats that have
already been run. Commands available are:

- Start/Resume Heat

- Pause Heat

- Add Lap/Sections - Provides a way to adjust results at the end of a
  heat; sections (fractions of a lap) as well as total lap time can be
  added or subtracted from each driver. This is often used in time-based
  heats.

- Next Heat - Jump to the next heat.

- Restart Heat

- Defer Heat - Moves the current heat to the end of the race.

- Skip Heat - Skips over the remainder of the current heat.

- Skip Race - Ends the race.

- Modify Heats - Brings up the *Manage Late Joiner* screen to add in
  drivers / adjust driver assignments to heats after racing has started.
  This includes adding new drivers and/or entirely new heats to a race
  in progress. If you have a late arrival, with most race configurations
  you can simply modify your race heats to add the heat they're in to
  the end of the race and then simply skip the heat the no show is in.
  This will delay when the no show actually needs to be on the track,
  allowing them time to arrive without holding up your race.

- Edit Laps

## Track Power

The Track Power menu provides on / off control of overall Track Power as
well as each individual lane (if the track is configured for per-lane
power control). The number of commands in this menu will depend on how
many lanes are configured for the selected track.

## Windows

The Windows menu provides the means to display additional status
windows, such as Leader Board, Heat Results and On Deck list. Multiple
windows can be sized to fit on one PC display; if the PC can support
multiple displays, multiple windows can be spread across those displays
as desired.

# Race Screen Customization (XAML)

## What is XAML?

XAML (e**X**tensible **A**pplication **M**arkup **L**anguage) is a
simple way to design on-screen layouts using text. It’s used in Race
Coordinator to describe what the layout looks like, where things go,
which fonts or sizes to use and which fields to show (like lap counts,
names, avatars, etc). It works a lot like HTML for websites but focused
on screen layouts.

Note: this is not an extensive tutorial on XAML: it’s more of a guide as
to how XAML works within Race Coordinator and some ideas on creating
your own files.

## Why Does Race Coordinator Use XAML?

Race Coordinator separates the **layout** (where things go) from the
**data** (the actual results and driver info). That means you can update
your layout file without touching the software or writing any real code.

Using XAML lets you:

- Place fields exactly where you want them

- Change fonts, colours, image sizes and styles

- Build overlays, race boards, and result screens that match your needs

## How Does Race Coordinator Use XAML?

The main race screen is loaded from an XAML file and is, therefore, 100%
customizable within the limits of what is currently supported. To
accomplish this, named elements in the XAML file represent specific data
values within a race, which update real-time during a race.

There are three types of data types that can be accessed in the XAML
file. They are:

- Generic Data: not associated with a specific racer. For example, track
  information, heat status information, or race status information

- Racer Data: associated with a particular racer. This includes heat
  data and overall data and includes things like name, nickname, lap
  times, etc.

- Action Data: commands to control the heat. These commands are only
  available at certain times throughout the heat, and the action is only
  performed when the element is selected.

Each of the ‘Racer Data’ fields normally require a postfix:

- \_Lane\<#\>: The data requested is for a racer in a specific lane on
  the track.

- \_Position\<#\>: The data requested is for a racer in a specific
  position in the heat (useful to display the heat standings).

- \_RaceLeader\<#\>: The data requested is for a racer in a specific
  position in the entire race (useful for a leader board). e.g.
  Lap_RaceLeader8

- \_GroupLeader\<#\>: The data requested is for a race in the currently
  heats group in a specific position in that group (useful for a group
  leaderboard).

- \_TeamLeader\<#\>: The data requested is for a team in a specific
  position in the entire race (useful for a team race leaderboard).

- \<Name\>\<#\>: There are a few exceptions, for example,
  NextTeamNickname1

where \# is an integer.

The ‘\_Lane’, ‘\_Position’ postfixes and the standalone names (like
NextTeamNickname1) request data for a racer in the current heat. The
racer is, therefore, in a specific lane on the track and the background
colour of the label or name will automatically be changed to the lane
colour specified in Race Coordinator. ‘\_RaceLeader’, ‘GroupLeader’ and
‘TeamLeader’ suffixes do not necessarily have a lane assignment and the
background colour is left alone.

## Example Data Types

The following is an example of elements supported in RC and the way to
name them to get real-time updates.

<table>
<colgroup>
<col style="width: 14%" />
<col style="width: 20%" />
<col style="width: 18%" />
<col style="width: 46%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>DATA TYPE</strong></th>
<th style="text-align: center;"><strong>XAML ELEMENT TYPE</strong></th>
<th style="text-align: center;"><strong>NAME</strong></th>
<th style="text-align: center;"><strong>DESCRIPTION</strong></th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>TrackName</p>
</blockquote></th>
<th>Displays the track name of the race being run.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>RaceTime</p>
</blockquote></th>
<th>Display how much time is left in the heat. It will count down for
timed heats and it will count up for lap based races.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>RaceLaps</p>
</blockquote></th>
<th>Displays how many laps are left in the heat. It will count down for
lap based heats and will count up displaying the heat leaders lap count
for time based races.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>EndHeatValue</p>
</blockquote></th>
<th>Displays the number of laps required to end the heat in a lap based
race, or the time in seconds that ends the heat in a time based race.
This value does not change throughout the race.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>RaceName</p>
</blockquote></th>
<th>Displays the name of the race being run.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>RaceFilter</p>
</blockquote></th>
<th>Displays the filter of the race being run. If set to ‘Unlimited’ any
car is available for this race. If set to ‘Practice’ there are no heats
and any driver can race any car. If set to a specific car type, only
cars of that type are allowed to race.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>HeatNumber</p>
</blockquote></th>
<th>Displays the current heat number.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>NumHeats</p>
</blockquote></th>
<th>Displays the total number of heats in the race.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Name</p>
</blockquote></th>
<th>Driver’s real name.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Nickname</p>
</blockquote></th>
<th>Driver’s nickname.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Lap</p>
</blockquote></th>
<th>Lap count for the driver.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>LapTime</p>
</blockquote></th>
<th>Driver’s last lap time.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>ReactionTime</p>
</blockquote></th>
<th>Driver’s reaction time off the line at the start of the heat.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>AverageTime</p>
</blockquote></th>
<th>Driver’s average lap time.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>BestLapTime</p>
</blockquote></th>
<th>Driver’s best lap time.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>GapLeader</p>
</blockquote></th>
<th>Driver’s time gap between him/herself and the race leader. This
value will be negative for drivers not in the lead, and positive for the
race leader.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>GapPosition</p>
</blockquote></th>
<th>Driver’s time game between him/herself and the driver one position
ahead. This value will be negative for everybody but the leader who will
have a positive gap time.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>TotalLaps</p>
</blockquote></th>
<th>Driver’s total number of laps completed across all heats.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>TotalTime</p>
</blockquote></th>
<th>Driver’s total lap time accumulated across all heats.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Label / TextBlock</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>TotalExtendedTime</p>
</blockquote></th>
<th>Total time a driver has raced beyond the actual heat time across all
heats. This time is only accumulated in Allow Finish races that end the
heat based on time.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Image</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>TrackImage</p>
</blockquote></th>
<th>Display the image for the track being raced on.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Image</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>RaceStateImage</p>
</blockquote></th>
<th>Displays one of the state images set up by the ‘&lt;color&gt; Flag
Image Path’ in the Manage/Track Dialog.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Generic Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Image</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>StartLamp&lt;#&gt;</p>
</blockquote></th>
<th>Displays the ‘&lt;Red/Yellow/Green&gt; Flag Start Image Path’ image
setup in the Manage/Track Dialog based on how much time is left in the
start countdown.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Image</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Avatar</p>
</blockquote></th>
<th>Displays the driver’s image.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Racer Data</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Image</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>CarImage</p>
</blockquote></th>
<th>Displays the driver’s car image.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Action</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Button / MenuItem</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Start</p>
</blockquote></th>
<th>When selected, start the race.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Action</p>
</blockquote></th>
<th style="text-align: left;">Button / MenuItem</th>
<th style="text-align: left;"><blockquote>
<p>Pause</p>
</blockquote></th>
<th>When selected, pause the race.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Action</p>
</blockquote></th>
<th style="text-align: left;">Button / MenuItem</th>
<th style="text-align: left;"><blockquote>
<p>AddLaps</p>
</blockquote></th>
<th>When selected, the lap adjustment dialog will come up. Laps are
adjustable at the end of every heat and only the racers in the heat can
have their laps adjusted.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Action</p>
</blockquote></th>
<th style="text-align: left;">Button / MenuItem</th>
<th style="text-align: left;"><blockquote>
<p>NextHeat</p>
</blockquote></th>
<th>Advance to the next heat.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Action</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Button / MenuItem</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>RestartHeat</p>
</blockquote></th>
<th>Stop the current heat and set it up to be started over. All lap data
will be lost.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Action</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Button / MenuItem</p>
</blockquote></th>
<th style="text-align: left;"><blockquote>
<p>Window</p>
</blockquote></th>
<th>Opens a new window. The ‘CommandParameter’ attribute specifies the
XAML file to load as the Window content.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Action</p>
</blockquote></th>
<th style="text-align: left;">Button / MenuItem</th>
<th style="text-align: left;"><blockquote>
<p>Dialog</p>
</blockquote></th>
<th>Opens up a new dialog. The ‘CommandParameter’ attribute specifies
the XAML file to load as the Window content.</th>
</tr>
<tr>
<th style="text-align: left;"><blockquote>
<p>Action</p>
</blockquote></th>
<th style="text-align: left;">Button / MenuItem</th>
<th style="text-align: left;"><blockquote>
<p>ClearLane</p>
</blockquote></th>
<th>Clears the lane specified in the ‘CommandParameter’ attribute of all
its data. A 0 clears all lanes.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

## Element Numbering

To support displaying the same race data or action more than once, Race
Coordinator automatically looks for elements names with an ‘\_#’
appended to them. Starting with 1, it looks for elements of each name
until it can't find the element. For example, if you wanted to display
the Track Name twice you would create two labels. The first would be
named ‘TrackName_1’ and the second would be called ‘TrackName_2’. If you
called them ‘TrackName_1’ and ‘TrackName_3’, only the first would
update, as ‘TrackName_2’ would not be found and the system would never
even look for ‘TrackName_3’.

Any field that represents time such as lap time, best lap, etc. support
the ‘DataContext’ attribute. This attribute is a modified JSON object
which supports the following fields. For example, this is from
Practice.xaml.

\<Viewbox MaxWidth="88" MaxHeight="255" Grid.Row="0" Grid.Column="0"
HorizontalAlignment="Right" VerticalAlignment="Bottom"\>

> \<Label Foreground="{StaticResource RSLabelColor}"
> Background="Transparent" BorderBrush="Transparent" FontSize="40"
> HorizontalContentAlignment="Right" VerticalContentAlignment="Bottom"
> Name="BestLapSegmentTime_Lane1_1" DataContext="'decimals':4,
> 'index':2" /\>

\</Viewbox\>

\<Viewbox MaxWidth="88" MaxHeight="255" Grid.Row="1" Grid.Column="0"
HorizontalAlignment="Right" VerticalAlignment="Bottom"\>

> \<Label Foreground="{StaticResource RSLabelColor}"
> Background="Transparent" BorderBrush="Transparent" FontSize="40"
> HorizontalContentAlignment="Right" VerticalContentAlignment="Bottom"
> Name="BestLapSegmentTime_Lane1_2" DataContext="'decimals':4,
> 'index':1" /\>

\</Viewbox\>

\<Viewbox MaxWidth="88" MaxHeight="255" Grid.Row="2" Grid.Column="0"
HorizontalAlignment="Right" VerticalAlignment="Bottom"\>

> \<Label Foreground="{StaticResource RSLabelColor}"
> Background="Transparent" BorderBrush="Transparent" FontSize="40"
> HorizontalContentAlignment="Right" VerticalContentAlignment="Bottom"
> Name="BestLapSegmentTime_Lane1_3" DataContext="'decimals':4,
> 'index':0" /\>

\</Viewbox\>

- index: Where appropriate (for example lap time) specifies which lap to
  display. 0 will display the last lap, 1 will display the second last
  lap, 2 the third last lap, etc

- decimals: How many decimal points to display for precision purposes.

Here are some ‘Racer Data’ example names:

- ‘Avatar_Position2_1’: Displays the image of the driver in second place
  for the heat

- ‘Avatar_Lane2_1’: Displays the image of the driver in lane two for the
  heat

- ‘Avatar_RaceLeader2_1’: Displays the image of the driver in second
  overall place

There are many XAML files provided with the RC install. They are located
in the directory \<install_dir\>\data\xaml .

## Let’s Build a Real Layout, Step by Step

### Step 1: Start with the base window

This is where everything sits. Think of it as your screen.

\<Window
xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"

xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"

Title="Race Day" Background="Transparent" Height="768" Width="1024"

WindowState="Maximized" FontFamily="Tahoma"
WindowStyle="ThreeDBorderWindow"

WindowStartupLocation="CenterScreen"\>

This tells Race Coordinator how big the screen is, what font to use, and
where to put it.

### Step 2: Add a Viewbox to scale everything

Viewbox makes sure your layout fills the screen at any resolution.

\<Viewbox Stretch="Fill"\>

\<!-- content goes here --\>

\</Viewbox\>

### Step 3: Add a Grid for rows and columns

The grid divides your screen into tidy boxes. You’ll use these to line
things up:

\<Grid\>

\<Grid.ColumnDefinitions\>

\<ColumnDefinition Width="150"/\>

\<ColumnDefinition Width="300"/\>

\<ColumnDefinition Width="150"/\>

\</Grid.ColumnDefinitions\>

\</Grid\>

Now your screen has 3 vertical sections.

### Step 4: Add a Label to show the driver's name

\<Label Name="Name_Lane1"

Content="Driver 1"

FontSize="24"

FontWeight="Bold"

Grid.Column="0"

HorizontalContentAlignment="Center"/\>

This puts the driver’s name in the first column. Race Coordinator will
replace Driver 1 with the real name.

### Step 5: Add an Image for the driver’s avatar

\<Image Name="Avatar_Lane1"

Source="\images\P_1.jpg"

Width="64" Height="64"

Grid.Column="1" /\>

The avatar image goes into the middle column.

### Step 6: Add a Lap Count

\<Label Name="Lap_Lane1"

Content="12"

FontSize="28"

Grid.Column="2"

HorizontalContentAlignment="Center" /\>

This shows how many laps that driver has completed. The number 12 is
just a placeholder as Race Coordinator will show the live lap count.

## Putting It All Together

<span class="mark">\<Window
xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"</span>

<span class="mark">xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"</span>

<span class="mark">Title="Race Day" Background="Transparent"
Height="768" Width="1024"</span>

<span class="mark">WindowState="Maximized" FontFamily="Tahoma"
WindowStyle="ThreeDBorderWindow"</span>

<span class="mark">WindowStartupLocation="CenterScreen"\></span>

<span class="mark">\<Viewbox Stretch="Fill"\></span>

<span class="mark">\<Grid\></span>

<span class="mark">\<Grid.ColumnDefinitions\></span>

<span class="mark">\<ColumnDefinition Width="150"/\></span>

<span class="mark">\<ColumnDefinition Width="300"/\></span>

<span class="mark">\<ColumnDefinition Width="150"/\></span>

<span class="mark">\</Grid.ColumnDefinitions\></span>

> <span class="mark">\<Label Name="Name_Lane1" Content="Driver 1"
> FontSize="24" FontWeight="Bold" Grid.Column="0"
> HorizontalContentAlignment="Center" /\></span>
>
> <span class="mark">\<Image Name="Avatar_Lane1"
> Source="\images\P_1.jpg" Width="64" Height="64" Grid.Column="1"
> /\></span>
>
> <span class="mark">\<Label Name="Lap_Lane1" Content="12" FontSize="28"
> Grid.Column="2" HorizontalContentAlignment="Center" /\></span>

<span class="mark">\</Grid\></span>

<span class="mark">\</Viewbox\></span>

<span class="mark">\</Window\></span>

### Common Gotchas to Avoid

- Don’t forget the \</Window\> tag at the end.

- Every Name="..." must match a real data field from Race Coordinator
  (see Appendix)

- Images must be in your images folder and named correctly.

- If something doesn’t show up, check spelling and tag placement.

- Racer Data and Generic Data fieldnames end in “\_\<integer\>”. Eg
  Start_1, CarImage_Lane7_1. Actions Data may have either with or
  without “\_\<integer\>”.

- If anywhere in the display of your custom XAML screens you see text
  that isn't what you put into the XAML file, and that text is prefixed
  with "RD\_" it means RC is trying to look up the localized text for
  the file. Here's how to fix it:

  1.  Create a file in the RC install directory  
      \<drive\>:\Program Files (x86)\Race Coordinator\data\Languages  
      named "custom.json".

  2.  Add the RD\_ key/value pairs just like they are in any of the
      other files there like "en_analog.json" (example below).

  3.  Relaunch RC.

> Note that the install directory can be located by using the Race Day
> Setup screens File menu option. Here's what your custom.json file
> might look like:
>
> {
>
> "RD_Key1": "Key1",
>
> "RD_Some Other Text": "Some other value",
>
> "RD_Last custom text": "Last custom value"
>
> }
>
> The keys must start with "RD\_" and must have the exact static text in
> your XAMLfile. This includes any punctuation, capitalization, and
> whitespace.

##  **Theme Dictionary**

Within the XAMLfolder (\<drive\>:\Program Files (x86)\Race
Coordinator\data\xaml), there is a file called ThemeDictionary.xaml,
which defines a central set of named resources — brushes, gradients,
colors, and styles — that control the look and feel of race-related
interfaces. These resources are referenced throughout your XAML via
{**StaticResource ResourceName**} and allow RC to apply standardized
visuals dynamically at runtime.

### Why It's Important in RC Layouts

- **Centralized Styling**: Instead of hardcoding colours on each
  control, layout designers use shared keys like **RSValueColor** or
  **RSTableCellBackground**. RC resolves these during layout load,
  ensuring consistent theming across all views.

- **Dynamic Skinning**: RC can swap or override these resources based on
  race mode, display type, or user settings — without modifying the
  layout structure.

- **Clarity and Contrast**: Keys like **RSLabelColorAlt**,
  **RSPenaltyColor**, and **RSBorderBrush** differentiate state
  indicators (e.g., penalties, lap count, performance metrics) with
  purposeful colour cues.

### Using Theme Dictionary

In the XAML file, add the following lines after the initial screen code:

\<Window.Resources\>

\<ResourceDictionary\>

\<ResourceDictionary.MergedDictionaries\>

\<ResourceDictionary Source="ThemeDictionary.xaml" /\>

\</ResourceDictionary.MergedDictionaries\>

\</ResourceDictionary\>

\</Window.Resources\>

For example:

## <img src=".\/media/image91.png"
style="width:7.37145in;height:1.29945in" /> Race Coordinator XAML Layout Explanation – Line by Line

<img src=".\/media/image128.png"
style="width:7.4858in;height:3.9365in" /><img src=".\/media/image117.png"
style="width:2.16875in;height:1.00903in" />

- Line 1: **\<Window ...\>** — This is the root element. It defines the
  entire window Race Coordinator will display.

- Lines 2-3: **xmlns** and **xmlns:x**: — Required namespaces for XAML
  to work – just accept this as it is.

- Line 4: **Title="Next Heat"** — The window’s title (may appear in the
  title bar).

**Width="275" Height="185"** — Sets the window size in pixels.

**ResizeMode="CanResize"** — Allows the user to resize the window.

**Background="Black"** — Sets the background color to black.

**SizeToContent="Manual"** — Prevents the window from resizing based on
its contents.

**WindowStartupLocation="CenterScreen"** — Opens the window in the
center of the  
screen.

- Line 5: **\<Viewbox Stretch="Fill"\>** — A Viewbox scales everything
  inside it to fit the window. Stretch="Fill" means it will stretch to
  fill the space.

- Line 6: **\<Grid\>** — A Grid is used to organize content in rows and
  columns.

- Line 7: **\<Grid.Background\>** — This sets a gradient background for
  the grid.

- Line 8: **LinearGradientBrush** — Creates a vertical gradient from top
  to bottom.

- Line 9: **GradientStop at Offset 0** — Dark gray (#181616) at the top.

- Line 10: **GradientStop at Offset 1** — Black (#000000) at the bottom.

- Line 11: **GradientStop at Offset 0.5** — Teal-blue (#2DADD6) in the
  middle.

- Line 12: **\</LinearGradientBrush\>** — This denotes that the
  LinearGradientBrush from line 8 is finished.

- Line 13: **\</Grid.Background\>** — This denotes that the definition
  of gradient background started in line 7 is finished.

- Line 15: **\<Grid.ColumnDefinitions\>** — This creates column
  definitions for the grid.

- Line 16: **\< ColumnDefinition Width=”250 /\>** — Defines one column
  that is 250 pixels wide and then closes the column definition on the
  same line.

- Line 17: **\</Grid.ColumnDefinitions\>** — This closes the column
  definitions for the grid.

- Line 19: **\<StackPanel Grid.RowSpan="2" Grid.Row="0" Margin="3"\>** —
  A StackPanel stacks items vertically. It spans two rows (even if not
  explicitly defined) and has a small margin around it.

- Line 20: **\<DockPanel ...\>** — Used to place the “Heat” label and
  the number of the heat field name (NextHeatNumber_1).

- Line 21: First **TextBlock** — Displays the word "Heat", font size 20,
  font colour white and font is in bold.

- Line 22: Second **TextBlock** — Displays the heat number, filled in by
  Race Coordinator using the field "NextHeatNumber_1". This is the first
  instance of NextHeatNumber.

- Line 25-26: **\<TextBlock FontSize="20" Name="NextHeatNickname1_1"
  Margin="5,0,10,0" Background="Black" Foreground="Black" /\>  
    
  \<TextBlock FontSize="20" Name="NextHeatNickname2_1" Margin="5,0,10,0"
  Background="Black" Foreground="Black" /\>**

> Each TextBlock displays a driver’s nickname for the upcoming heat.

- **FontSize="20"** — Makes the text readable.

- **Margin="5,0,10,0"** — Adds spacing around the text.

- **Background="Black"** and **Foreground="Black"** — In Race
  Coordinator, it’s common to see layout elements defined like this.
  This does *not* mean the control will display black text on a black
  background during runtime as Race Coordinator automatically injects
  runtime styling, including updated Background and Foreground colours,
  for Racer Data layout fields when the XAML is loaded. The colours on
  the loaded screen are defined in Race Coordinator on the Track Manager
  page:

> <img src=".\/media/image100.png"
> style="width:6.40188in;height:4.26792in" />

##  Field Names and Data Types

These are the field names that have been used in the Race Coordinator
XAML examples contained in the folder:

\<drive\>:\Program Files (x86)\Race Coordinator\data\xaml

**RACERDATA**

AddLapSections_Lane1

AddLapSections_Lane2

AddLapSections_Lane3

AddLapSections_Lane4

AddLapSections_Lane5

AddLapSections_Lane6

AddLapSections_Lane7

AddLapSections_Lane8

AdjustDeslot_Lane1

AdjustDeslot_Lane2

AdjustDeslot_Lane3

AdjustDeslot_Lane4

AdjustDeslot_Lane5

AdjustDeslot_Lane6

AdjustDeslot_Lane7

AdjustDeslot_Lane8

AverageTime_Lane1

AverageTime_Lane2

AverageTime_Lane3

AverageTime_Lane4

AverageTime_Lane5

AverageTime_Lane6

AverageTime_Lane7

AverageTime_Lane8

Avatar_Lane1

Avatar_Lane2

Avatar_Lane3

Avatar_Lane4

Avatar_Lane5

Avatar_Lane6

Avatar_Lane7

Avatar_Lane8

BestLaneNickname_Lane1

BestLaneNickname_Lane2

BestLaneNickname_Lane3

BestLaneNickname_Lane4

BestLaneNickname_Lane5

BestLaneNickname_Lane6

BestLaneNickname_Lane7

BestLaneNickname_Lane8

BestLaneName_Lane1

BestLaneName_Lane2

BestLaneName_Lane3

BestLaneName_Lane4

BestLaneName_Lane5

BestLaneName_Lane6

BestLaneName_Lane7

BestLaneName_Lane8

BestLaneTime_Lane1

BestLaneTime_Lane2

BestLaneTime_Lane3

BestLaneTime_Lane4

BestLaneTime_Lane5

BestLaneTime_Lane6

BestLaneTime_Lane7

BestLaneTime_Lane8

BestLapSegmentTime_Lane1

BestLapSegmentTime_Lane2

BestLapSegmentTime_Lane3

BestLapSegmentTime_Lane4

BestLapSegmentTime_Lane5

BestLapSegmentTime_Lane6

BestLapSegmentTime_Lane7

BestLapSegmentTime_Lane8

BestLapTime_Lane1

BestLapTime_Lane2

BestLapTime_Lane3

BestLapTime_Lane4

BestLapTime_Lane5

BestLapTime_Lane6

BestLapTime_Lane7

BestLapTime_Lane8

CarImage_Lane1

CarImage_Lane2

CarImage_Lane3

CarImage_Lane4

CarImage_Lane5

CarImage_Lane6

CarImage_Lane7

CarImage_Lane8

ChangeCar_Lane1

ChangeCar_Lane2

ChangeCar_Lane3

ChangeCar_Lane4

ChangeCar_Lane5

ChangeCar_Lane6

ChangeCar_Lane7

ChangeCar_Lane8

ChangeDriver_Lane1

ChangeDriver_Lane2

ChangeDriver_Lane3

ChangeDriver_Lane4

ChangeDriver_Lane5

ChangeDriver_Lane6

ChangeDriver_Lane7

ChangeDriver_Lane8

DeslotCount_Lane1

DeslotCount_Lane2

DeslotCount_Lane3

DeslotCount_Lane4

DeslotCount_Lane5

DeslotCount_Lane6

DeslotCount_Lane7

DeslotCount_Lane8

DriftLap_Lane1

DriftLap_Lane2

DriftLap_Lane3

DriftLap_Lane4

DriftLap_Lane5

DriftLap_Lane6

DriftLap_Lane7

DriftLap_Lane8

FuelCapacity_Lane1

FuelCapacity_Lane2

FuelCapacity_Lane3

FuelCapacity_Lane4

FuelCapacity_Lane5

FuelCapacity_Lane6

FuelCapacity_Lane7

FuelCapacity_Lane8

FuelImage_Lane1

FuelImage_Lane2

FuelImage_Lane3

FuelImage_Lane4

FuelImage_Lane5

FuelImage_Lane6

FuelImage_Lane7

FuelImage_Lane8

FuelLevel_Lane1

FuelLevel_Lane2

FuelLevel_Lane3

FuelLevel_Lane4

FuelLevel_Lane5

FuelLevel_Lane6

FuelLevel_Lane7

FuelLevel_Lane8

GapLeader_Lane1

GapLeader_Lane2

GapLeader_Lane3

GapLeader_Lane4

GapLeader_Lane5

GapLeader_Lane6

GapLeader_Lane7

GapLeader_Lane8

Lap_Lane1

Lap_Lane2

Lap_Lane3

Lap_Lane4

Lap_Lane5

Lap_Lane6

Lap_Lane7

Lap_Lane8

LapTime_Lane1

LapTime_Lane2

LapTime_Lane3

LapTime_Lane4

LapTime_Lane5

LapTime_Lane6

LapTime_Lane7

LapTime_Lane8

MedianTime_Lane1

MedianTime_Lane2

MedianTime_Lane3

MedianTime_Lane4

MedianTime_Lane5

MedianTime_Lane6

MedianTime_Lane7

MedianTime_Lane8

Name_Lane1

Name_Lane2

Name_Lane3

Name_Lane4

Name_Lane5

Name_Lane6

Name_Lane7

Name_Lane8

Nickname_Lane1

Nickname_Lane2

Nickname_Lane3

Nickname_Lane4

Nickname_Lane5

Nickname_Lane6

Nickname_Lane7

Nickname_Lane8

ReactionTime_Lane1

ReactionTime_Lane2

ReactionTime_Lane3

ReactionTime_Lane4

ReactionTime_Lane5

ReactionTime_Lane6

ReactionTime_Lane7

ReactionTime_Lane8

RecordLaneName_Lane1

RecordLaneName_Lane2

RecordLaneName_Lane3

RecordLaneName_Lane4

RecordLaneName_Lane5

RecordLaneName_Lane6

RecordLaneName_Lane7

RecordLaneName_Lane8

RecordLaneNickname_Lane1

RecordLaneNickname_Lane2

RecordLaneNickname_Lane3

RecordLaneNickname_Lane4

RecordLaneNickname_Lane5

RecordLaneNickname_Lane6

RecordLaneNickname_Lane7

RecordLaneNickname_Lane8

RecordLaneTime_Lane1

RecordLaneTime_Lane2

RecordLaneTime_Lane3

RecordLaneTime_Lane4

RecordLaneTime_Lane5

RecordLaneTime_Lane6

RecordLaneTime_Lane7

RecordLaneTime_Lane8

SelfPerformance_Lane1

SelfPerformance_Lane2

SelfPerformance_Lane3

SelfPerformance_Lane4

SelfPerformance_Lane5

SelfPerformance_Lane6

SelfPerformance_Lane7

SelfPerformance_Lane8

SegmentTime_Lane1

SegmentTime_Lane2

SegmentTime_Lane3

SegmentTime_Lane4

SegmentTime_Lane5

SegmentTime_Lane6

SegmentTime_Lane7

SegmentTime_Lane8

AddLapSections_Position1

AddLapSections_Position2

AddLapSections_Position3

AddLapSections_Position4

AddLapSections_Position5

AddLapSections_Position6

AddLapSections_Position7

AddLapSections_Position8

AdjustDeslot_Position1

AdjustDeslot_Position2

AdjustDeslot_Position3

AdjustDeslot_Position4

AdjustDeslot_Position5

AdjustDeslot_Position6

AdjustDeslot_Position7

AdjustDeslot_Position8

Avatar_Position1

Avatar_Position2

Avatar_Position3

Avatar_Position4

Avatar_Position5

Avatar_Position6

Avatar_Position7

Avatar_Position8

AverageTime_Position1

AverageTime_Position2

AverageTime_Position3

AverageTime_Position4

BestLaneName_Position1

BestLaneName_Position2

BestLaneName_Position3

BestLaneName_Position4

BestLaneTime_Position1

BestLaneTime_Position2

BestLaneTime_Position3

BestLaneTime_Position4

BestLapTime_Position1

BestLapTime_Position2

BestLapTime_Position3

BestLapTime_Position4

BestLapTime_Position5

BestLapTime_Position6

BestLapTime_Position7

BestLapTime_Position8

CarImage_Position1

CarImage_Position2

CarImage_Position3

CarImage_Position4

CarImage_Position5

CarImage_Position6

CarImage_Position7

CarImage_Position8

ChangeCar_Position1

ChangeCar_Position2

ChangeCar_Position3

ChangeCar_Position4

ChangeCar_Position5

ChangeCar_Position6

ChangeCar_Position7

ChangeCar_Position8

ChangeDriver_Position1

ChangeDriver_Position2

ChangeDriver_Position3

ChangeDriver_Position4

ChangeDriver_Position5

ChangeDriver_Position6

ChangeDriver_Position7

ChangeDriver_Position8

DeslotCount_Position1

DeslotCount_Position2

DeslotCount_Position3

DeslotCount_Position4

DeslotCount_Position5

DeslotCount_Position6

DeslotCount_Position7

DeslotCount_Position8

DriftLap_Position1

DriftLap_Position2

DriftLap_Position3

DriftLap_Position4

DriftLap_Position5

DriftLap_Position6

DriftLap_Position7

DriftLap_Position8

FuelCapacity_Position1

FuelCapacity_Position2

FuelCapacity_Position3

FuelCapacity_Position4

FuelCapacity_Position5

FuelCapacity_Position6

FuelCapacity_Position7

FuelCapacity_Position8

FuelImage_Position1

FuelImage_Position2

FuelImage_Position3

FuelImage_Position4

FuelImage_Position5

FuelImage_Position6

FuelImage_Position7

FuelImage_Position8

FuelLevelPCT_Position1

FuelLevelPCT_Position2

FuelLevelPCT_Position3

FuelLevelPCT_Position4

FuelLevel_Position1

FuelLevel_Position2

FuelLevel_Position3

FuelLevel_Position4

FuelLevel_Position5

FuelLevel_Position6

FuelLevel_Position7

FuelLevel_Position8

GapLeader_Position1

GapLeader_Position2

GapLeader_Position3

GapLeader_Position4

HeatPerformance_Position1

HeatPerformance_Position2

HeatPerformance_Position3

HeatPerformance_Position4

LapTime_Position1

LapTime_Position2

LapTime_Position3

LapTime_Position4

LapTime_Position5

LapTime_Position6

LapTime_Position7

LapTime_Position8

Lap_Position1

Lap_Position2

Lap_Position3

Lap_Position4

Lap_Position5

Lap_Position6

Lap_Position7

Lap_Position8

Led_Position1

Led_Position2

Led_Position3

Led_Position4

MPH_Position1

MPH_Position2

MPH_Position3

MPH_Position4

MedianTime_Position1

MedianTime_Position2

MedianTime_Position3

MedianTime_Position4

MedianTime_Position5

MedianTime_Position6

MedianTime_Position7

MedianTime_Position8

Nickname_Position1

Nickname_Position2

Nickname_Position3

Nickname_Position4

Nickname_Position5

Nickname_Position6

Nickname_Position7

Nickname_Position8

ReactionTime_Position1

ReactionTime_Position2

ReactionTime_Position3

ReactionTime_Position4

RecordLaneName_Position1

RecordLaneName_Position2

RecordLaneName_Position3

RecordLaneName_Position4

RecordLaneTime_Position1

RecordLaneTime_Position2

RecordLaneTime_Position3

RecordLaneTime_Position4

Seed_Position1

Seed_Position2

Seed_Position3

Seed_Position4

SegmentTime_Position1

SegmentTime_Position2

SegmentTime_Position3

SegmentTime_Position4

SegmentTime_Position5

SegmentTime_Position6

SegmentTime_Position7

SegmentTime_Position8

SelfPerformance_Position1

SelfPerformance_Position2

SelfPerformance_Position3

SelfPerformance_Position4

TrackPerformance_Position1

TrackPerformance_Position2

TrackPerformance_Position3

TrackPerformance_Position4

Avatar_RaceLeader1

Avatar_RaceLeader2

Avatar_RaceLeader3

Avatar_RaceLeader4

Avatar_RaceLeader5

Avatar_RaceLeader6

Avatar_RaceLeader7

Avatar_RaceLeader8

Avatar_RaceLeader9

Avatar_RaceLeader10

Avatar_RaceLeader11

Avatar_RaceLeader12

Avatar_RaceLeader13

Avatar_RaceLeader14

Avatar_RaceLeader15

Avatar_RaceLeader16

Avatar_RaceLeader17

Avatar_RaceLeader18

Avatar_RaceLeader19

Avatar_RaceLeader20

AverageTime_RaceLeader1

AverageTime_RaceLeader10

AverageTime_RaceLeader11

AverageTime_RaceLeader12

AverageTime_RaceLeader13

AverageTime_RaceLeader14

AverageTime_RaceLeader15

AverageTime_RaceLeader16

AverageTime_RaceLeader17

AverageTime_RaceLeader18

AverageTime_RaceLeader19

AverageTime_RaceLeader2

AverageTime_RaceLeader20

AverageTime_RaceLeader3

AverageTime_RaceLeader4

AverageTime_RaceLeader5

AverageTime_RaceLeader6

AverageTime_RaceLeader7

AverageTime_RaceLeader8

AverageTime_RaceLeader9

BestLapTime_RaceLeader1

BestLapTime_RaceLeader10

BestLapTime_RaceLeader11

BestLapTime_RaceLeader12

BestLapTime_RaceLeader13

BestLapTime_RaceLeader14

BestLapTime_RaceLeader15

BestLapTime_RaceLeader16

BestLapTime_RaceLeader17

BestLapTime_RaceLeader18

BestLapTime_RaceLeader19

BestLapTime_RaceLeader2

BestLapTime_RaceLeader20

BestLapTime_RaceLeader3

BestLapTime_RaceLeader4

BestLapTime_RaceLeader5

BestLapTime_RaceLeader6

BestLapTime_RaceLeader7

BestLapTime_RaceLeader8

BestLapTime_RaceLeader9

GapLeader_RaceLeader1

GapLeader_RaceLeader10

GapLeader_RaceLeader11

GapLeader_RaceLeader12

GapLeader_RaceLeader13

GapLeader_RaceLeader14

GapLeader_RaceLeader15

GapLeader_RaceLeader16

GapLeader_RaceLeader17

GapLeader_RaceLeader18

GapLeader_RaceLeader19

GapLeader_RaceLeader2

GapLeader_RaceLeader20

GapLeader_RaceLeader3

GapLeader_RaceLeader4

GapLeader_RaceLeader5

GapLeader_RaceLeader6

GapLeader_RaceLeader7

GapLeader_RaceLeader8

GapLeader_RaceLeader9

GapPosition_RaceLeader1

GapPosition_RaceLeader10

GapPosition_RaceLeader11

GapPosition_RaceLeader12

GapPosition_RaceLeader13

GapPosition_RaceLeader14

GapPosition_RaceLeader15

GapPosition_RaceLeader16

GapPosition_RaceLeader17

GapPosition_RaceLeader18

GapPosition_RaceLeader19

GapPosition_RaceLeader2

GapPosition_RaceLeader20

GapPosition_RaceLeader3

GapPosition_RaceLeader4

GapPosition_RaceLeader5

GapPosition_RaceLeader6

GapPosition_RaceLeader7

GapPosition_RaceLeader8

GapPosition_RaceLeader9

Lap_RaceLeader1

Lap_RaceLeader10

Lap_RaceLeader11

Lap_RaceLeader12

Lap_RaceLeader13

Lap_RaceLeader14

Lap_RaceLeader15

Lap_RaceLeader16

Lap_RaceLeader17

Lap_RaceLeader18

Lap_RaceLeader19

Lap_RaceLeader2

Lap_RaceLeader20

Lap_RaceLeader3

Lap_RaceLeader4

Lap_RaceLeader5

Lap_RaceLeader6

Lap_RaceLeader7

Lap_RaceLeader8

Lap_RaceLeader9

Nickname_RaceLeader1

Nickname_RaceLeader10

Nickname_RaceLeader11

Nickname_RaceLeader12

Nickname_RaceLeader13

Nickname_RaceLeader14

Nickname_RaceLeader15

Nickname_RaceLeader16

Nickname_RaceLeader17

Nickname_RaceLeader18

Nickname_RaceLeader19

Nickname_RaceLeader2

Nickname_RaceLeader20

Nickname_RaceLeader3

Nickname_RaceLeader4

Nickname_RaceLeader5

Nickname_RaceLeader6

Nickname_RaceLeader7

Nickname_RaceLeader8

Nickname_RaceLeader9

Seed_RaceLeader1

Seed_RaceLeader10

Seed_RaceLeader11

Seed_RaceLeader12

Seed_RaceLeader13

Seed_RaceLeader14

Seed_RaceLeader15

Seed_RaceLeader16

Seed_RaceLeader17

Seed_RaceLeader18

Seed_RaceLeader19

Seed_RaceLeader2

Seed_RaceLeader20

Seed_RaceLeader3

Seed_RaceLeader4

Seed_RaceLeader5

Seed_RaceLeader6

Seed_RaceLeader7

Seed_RaceLeader8

Seed_RaceLeader9

Standing_RaceLeader1

Standing_RaceLeader10

Standing_RaceLeader11

Standing_RaceLeader12

Standing_RaceLeader13

Standing_RaceLeader14

Standing_RaceLeader15

Standing_RaceLeader16

Standing_RaceLeader17

Standing_RaceLeader18

Standing_RaceLeader19

Standing_RaceLeader2

Standing_RaceLeader20

Standing_RaceLeader3

Standing_RaceLeader4

Standing_RaceLeader5

Standing_RaceLeader6

Standing_RaceLeader7

Standing_RaceLeader8

Standing_RaceLeader9

Nickname_SeasonLeader1

Nickname_SeasonLeader10

Nickname_SeasonLeader11

Nickname_SeasonLeader12

Nickname_SeasonLeader13

Nickname_SeasonLeader14

Nickname_SeasonLeader15

Nickname_SeasonLeader16

Nickname_SeasonLeader17

Nickname_SeasonLeader18

Nickname_SeasonLeader19

Nickname_SeasonLeader2

Nickname_SeasonLeader20

Nickname_SeasonLeader3

Nickname_SeasonLeader4

Nickname_SeasonLeader5

Nickname_SeasonLeader6

Nickname_SeasonLeader7

Nickname_SeasonLeader8

Nickname_SeasonLeader9

Standing_SeasonLeader1

Standing_SeasonLeader10

Standing_SeasonLeader11

Standing_SeasonLeader12

Standing_SeasonLeader13

Standing_SeasonLeader14

Standing_SeasonLeader15

Standing_SeasonLeader16

Standing_SeasonLeader17

Standing_SeasonLeader18

Standing_SeasonLeader19

Standing_SeasonLeader2

Standing_SeasonLeader20

Standing_SeasonLeader3

Standing_SeasonLeader4

Standing_SeasonLeader5

Standing_SeasonLeader6

Standing_SeasonLeader7

Standing_SeasonLeader8

Standing_SeasonLeader9

Nickname_SeasonRaceLeader1

Nickname_SeasonRaceLeader10

Nickname_SeasonRaceLeader11

Nickname_SeasonRaceLeader12

Nickname_SeasonRaceLeader13

Nickname_SeasonRaceLeader14

Nickname_SeasonRaceLeader15

Nickname_SeasonRaceLeader16

Nickname_SeasonRaceLeader17

Nickname_SeasonRaceLeader18

Nickname_SeasonRaceLeader19

Nickname_SeasonRaceLeader2

Nickname_SeasonRaceLeader20

Nickname_SeasonRaceLeader3

Nickname_SeasonRaceLeader4

Nickname_SeasonRaceLeader5

Nickname_SeasonRaceLeader6

Nickname_SeasonRaceLeader7

Nickname_SeasonRaceLeader8

Nickname_SeasonRaceLeader9

Standing_SeasonRaceLeader1

Standing_SeasonRaceLeader10

Standing_SeasonRaceLeader11

Standing_SeasonRaceLeader12

Standing_SeasonRaceLeader13

Standing_SeasonRaceLeader14

Standing_SeasonRaceLeader15

Standing_SeasonRaceLeader16

Standing_SeasonRaceLeader17

Standing_SeasonRaceLeader18

Standing_SeasonRaceLeader19

Standing_SeasonRaceLeader2

Standing_SeasonRaceLeader20

Standing_SeasonRaceLeader3

Standing_SeasonRaceLeader4

Standing_SeasonRaceLeader5

Standing_SeasonRaceLeader6

Standing_SeasonRaceLeader7

Standing_SeasonRaceLeader8

Standing_SeasonRaceLeader9

NextHeatNickname1

NextHeatNickname2

NextHeatNickname3

NextHeatNickname4

NextHeatNickname5

NextHeatNickname6

NextHeatNickname7

NextHeatNickname8

OnDeckNickname1

OnDeckNickname2

OnDeckNickname3

OnDeckNickname4

OnDeckNickname5

OnDeckNickname6

OnDeckNickname7

OnDeckNickname8

SegmentTimeLabel1

SegmentTimeLabel2

SegmentTimeLabel3

SegmentTimeLabel4

SegmentTimeLabel5

SegmentTimeLabel6

SegmentTimeLabel7

SegmentTimeLabel8

Pos1

Pos2

Pos3

Pos4

Pos5

Pos6

Pos7

Pos8

Pos9

Pos10

Pos11

Pos12

Pos13

Pos14

Pos15

Pos16

Pos17

Pos18

Pos19

Pos20

<table style="width:65%;">
<colgroup>
<col style="width: 35%" />
<col style="width: 29%" />
</colgroup>
<thead>
<tr>
<th style="text-align: left;"><strong>GENERIC DATA</strong></th>
<th style="text-align: left;"><strong>ACTIONS</strong></th>
</tr>
<tr>
<th><p>BestHeatName</p>
<p>BestHeatNickname</p>
<p>BestHeatTime</p>
<p>BestName</p>
<p>BestNickname</p>
<p>BestTime</p>
<p>HeatNumber</p>
<p>NumHeats</p>
<p>RaceName</p>
<p>RaceStateImage</p>
<p>RaceTime</p>
<p>RecordName</p>
<p>RecordNickname</p>
<p>RecordScore</p>
<p>RecordScoreName</p>
<p>RecordScoreNickname</p>
<p>RecordTime</p>
<p>SeasonRaces</p>
<p>StartLamp1</p>
<p>StartLamp2</p>
<p>StartLamp3</p>
<p>StartLamp4</p>
<p>StartLamp5</p>
<p>StartLamp6</p>
<p>StartLamp7</p>
<p>StartLamp8</p>
<p>StartLamp9</p>
<p>StartLamp10</p>
<p>StatusLabel</p>
<p>TrackImage</p>
<p>TrackName</p>
<p>NextHeatNumber</p></th>
<th><p>AddLaps</p>
<p>ClearLane</p>
<p>DebugodeToggle</p>
<p>DeferHeat</p>
<p>DriverLB</p>
<p>Editor</p>
<p>Export</p>
<p>LapEditor</p>
<p>LapLB</p>
<p>ModifyHeats</p>
<p>NextHeat</p>
<p>Pause</p>
<p>PowerOff</p>
<p>PowerOn</p>
<p>PreviewHost</p>
<p>RestartHeat</p>
<p>Save</p>
<p>SaveAs</p>
<p>SkipHeat</p>
<p>SkipRace</p>
<p>Start</p>
<p>Toggle</p>
<p>VideoTest</p>
<p>ViewHeats</p>
<p>Window</p>
<p>dockPanel1</p>
<p>dockPanel2</p>
<p>grid1</p>
<p>menu1</p>
<p>stackPanel1</p></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

##  

## XAML Editing Software

A quick internet search will result in an overwhelming number of code /
text editors, development environments, and other coding tools. Prices
range from free to expensive. It is beyond the scope of this document to
suggest what would work best for a specific user.

However, a member of the RC user community has provided a free & open
source coding & preview tool that is specific to working with Race
Coordinator. It called RC Layout Preview, and can be found via this link
on the GitHub online code repository web site:  
[<u>ConnalM/RaceCoordinatorCommunity: XAML
Preview</u>](https://github.com/ConnalM/RaceCoordinatorCommunity)

A big advantage of this tool is that it shows a fairly close
approximation of what your custom screens will look like without having
to be running Race Coordinator.

# <img src=".\/media/image116.jpg"
style="width:7.11458in;height:6.30208in" />  

# RCLive

## Setup 

### 1. Prerequisites

- **Operating System**: Windows XP or higher, fully updated.

- **.NET Framework**: Version 4 installed (RC installer checks this).

- **Race Coordinator Installed**: Latest version from
  [<u>racecoordinator.net</u>](https://www.racecoordinator.net/).

- **Track Hardware**: Arduino, Trakmate, parallel port, game port, or
  webcam interface connected and configured.

### 2. Enable the Webserver

RCLive runs through RC’s built‑in webserver.

- Open **Race Coordinator**.

- Go to **Manage → Track** or **Options** (depending on version).

- Enable the **Webserver** option.

- Choose a **port number** (default is often 8080 or 1234).

- Confirm the **root directory** for served files (where your
  HTML/CSS/JS overlays will live).

- Restart Race Coordinator in Administrator mode, if not already done.

Example:  
If the port is 8080, then http://localhost:8080 will serve your
index.html file.  
API queries are available at http://localhost:8080/api.

### 3. Test the Webserver

- Open a browser on the same PC.

- Navigate to http://localhost:8080.

- You should see either the default index.html or your custom overlay
  page.

- Test an API call:

<!-- -->

- http://localhost:8080/api?q=trackData → returns track info.

- http://localhost:8080/api?q=raceData → returns race info.

- http://localhost:8080/api?q=heatData → returns heat status.

- http://localhost:8080/api?q=heatDriverData → returns driver standings.

### 4. Build Your RCLive Overlay

- Create a simple **HTML/JavaScript page** that polls the API endpoints.

- Display key race data such as:

  - Track name and lane colors

  - Current heat number and time/laps remaining

  - Driver names, nicknames, lap counts, best laps, gaps to leader

- Place this page in the webserver’s root directory.

- Open it in a browser window or on a projector for spectators.

### 5. Broadcasting Online

If you want remote viewers:

- Share your PC’s IP address + port (e.g., http://192.168.1.50:8080) for
  LAN spectators.

- For internet broadcasting, capture the RCLive browser window in
  **OBS** or similar streaming software.

- Stream to YouTube, Twitch, or your club’s site.

### 6. Race Day Workflow

1.  Start Race Coordinator.

2.  Load drivers, cars, and race profile.

3.  Ensure the webserver is running.

4.  Open your RCLive overlay in a browser or projector.

5.  Spectators follow along live via the overlay or stream.

### 7. Tips & Best Practices

- **Simulation Mode**: Test RCLive without hardware by running demo
  races.

- **Customization**: Add driver avatars, car images, or lane colors for
  a polished look.

- **Performance**: Keep overlays lightweight (HTML/JS) to avoid lag.

- **Security**: If broadcasting online, restrict access or use a VPN.

## 

##  

## Query Protocol (RCLive)

Purpose

The **Query Protocol** is the backbone of RCLive. It allows external
applications (like web pages or overlays) to request live race data from
Race Coordinator’s built-in webserver. Instead of being limited to the
local race screen (XAML bindings), the Query Protocol exposes detailed,
structured JSON data about the track, race, heats, drivers, and laps.

This makes it possible to build **custom dashboards, streaming overlays,
or spectator displays** that show exactly the information you want, in
real time.

Why It’s Better Than XAML

- **XAML**: Only updates the local race screen inside Race Coordinator.
  It’s limited to predefined bindings (lap count, race time, etc.).

- **Query Protocol**: Exposes *all* race data externally in JSON format.
  You can request specific fields, combine multiple queries, and build
  your own presentation layer.

- **Flexibility**: You can design overlays that show reaction times,
  fuel levels, lap‑by‑lap breakdowns, or custom leaderboards — things
  that XAML cannot easily provide.

In short: **XAML is for local display, Query Protocol is for external
broadcast and integration.**

How Queries Work

- Queries are sent to the RC webserver at /api.

- Each query specifies what data you want (trackData, raceData,
  heatData, heatDriverData, etc.).

- Responses are returned as JSON objects.

- You can include a transaction ID (tid) to match requests and
  responses.

- Multiple queries can be bundled into one request.

Example Query

Request (typed into a browser or used in code):

http://localhost:8080/api?tid=m0&q=trackData

Response (JSON):

<img src=".\/media/image1.png"
style="width:4.08188in;height:3.53646in" />

Example in HTML

It’s outside the scope here to explain full HTML/JavaScript coding, but
the general idea is:

\<script\>

fetch("http://localhost:8080/api?tid=m0&q=trackData")

.then(response =\> response.json())

.then(data =\> {

// Access fields

const trackName = data.r\[0\].trackData.n;

const lanes = data.r\[0\].trackData.l;

document.getElementById("trackName").innerText = trackName;

// Example: show lane colors and lengths

lanes.forEach(lane =\> {

console.log("Lane color:", lane.c, "Length:", lane.l);

});

});

\</script\>

\<div id="trackName"\>\</div\>

This snippet fetches the track name and lane data, then displays it in a
web page. You can find plenty of tutorials online about using fetch() in
JavaScript to handle JSON data.

### Information Provided by the Query Protocol

Data Sections

1\. **Track Data**

- **Purpose**: Returns information about the track being raced on.

- **Fields Provided**:

  - n → Track name

  - l → Array of lane objects, each with:

  - c → Lane color

  - l → Lane length (in feet)

- **Use Case**: Display lane colors and lengths in overlays, or show
  track name in a broadcast.

2\. **Race Data**

- **Purpose**: Provides details about the race configuration and
  participants.

- **Fields Provided**:

  - n → Race name

  - rlt → Record lap time (driver + value + date)

  - rs → Record score (driver + value + date)

  - blt → Best lap time for this specific race instance

  - d → Array of race driver objects:

  - n → Driver name

  - nn → Nickname

  - s → Seed (starting order/position)

  - did → Unique driver ID

  - h → Array of heats the driver is assigned to

- **Use Case**: Show race name, current records, and list of drivers
  with nicknames and seeds.

3\. **Heat Data**

- **Purpose**: Returns information about the current heat.

- **Fields Provided**:

  - s → Heat state (integer code: not started, countdown, racing,
    paused, ended, etc.)

  - sname → Human-readable state (e.g., “Paused”, “Racing”)

  - cnt → Total number of heats in the race

  - hn → Current heat number (0-based)

  - t → Time value (depends on state: countdown seconds, elapsed time,
    or time remaining)

- **Use Case**: Show heat progress, countdown timers, or whether the
  race is paused.

4\. **Race Driver Data**

- **Purpose**: Aggregates data for each driver across all heats.

- **Fields Provided**:

  - n → Driver name

  - nn → Nickname

  - did → Unique driver ID

  - v → Overall race score (laps, points, or time depending on
    configuration)

  - led → Number of laps led

  - l → Total lap count

  - blt → Best lap time

- **Use Case**: Build a leaderboard showing total laps, scores, and best
  laps across the whole event.

5\. **Heat Driver Data**

- **Purpose**: Provides per-driver data for the current heat.

- **Fields Provided**:

  - n → Driver name

  - nn → Nickname

  - rt → Reaction time (start line response)

  - led → Laps led in this heat

  - l → Lap count in this heat

  - lt → Last lap time

  - blt → Best lap time in this heat

  - a → Average lap time

  - g → Gap to leader

  - gp → Gap to next position

  - p → Position in heat

  - f → Fuel level (if fuel simulation is enabled)

  - fm → Maximum fuel capacity

- **Use Case**: Show live heat standings, lap times, and gaps between
  drivers.

6\. **Heat Driver Lap Data**

- **Purpose**: Returns lap-by-lap data for a specific driver.

- **Fields Provided**:

  - abs → Absolute race time when the lap was completed

  - lt → Lap time for that lap

- **Use Case**: Detailed lap charts, performance analysis, or post-race
  statistics.

Further Information

The README file you uploaded contains **full details of every query,
parameter, and response field**. For deeper integration, refer to the
readme files in the root of Race Coordinator to see all available
options and data structures.

> 

# Appendices

## Appendix A - Definitions, Acronyms & Abbreviations

| **TERM** | **DESCRIPTION / DEFINITION** |
|----|----|
| **CSV** | Comma Separated Values. A plain text data format that separates each data value within a record with a comma and each record with a newline character. Each line in the file usually represents one data record. |
| **Event** | A series of races. The first race gets its drivers' seeds from the order in which they are added in the Race Day Setup screen. Each subsequent race gets its drivers and their seeds from the previous race's final standings. Any number of races can be added to an event, allowing for any combination of Practice, Qualifiers, Semifinal, and Finals races. Some or all drivers can be carried over from one race to the next, so the driver field can be reduced down slowly if desired. |
| **GUI** | Graphical User Interface. |
| **Heat** | A heat is a set of drivers racing around the track for either a set period of time or a set number of laps. Each heat is scored independently of all other heats. There are several RC settings that control how long a heat lasts and how it is scored. |
| **IR** | Infrared. A wavelength of light that cannot be seen by the human eye. |
| **LED** | Light Emitting Diode. A type of semiconductor device that emits light in various visible light wavelengths / colors as well as infrared light. |
| **NC** | Normally Closed. Usually in reference to track power relays. |
| **NO** | Normally Open. Usually in reference to track power relays. |
| **Race** | A collection of heats. Each driver's heat scores are combined to calculate the final race standings for that driver. There are many RC settings that control how the heat scores are combined. |
| **RC** | Race Coordinator. |
| **RMS** | Race Management System. Race Coordinator is an RMS. |
| **Round Robin** | A popular race format intended to remove the advantage of certain lanes of a track being quicker or easier to drive. To achieve this, each driver races once (or could be multiple times) on each lane of the track. The winner is decided on the cumulative totals of all of the heats |
| **Season** | A number of events (e.g., the number of grand prix in a year). |
| **USB** | Universal Serial Bus. |
| **.XLSX** | A file with the .xlsx file extension is a Microsoft Excel Open XML Spreadsheet (XLSX) file. You can also open this format in other spreadsheet applications, such as Apple Numbers, Google Docs, LibreOffice Calc and OpenOffice Calc. RC exports race results / statistics in XLSX format |

## Appendix B - Revision History

Summary of changes made in each revision of the manual. The draft
version 0.x descriptions will probably be removed in document version
1.0.

<table style="width:100%;">
<colgroup>
<col style="width: 12%" />
<col style="width: 13%" />
<col style="width: 73%" />
</colgroup>
<thead>
<tr>
<th style="text-align: center;"><strong>DOCUMENT VERSION</strong></th>
<th style="text-align: center;"><strong>RELEASE DATE</strong></th>
<th style="text-align: center;"><strong>DESCRIPTION /
COMMENTS</strong></th>
</tr>
<tr>
<th style="text-align: center;">0.8</th>
<th style="text-align: center;">xx/xx/xxxx</th>
<th></th>
</tr>
<tr>
<th style="text-align: center;">0.7</th>
<th style="text-align: center;">xx/xx/xxxx</th>
<th></th>
</tr>
<tr>
<th style="text-align: center;">0.6</th>
<th style="text-align: center;">10/13/2025</th>
<th><p>Added Chapter - Race Screen XAML Customization (Dave priority
#1).</p>
<p>Added Chapter - Event Setup.</p>
<p>Added Chapter - Season Setup.</p>
<p>Added Chapter - Race Day.</p>
<p>Added Detail - Track Setup chapter: Arduino sketch Extended Protocol
(Dave priority #3).</p>
<p>Added Detail - Race Setup chapter: all setup methods. Includes
detailed descriptions of race formats, scoring settings, and everything.
(Dave priority #2).</p>
<p>Added Detail - Race Day Setup chapter.</p>
<p>Added Appendix - XAML Keyboard Shortcuts.</p></th>
</tr>
<tr>
<th style="text-align: center;">0.5</th>
<th style="text-align: center;">07/15/2025</th>
<th><p>Added details to the <em>Track Setup</em> chapter’s <em>Track
Manager</em> section.</p>
<p>Added details to the <em>Track Setup</em> chapter’s <em>Track
Interface</em> &gt; <em>Web Cam</em> section. Used text from RC website
FAQ.<br />
Added details to the <em>Track Setup</em> chapter’s <em>Track
Interface</em> &gt; <em>DS Electronics DSxx</em> section. The kind folks
at Pendle Slot Racing gave us permission to reproduce their blog entry
<em>Using DS Lap Counter with Race Coordinator.</em></p>
<p>Added details to the <em>Car Setup</em> chapter.</p>
<p>Added details to the <em>Driver Setup</em> chapter’s <em>Driver
Guided Setup</em> section.</p>
<p>Updated fonts to latest versions: Source Sans Pro to Source Sans 3,
and Source Serif Pro to Source Serif 4.</p></th>
</tr>
<tr>
<th style="text-align: center;">0.4</th>
<th style="text-align: center;">09/13/2024</th>
<th><p>Added Appendix B - Revision History.</p>
<p>Added Appendix C - Backup / Restore RC Database. Text was copied from
the</p>
<p>Slot Forum discussion thread of the same name.</p>
<p>Added Quick Start chapter in an attempt to provide a short concise
procedure to get a new user up &amp; running, based on input provided by
SlotForum members Race Coordinator, beardy56 and Dopamine.</p>
<p>Added details to Track Interface section Arduino, based on input
provided by SlotForum members Race Coordinator and Lannoc.</p>
<p>Added details to Track Interface section Trackmate, based on input
provided by Trackmate; it turns out that all past and present serial
Trackmate versions are supported.</p>
<p>Renamed chapter Installation and Setup to Installation - to avoid
confusion with chapters such as Track Setup, Race Setup, etc..</p>
<p>Moved sections about specific track interfaces around so that serial
Trackmate and Arduino are listed first; according to Dave these are the
most popular with RC and will be the ones first supported if a Version
1.16 / 2.0 is created.</p>
<p>Added Source Code Pro to the typefaces used in the document. It is
another Open Source (free) product originally created by Adobe, and is
used in the document for “code” text such as software commands /
listings.</p></th>
</tr>
<tr>
<th style="text-align: center;">0.3</th>
<th style="text-align: center;">06/22/2024</th>
<th><p>Changed the typeface families to Source Sans Pro and Source Serif
Pro - both are Open Source (free) products originally created by Adobe.
Heading text color changed to RGB=19 72 129 and body text color to
RGB=34 30 31. Moved the Definitions, Acronyms &amp; Abbreviations from
the Introduction chapter to a new Appendix A - Definitions, Acronyms
&amp; Abbreviations. There will most likely be several additional
Appendices - just not sure yet which of the many possible topics to
include.</p>
<p>Updated the screen captures in the Track Setup chapter to those from
a new RC 1.15.2.0 installation.</p>
<p>Added detail about Track Interface configuration for the Serial
Trackmate (I have never used one, so if someone could provide some help
here that would be great), and the Web Cam (which doesn't have any
configuration done within RC). Heading "stubs" added for the other Track
Interfaces.</p>
<p>Changed the application program from Microsoft Word 2010 to Affinity
Publisher 2.</p></th>
</tr>
<tr>
<th style="text-align: center;">0.2</th>
<th style="text-align: center;">06/19/2024</th>
<th>Added Chapters and document text provided by SlotForum user @Lannoc.
Added RC screenshots with detailed descriptions of the Track Manager
General and Lanes windows.</th>
</tr>
<tr>
<th style="text-align: center;">0.1</th>
<th style="text-align: center;">06/18/2024</th>
<th>A first (really rough) stab at establishing a document template for
the Technical / User Manual. Formatting based on a template supplied
with Microsoft Word.</th>
</tr>
</thead>
<tbody>
</tbody>
</table>

## Appendix C - Backup / Restore RC Database

This section describes how to backup / restore RCʼs data. This includes
moving RC from one PC to another.

**NOTE:** The following is only in regards to the RC database and saved
data. It does not backup anything the RC installer does. That is done by
simply running the RC installer.

### Backing up the RC Database

RC can be backed up as often as you want. If you're going to make major
configuration changes and you are at all nervous, make a backup. Keep in
mind that the backup is only useful until you run your next race. Once
you run a new race, the backup you made will still work; however, it
won't have any of the race data run after the most recent backup was
made.

To make a backup:

1.  Launch RC

2.  From the menu bar, select File → Debug To Zip.

3.  Save the file somewhere safe. You're all backed up!

4.  Make note of the version of RC you're running when the backup was
    made. Consider adding the version number into the filename of the
    file created in step 2. You'll need to know the version when you
    restore the backup. You can get the RC version from the About menu
    on the main setup screen or the bottom right of the splash screen
    when RC starts up

**NOTE:** If you use custom sounds, XAML files or localization make sure
you copy those to your new PC in the same directories as they were
located in your old PC. You may have to update Driver and/or Race
settings depending on how you've configured things. The custom
localization file will be found at \<install
directory\>\data\Languages\custom.json. You can find the location of
"install directory” by going to the menu bar and selecting File → Show
Install Directory.

If the backup file is too large, there may be debug dump files. You can
do the following:

1.  Launch RC

2.  From the menu bar, select File → Open Database Folder.

3.  Look for any files named "RCDump" or something similar. They'll be
    much bigger than everything else. Just delete them. **NOTE:** When
    in doubt do NOT delete anything. Ask for help. If you delete the
    wrong file(s) you could corrupt RC beyond repair, requiring you to
    either undelete the deleted files (if possible) or restore from a
    previously created backup.

4.  From the menu bar, select File → Debug To Zip.

5.  Save the file somewhere safe. You're all backed up!

6.  Make note of the version of RC you're running when the backup was
    made. Consider adding the version number into the filename of the
    file created in step 4. You'll need to know the version when you
    restore the backup. You can get the RC version from the About menu
    on the main setup screen or the bottom right of the splash screen
    when RC starts up

### Restoring the RC Database

RC backup files can be used to restore RC to a previous state either on
the same computer it was created on or a different computer. It does not
matter.

**WARNING: When restoring a backup, the destination PC must be running
the same version of RC or a newer version of RC. If the destination PC
is running an older version of RC than the backup was made from, your
database will eventually get corrupted beyond repair and you'll have to
restore from the backup.**

## Appendix D - XAML Keyboard Shortcuts

Race Coordinator can be modified to use your desired keyboard keys to
control its operation. Below is an example from the XAML file
RaceDay_2L.xaml. In the example, the key combination of ALT-F5 (ALT and
F5 keys pressed at the same time) will skip the current heat. The key
and modifier values can be changed to suit the user’s needs by editing
this line:

\<MenuItem Name="SkipHeat_1" Header="Skip Heat"
DataContext="'**key**':'**F5**','**modifier**':'**Alt**'"
ToolTip="ALT-F5 to skip the remainder of this heat" /\>

The following table lists all the "modifier" values accepted as keyboard
shortcut modifiers. Simply use the text value exactly as shown to the
left of the '=' sign. If the modifier value doesn't match one of these
text values exactly, it will not be set up. None of the text values have
any spaces in them, and they end at the last character before the '='
(i.e., not including the '=' sign). See file KitchenSink_4L.xaml for
examples. The modifier field is required to create some keyboard
shortcuts.

| **TYPE** | **SUMMARY**            | **VALUE**   |
|----------|------------------------|-------------|
| MODIFIER | The ALT Key            | Alt = 1     |
| MODIFIER | The CONTROL (CTRL) Key | Control = 2 |
| MODIFIER | The SHIFT Key          | Shift = 4   |
| MODIFIER | The Windows Logo Key   | Windows = 8 |

The following table lists all the "key" values accepted as a keyboard
shortcut. Simply use the text value exactly as shown to the left of the
'=' sign. If the key value doesn't match one of these text values
exactly, it will not be set up. None of the text values have any spaces
in them, and they end at the last character before the '=' (i.e., not
including the '=' sign). See file KitchenSink_4L.xaml for examples. The
key field is required to create the shortcut. Most keyboard shortcuts
require the "modifier" value to also be set. Numeric values "0", "1",
"2", .., "9" can be used in place of the equivalent "D0", "D1", "D2",
.., "D9" values.

| **TYPE** | **SUMMARY** | **VALUE** | **NOTES** |
|----|----|----|----|
| KEY | The Cancel key | Cancel = 1 |  |
| KEY | The Backspace key | Back = 2 |  |
| KEY | The Tab key | Tab = 3 |  |
| KEY | The Linefeed key | LineFeed = 4 |  |
| KEY | The Clear key | Clear = 5 |  |
| KEY | The Return key | Return = 6 |  |
| KEY | The Enter key | Enter = 6 |  |
| KEY | The Pause key | Pause = 7 |  |
| KEY | The Caps Lock key | CapsLock = 8 |  |
| KEY | The Caps Lock key | Capital = 8 | Alternate value |
| KEY | The IME Hangul mode key | HangulMode = 9 |  |
| KEY | The IME Kana mode key | KanaMode = 9 |  |
| KEY | The IME Junja mode key | JunjaMode = 10 |  |
| KEY | The IME Final mode key | FinalMode = 11 |  |
| KEY | The IME Kanji mode key | KanjiMode = 12 |  |
| KEY | The IME Hanja mode key | HanjaMode = 12 |  |
| KEY | The ESC key | Escape = 13 |  |
| KEY | The IME Convert key | ImeConvert = 14 |  |
| KEY | The IME NonConvert key | ImeNonConvert = 15 |  |
| KEY | The IME Accept key | ImeAccept = 16 |  |
| KEY | The IME Mode change request | ImeModeChange = 17 |  |
| KEY | The Spacebar key | Space = 18 |  |
| KEY | The Page Up key | PageUp = 19 |  |
| KEY | The Page Up key | Prior = 19 | Alternate value |
| KEY | The Page Down key | PageDown = 20 |  |
| KEY | The Page Down key | Next = 20 | Alternate value |
| KEY | The End key | End = 21 |  |
| KEY | The Home key | Home = 22 |  |
| KEY | The Left Arrow key | Left = 23 |  |
| KEY | The Up Arrow key | Up = 24 |  |
| KEY | The Right Arrow key | Right = 25 |  |
| KEY | The Down Arrow key | Down = 26 |  |
| KEY | The Select key | Select = 27 |  |
| KEY | The Print key | Print = 28 |  |
| KEY | The Execute key | Execute = 29 |  |
| KEY | The Print Screen key | PrintScreen = 30 |  |
| KEY | The Print Screen key | Snapshot = 30 | Alternate value |
| KEY | The Insert key | Insert = 31 |  |
| KEY | The Delete key | Delete = 32 |  |
| KEY | The Help key | Help = 33 |  |
| KEY | The 0 (zero) key | D0 = 34 | Can use 0 instead of D0 |
| KEY | The 1 (one) key | D1 = 35 | Can use 1 instead of D1 |
| KEY | The 2 key | D2 = 36 | Can use 2 instead of D2 |
| KEY | The 3 key | D3 = 37 | Can use 3 instead of D3 |
| KEY | The 4 key | D4 = 38 | Can use 4 instead of D4 |
| KEY | The 5 key | D5 = 39 | Can use 5 instead of D5 |
| KEY | The 6 key | D6 = 40 | Can use 6 instead of D6 |
| KEY | The 7 key | D7 = 41 | Can use 7 instead of D7 |
| KEY | The 8 key | D8 = 42 | Can use 8 instead of D8 |
| KEY | The 9 key | D9 = 43 | Can use 9 instead of D9 |
| KEY | The A key | A = 44 |  |
| KEY | The B key | B = 45 |  |
| KEY | The C key | C = 46 |  |
| KEY | The D key | D = 47 |  |
| KEY | The E key | E = 48 |  |
| KEY | The F key | F = 49 |  |
| KEY | The G key | G = 50 |  |
| KEY | The H key | H = 51 |  |
| KEY | The I key | I = 52 |  |
| KEY | The J key | J = 53 |  |
| KEY | The K key | K = 54 |  |
| KEY | The L key | L = 55 |  |
| KEY | The M key | M = 56 |  |
| KEY | The N key | N = 57 |  |
| KEY | The O key | O = 58 |  |
| KEY | The P key | P = 59 |  |
| KEY | The Q key | Q = 60 |  |
| KEY | The R key | R = 61 |  |
| KEY | The S key | S = 62 |  |
| KEY | The T key | T = 63 |  |
| KEY | The U key | U = 64 |  |
| KEY | The V key | V = 65 |  |
| KEY | The W key | W = 66 |  |
| KEY | The X key | X = 67 |  |
| KEY | The Y key | Y = 68 |  |
| KEY | The Z key | Z = 69 |  |
| KEY | The left Windows logo key (Microsoft Natural Keyboard) | LWin = 70 |  |
| KEY | The right Windows logo key (Microsoft Natural Keyboard) | RWin = 71 |  |
| KEY | The Application key (Microsoft Natural Keyboard) | Apps = 72 |  |
| KEY | The Computer Sleep key | Sleep = 73 |  |
| KEY | The 0 key on the numeric keypad | NumPad0 = 74 |  |
| KEY | The 1 key on the numeric keypad | NumPad1 = 75 |  |
| KEY | The 2 key on the numeric keypad | NumPad2 = 76 |  |
| KEY | The 3 key on the numeric keypad | NumPad3 = 77 |  |
| KEY | The 4 key on the numeric keypad | NumPad4 = 78 |  |
| KEY | The 5 key on the numeric keypad | NumPad5 = 79 |  |
| KEY | The 6 key on the numeric keypad | NumPad6 = 80 |  |
| KEY | The 7 key on the numeric keypad | NumPad7 = 81 |  |
| KEY | The 8 key on the numeric keypad | NumPad8 = 82 |  |
| KEY | The 9 key on the numeric keypad | NumPad9 = 83 |  |
| KEY | The Multiply key | Multiply = 84 |  |
| KEY | The Add key | Add = 85 |  |
| KEY | The Separator key | Separator = 86 |  |
| KEY | The Subtract key | Subtract = 87 |  |
| KEY | The Decimal key | Decimal = 88 |  |
| KEY | The Divide key | Divide = 89 |  |
| KEY | The F1 key | F1 = 90 |  |
| KEY | The F2 key | F2 = 91 |  |
| KEY | The F3 key | F3 = 92 |  |
| KEY | The F4 key | F4 = 93 |  |
| KEY | The F5 key | F5 = 94 |  |
| KEY | The F6 key | F6 = 95 |  |
| KEY | The F7 key | F7 = 96 |  |
| KEY | The F8 key | F8 = 97 |  |
| KEY | The F9 key | F9 = 98 |  |
| KEY | The F10 key | F10 = 99 |  |
| KEY | The F11 key | F11 = 100 |  |
| KEY | The F12 key | F12 = 101 |  |
| KEY | The F13 key | F13 = 102 |  |
| KEY | The F14 key | F14 = 103 |  |
| KEY | The F15 key | F15 = 104 |  |
| KEY | The F16 key | F16 = 105 |  |
| KEY | The F17 key | F17 = 106 |  |
| KEY | The F18 key | F18 = 107 |  |
| KEY | The F19 key | F19 = 108 |  |
| KEY | The F20 key | F20 = 109 |  |
| KEY | The F21 key | F21 = 110 |  |
| KEY | The F22 key | F22 = 111 |  |
| KEY | The F23 key | F23 = 112 |  |
| KEY | The F24 key | F24 = 113 |  |
| KEY | The Num Lock key | NumLock = 114 |  |
| KEY | The Scroll Lock key | Scroll = 115 |  |
| KEY | The left Shift key | LeftShift = 116 |  |
| KEY | The right Shift key | RightShift = 117 |  |
| KEY | The left CTRL key | LeftCtrl = 118 |  |
| KEY | The right CTRL key | RightCtrl = 119 |  |
| KEY | The left ALT key | LeftAlt = 120 |  |
| KEY | The right ALT key | RightAlt = 121 |  |
| KEY | The Browser Back key | BrowserBack = 122 | Key values 122 and higher are found on specialty / extended keyboards |
| KEY | The Browser Forward key | BrowserForward = 123 |  |
| KEY | The Browser Refresh key | BrowserRefresh = 124 |  |
| KEY | The Browser Stop key | BrowserStop = 125 |  |
| KEY | The Browser Search key | BrowserSearch = 126 |  |
| KEY | The Browser Favorites key | BrowserFavorites = 127 |  |
| KEY | The Browser Home key | BrowserHome = 128 |  |
| KEY | The Volume Mute key | VolumeMute = 129 |  |
| KEY | The Volume Down key | VolumeDown = 130 |  |
| KEY | The Volume Up key | VolumeUp = 131 |  |
| KEY | The Media Next Track key | MediaNextTrack = 132 |  |
| KEY | The Media Previous Track key | MediaPreviousTrack = 133 |  |
| KEY | The Media Stop key | MediaStop = 134 |  |
| KEY | The Media Play Pause key | MediaPlayPause = 135 |  |
| KEY | The Launch Mail key | LaunchMail = 136 |  |
| KEY | The Select Media key | SelectMedia = 137 |  |
| KEY | The Launch Application1 key | LaunchApplication1 = 138 |  |
| KEY | The Launch Application2 key | LaunchApplication2 = 139 |  |
| KEY | The OEM Semicolon key | OemSemicolon = 140 |  |
| KEY | The OEM 1 key | Oem1 = 140 |  |
| KEY | The OEM Addition key | OemPlus = 141 |  |
| KEY | The OEM Comma key | OemComma = 142 |  |
| KEY | The OEM Minus key | OemMinus = 143 |  |
| KEY | The OEM Period key | OemPeriod = 144 |  |
| KEY | The OEM Question key | OemQuestion = 145 |  |
| KEY | The OEM 2 key | Oem2 = 145 |  |
| KEY | The OEM Tilde key | OemTilde = 146 |  |
| KEY | The OEM 3 key | Oem3 = 146 |  |
| KEY | The ABNT_C1 (Brazilian) key | AbntC1 = 147 |  |
| KEY | The ABNT_C2 (Brazilian) key | AbntC2 = 148 |  |
| KEY | The OEM Open Brackets key | OemOpenBrackets = 149 |  |
| KEY | The OEM 4 key | Oem4 = 149 |  |
| KEY | The OEM Pipe key | OemPipe = 150 |  |
| KEY | The OEM 5 key | Oem5 = 150 |  |
| KEY | The OEM Close Brackets key | OemCloseBrackets = 151 |  |
| KEY | The OEM 6 key | Oem6 = 151 |  |
| KEY | The OEM Quotes key | OemQuotes = 152 |  |
| KEY | The OEM 7 key | Oem7 = 152 |  |
| KEY | The OEM 8 key | Oem8 = 153 |  |
| KEY | The OEM Backslash key | OemBackslash = 154 |  |
| KEY | The OEM 102 key | Oem102 = 154 |  |
| KEY | A special key masking the real key being processed by an IME | ImeProcessed = 155 |  |
| KEY | A special key masking the real key being processed as a system key | System = 156 |  |
| KEY | The OEM ATTN key | OemAttn = 157 |  |
| KEY | The DBE_ALPHANUMERIC key | DbeAlphanumeric = 157 |  |
| KEY | The OEM FINISH key | OemFinish = 158 |  |
| KEY | The DBE_KATAKANA key | DbeKatakana = 158 |  |
| KEY | The DBE_HIRAGANA key | DbeHiragana = 159 |  |
| KEY | The OEM COPY key | OemCopy = 159 |  |
| KEY | The DBE_SBCSCHAR key | DbeSbcsChar = 160 |  |
| KEY | The OEM AUTO key | OemAuto = 160 |  |
| KEY | The DBE_DBCSCHAR key | DbeDbcsChar = 161 |  |
| KEY | The OEM ENLW key | OemEnlw = 161 |  |
| KEY | The OEM BACKTAB key | OemBackTab = 162 |  |
| KEY | The DBE_ROMAN key | DbeRoman = 162 |  |
| KEY | The DBE_NOROMAN key | DbeNoRoman = 163 |  |
| KEY | The ATTN key | Attn = 163 |  |
| KEY | The CRSEL key | CrSel = 164 |  |
| KEY | The DBE_ENTERWORDREGISTERMODE key | DbeEnterWordRegisterMode = 164 |  |
| KEY | The EXSEL key | ExSel = 165 |  |
| KEY | The DBE_ENTERIMECONFIGMODE key | DbeEnterImeConfigureMode = 165 |  |
| KEY | The ERASE EOF key | EraseEof = 166 |  |
| KEY | The DBE_FLUSHSTRING key | DbeFlushString = 166 |  |
| KEY | The PLAY key | Play = 167 |  |
| KEY | The DBE_CODEINPUT key | DbeCodeInput = 167 |  |
| KEY | The DBE_NOCODEINPUT key | DbeNoCodeInput = 168 |  |
| KEY | The ZOOM key | Zoom = 168 |  |
| KEY | A constant reserved for future use | NoName = 169 |  |
| KEY | The DBE_DETERMINESTRING key | DbeDetermineString = 169 |  |
| KEY | The DBE_ENTERDLGCONVERSIONMODE key | DbeEnterDialogConversionMode = 170 |  |
| KEY | The PA1 key | Pa1 = 170 |  |
| KEY | The OEM Clear key | OemClear = 171 |  |
| KEY |  | DeadCharProcessed = 172 | Alternate Value? |
