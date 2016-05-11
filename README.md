# Pro-Tools-Accessibility-Scripts
#Welcome!
Welcome to the Pro Tools Accessibility Scripts. These scripts were developed to enhance the usability of Pro Tools for VoiceOver users.
This document is divided into headings for easier screen reader navigation. Read below to get started.
#Installation
These scripts rely on a third party program, called Keyboard Maestro. Download instructions are below.

1. Go to the Keyboard Maestro homepage by clicking [here](https://www.keyboardmaestro.com/) and download the Keyboard Maestro application from the website.

2. Copy the Keyboard Maestro application from the downloads folder to your applications folder. From there, open Keyboard Maestro.


##Script Installation
To install the script files, go to the file menu of Keyboard Maestro, and select Import Macros.

A dialogue will appear asking you to choose a file. Navigate to the contents of the provided zip file, and choose: protools scripts.kmmacros.

If successful, Keyboard Maestro should announce: Successfully imported macros.

##Note:
Keyboard Maestro is limited by a 30-day trial period. After this time, you will need to purchase a one-time license to continue using the program, and subsequently, the scripts.

###Getting Started

Below is a list of commands, and their associated descriptions.

- Close any PT window that is not Mix or Edit: command option W

- simulate option click: control x

- simulate option shift click: control shift x
  - Note: for any click simulation to work properly, you need to scroll to the track that you want to work with by pressing VO f and typing the track number.

- Speak current counter position: command 0

- Speak selection start: command 1

- Speak selection end: command 2

- Speak selection length: command 3

- Track Status: find out what tracks are armed, soloed, muted, or selected:

  - Option shift a: arm state
  - Option shift s: solo state
  - Option shift m: mute state
  - Option shift e: selection state

- Speak track meter: option m
  - This command speaks the meter level of the current track under the VoiceOver cursor

- Unarm all tracks: option shift a, twice quickly

- Unsolo all tracks: option shift s, twice quickly

- Unmute all tracks: option shift m, twice quickly

###Changing Shortcuts

The shortcuts outlined above are the default assignments for the scripts. They can be changed based on personal preference. If you feel that you want to change a shortcut, open Keyboard Maestro and do the following:

- 1\. Find the Macro Groups scroll area and interact with it. Inside, find and select the protools macro group by pressing VO space on it.
- 2\. Stop interacting with this area and move to the right to the macros scroll area.

  - Interact, and find the script with the shortcut you want to change. Press VO space to select it, and press tab.

This should move you inside the edit screen of the macro. VO right arrow, and you should see a button with the current shortcut for the script.

To change it, simply type your new desired shortcut and then stop interacting with the edit area. Be careful not to press command tab here, as this will assign it self as a new shortcut.

####Known Issues

* Checking the arm status of tracks does not report consistently. There is no work around for this presently, but it is due to the way that Pro Tools indicates whether a track is record enabled.

