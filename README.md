# Flo Tools
#Welcome!
Welcome to Flo Tools! This product was developed to enhance the usability and improve workflow for VoiceOver users of Pro Tools.
This document is divided into headings for easier screen reader navigation. Read below to get started.

#Acknowledgements:

Flo Tools was first developed as a concept by Chi Kim and Rocco Fiorentino, in the Assistive Music Technology Lab at Berklee College of Music. After realizing the potential of the project, Slau Halatyn joined the team, and the group worked together to continue developing the scripts outside of the classroom. Many thanks to Rocco Fiorentino for his contribution to writing scripts and documentation. And many thanks to Slau Halatyn, who beta tested Flo Tools and gave invaluable feedback with his expert knowledge in Pro Tools. We’d also like to thank Chi Kim for his time, effort, and creative scripting abilities to make this project a success. We sincerely hope Flo Tools will enhance the work flow of Pro Tools users with visual impairments!

#Note:

The  zip file referenced in this read me will automatically decompress itself into a folder on Mac OS. Please refer to this downloaded folder, called "Flo Tools Master", when reading this document.

You can download the zip file directly from [here](https://github.com/rfiorentino1/Flo-Tools/archive/master.zip)

#System Requirements:

Flo Tools supports Mac OS version 10.10 or later, and Pro Tools version 12.3 or later. Earlier versions of Mac OS and Pro Tools may provide limited functionality with Flo Tools, but have not been tested and are not guaranteed to function correctly.

#Installation
Flo Tools relies on a third party program, called Keyboard Maestro. Download instructions are below.

##Keyboard Maestro Installation:

1. Go to the Keyboard Maestro homepage by clicking [here](https://www.keyboardmaestro.com/) and download the Keyboard Maestro application from the website.

2. Copy the Keyboard Maestro application from the downloads folder to your applications folder. From there, open Keyboard Maestro.


##Flo Tools Installation
To install Flo Tools, go to the provided zip file, and open the file called "Flo Tools.kmmacros"

If successful, Keyboard Maestro should announce, "Successfully imported macros."

For the scripts to run correctly, open Keyboard Maestro Preferences, and under the general tab, check the checkbox that says "start Keyboard Maestro Engine at log-in."

##Note:
Keyboard Maestro is limited by a 30-day trial period. After this time, you will need to purchase a one-time license to continue using the program, and subsequently, Flo Tools.


###Getting Started

###Auditory Feedback:

Flo Tools uses 2 distinct sounds to provide auditory feedback. The first is [this sound](file:///System/Library/Sounds/Pop.aiff), which signals that something is in process and the user needs to wait for Flo Tools to complete a task. An example of this would be deselecting all tracks in a large session.

The second is [this sound](file:///System/Library/Sounds/Tink.aiff), which tells a user that something has been toggled, such as solo on and off.

###Commands:

Flo Tools has two groups of commands. The first, called "Flo Tools", is always active, and applies to the entire session. The second group, called "Flo Tools Inspector", is active by default, but can be toggled on and off. The inspector only applies to an individual track.

Below is a list of Flo Tools commands, and their associated functions, separated by their respective groups.

###Flo Tools:

Where two actions are listed, double-tapping the key will perform the second action.

- Speak selection start: Command+f1
- Speak Selection End: Command+f2
- Speak Selection Length: Command+f3
- Speak main counter: Command+f4
- Close All Floating Windows: Command+Option+w
- Zoom/Maximize Window: Command+Option+Control+z (must be passed through)
- Show All Tracks: Option+f1
- Hide All Tracks: Option+f2
- Show Only Selected Tracks: Option+Shift+f1
- Hide Selected Tracks: Option+Shift+f2
- Speak Selected Tracks, Deselect All Tracks: Option+Shift+t
- Speak Input Monitor-Enabled Tracks, Disable Input Monitor On All Tracks: Option+Shift+k
- Speak Record-Enabled Tracks, Disarm All Record Enabled Tracks: Option+Shift+r
- Speak Soloed Tracks, Unsolo All Tracks: Option+Shift+s
- Speak Muted Tracks, Unmute All Tracks: Option+Shift+m
- Speak Record Safe Tracks: Command+Option+Shift+r
- Speak Solo Safe Tracks: Command+Option+Shift+s
- Speak Clipped Tracks: Option+Shift+c
- Control-Click: Control+x
- Option-Click: Option+x
- Option+Shift-Click: Option+Shift+x
- Command-Click: Command+Control+x
- Command+Option-Click: Command+Option+x

Note: For click simulation to work properly, the desired track must be visible. Scroll to the track if necessary by pressing VO f and typing the track number.


###Flo Tools Inspector:

The following commands apply to the current track that VoiceOver is focused on. This means the track name must be under the VoiceOver cursor, and the user should not be interacted with anything inside the track.

Note: The inspector must be disabled to use first-letter navigation in pop-up menus in Pro Tools.

Where 2 actions are listed, double tapping the key will perform the second action.

- Activate Inspector: /
- Deactivate Inspector: Shift+/
- Speak Track Name, Select Track Pop-Up Menu: t
- Speak/Open Inserts A through J: 1 through 0
- Assign Inserts A through J: Command+1 through 0
- Speak/Open Sends A through J: Control+1 through 0
- Assign Sends A through J: Command+Control+1 through 0
- Speak/Select Input: i
- Speak/Select Output: o
- Beta: Speak/Select Automation Mode: a
- Speak/Select Group: g
- Speak/Reset Pan: n
- Speak/Toggle Input Monitor: k
- Speak/Toggle Record State: r
- Speak/Toggle Solo: s
- Speak/Toggle Mute: m
- Speak/Reset Volume Fader: v
- Speak/Reset Level Meter: l
- Speak/Reset Peak Meter: p
- Speak/Reset Gain Reduction Meter: g
- Speak/Edit Comments: c
- Beta: Track Options Menu: h
- Speak/Select Playlist: \
- Beta: Speak/Select Track View: w
- Speak/Toggle Freeze Status: f
- Speak/Select Timebase: b
- Beta: Speak/Select Elastic Audio Plugin: e


####Changing Shortcuts

The shortcuts outlined above are the default assignments for Flo Tools. They can be changed based on personal preference, however, when Flo Tools is updated, the shortcuts will revert back to their default assignments. If you feel that you want to change a shortcut, open Keyboard Maestro and do the following:

1. Go to the view menu, and select "start editing macros."
2. Find the Macro Groups scroll area and interact with it. Inside, find and select the appropriate Flo Tools macro group by pressing VO space on it.
3. Stop interacting with this area and move to the right to the macros scroll area.

  - Interact, and find the script with the shortcut you want to change. Press VO space to select it, and press tab.

This should move you inside the edit screen of the macro. VO right arrow, and you should see a button, labeled with the current shortcut for the script.

To change it, simply type your new desired shortcut and then stop interacting with the edit area. Be careful not to press command tab here, as this will assign it self as a new shortcut.


####Reporting Issues:

GitHub provides a convenient and reliable way to track and resolve issues. Please click [here](https://github.com/rfiorentino1/Flo-Tools/issues), and search for your issue. If you don't find an open issue relating to your problem with Flo Tools, you can create a new one by clicking on "new issue" and filling out the required fields.


####Known Issues

* Checking the arm state of tracks does not report consistently. This is due to the way that Pro Tools indicates whether a track is record enabled. To work around this, check the arm state multiple times.
