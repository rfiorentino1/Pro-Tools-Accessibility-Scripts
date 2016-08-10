# Pro-Tools-Accessibility-Scripts
#Welcome!
Welcome to the Pro Tools Accessibility Scripts. These scripts were developed to enhance the usability of Pro Tools for VoiceOver users.
This document is divided into headings for easier screen reader navigation. Read below to get started.
#Note:

The downloaded zip file, referenced in this read me, will automatically decompress itself into a folder on Mac OS. Please refer to this downloaded folder, called "Pro Tools Accessibility Scripts Master", when reading this document.

#Installation
These scripts rely on a third party program, called Keyboard Maestro. Download instructions are below.

##Keyboard Maestro Installation:

1. Go to the Keyboard Maestro homepage by clicking [here](https://www.keyboardmaestro.com/) and download the Keyboard Maestro application from the website.

2. Copy the Keyboard Maestro application from the downloads folder to your applications folder. From there, open Keyboard Maestro.


##Script Installation
To install the script files, go to the provided zip file, and open the file called "Protools scripts.kmmacros"

If successful, Keyboard Maestro should announce, "Successfully imported macros."

##Note:
Keyboard Maestro is limited by a 30-day trial period. After this time, you will need to purchase a one-time license to continue using the program, and subsequently, the scripts.

##Setting Up More Advanced Script Functions:

In future revisions and updates to this set of scripts, it will be necessary to utilize certain script libraries to perform functions. Currently, this only applies to the commands related to mouse click simulation, but it's a good idea to set up the folder structure now, for later use. To do this, follow the steps below:

1. Go to the finder, and press command shift G, to open the go to folder window.

Type "~/Library", and press enter. This should bring you to your User library folder, hidden by default.

2. Inside this folder, look for a folder called "Script Libraries." If it doesn’t exist, please create it.

3. In the provided zip file, copy the file called "KMV.scpt", and paste it into the Script Libraries folder.


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

  - Control shift A: arm state
  - Control shift s: solo state
  - Control shift m: mute state
  - Control shift e: selection state

- Speak track meter: option m
  - This command speaks the meter level of the current track under the VoiceOver cursor

- Unarm all tracks: option shift a

- Unsolo all tracks: option shift s

- Unmute all tracks: option shift m

- Unselect all tracks: Control U

###Changing Shortcuts

The shortcuts outlined above are the default assignments for the scripts. They can be changed based on personal preference, however, when the scripts are updated, the shortcuts will revert back to their default assignments. If you feel that you want to change a shortcut, open Keyboard Maestro and do the following:

1. Find the Macro Groups scroll area and interact with it. Inside, find and select the protools macro group by pressing VO space on it.
2. Stop interacting with this area and move to the right to the macros scroll area.

  - Interact, and find the script with the shortcut you want to change. Press VO space to select it, and press tab.

This should move you inside the edit screen of the macro. VO right arrow, and you should see a button, labeled with the current shortcut for the script.

To change it, simply type your new desired shortcut and then stop interacting with the edit area. Be careful not to press command tab here, as this will assign it self as a new shortcut.

####Known Issues

* Checking the arm status of tracks does not report consistently. There is no work around for this presently, but it is due to the way that Pro Tools indicates whether a track is record enabled.

* Track Meter command does not function. We're currently working on this, and will have it fixed as soon as possible.
