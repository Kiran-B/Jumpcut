# Jumpcut
A minimalist application to provide clipboard buffering for macOS written by snarkout.

This repo is an import from https://sourceforge.net/projects/jumpcut/

For more details, please see the original project page.

Retaining the license of the original author, which is MIT license. All credits goes to the original author.

## Purpose:
The original app served me well as it worked well until macOS Mojave. When I switched to macOS Catalina, this was the app that I immediately missed. Hence this repo. 

This repo makes the app 64-bit compatible and thus supports macOS Catalina. I love this app for its minimalism and thus I would not attempt to add features. 

## Compatibility:
macOS 10.6 (Snow Leopard) ~ 10.15 (macOS Catalina)

Note: I have tested this only in Mojave and Catalina.

## Install:

1. Build and run:
- Get [Xcode 10.2.1](https://developer.apple.com/download/)
- Download the [code](https://github.com/Kiran-B/Jumpcut/archive/0.0.66.tar.gz) and build/run the app.
2. Allow the app to run accepting the risk that it was from an unidentified developer. Here is how you may do it:
- control-click (right-click) the app icon, then choose Open from the contextual menu.
- You would see an alert that says Jumpcut is from an unidentified developer. Click `Open` in the alert.

The above step will be a one time thing.

More details here: https://support.apple.com/kb/ph25088 

A pictorial version is available here: https://www.imore.com/how-open-apps-unidentified-developers-mac

## Additional permissions:
Jumpcut does not need special macOS permission to track and record global clipboard. But, Jumpcut makes use of accessibility APIs to paste recorded content on to the current app. When you use this feature for the first time, macOS (for obvious security and privacy reason) puts up an alert. The alert seeks your permission to allow Jumpcut to use the accessibility feature. I recommend you to review this [Apple Support document](https://support.apple.com/guide/mac-help/mh43185/mac) for more information.

If you had denied the permission, you could change it. Open System Preferences, click Privacy, click Accessibility, then select the app’s checkbox. Unselect the app’s checkbox to remove the permission anytime.

Paste workflow without the accessibility permission:
- Use paste shortcut one or more time to chose the content you want to paste. 
- Wait for the bezel to fade off and let the current app gain focus
- Use paste shortcut of the app

Paste workflow with the accessibility permission:
- Use paste shortcut one or more time to chose the content you want to paste. The last chosen content will paste onto the current app.

Hints:
- When the paste bezel is active, use arrow keys to chose previous or next clipboard.
- App allows pasting previous content from the Jumpcut menu. For this, enable 'Menu selection paste' in preferences.

## TODO:
[ ] Explore generation of a code-signed/notarized build 

[ ] Distribution via Homebrew

[ ] Update image assets to support Retina screen, if anyone could contribute image assets. 

## Build:

Use Xcode 10.2.1

## Download pre-built binary:
Download Jumpcut.app.zip from [here](https://github.com/Kiran-B/Jumpcut/releases)
