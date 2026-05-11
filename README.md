# Heos Controller
Desktop controller for [Denon Heos](http://heosbydenon.denon.com) wifi speakers.

⚠️ This project has been rebuilt and migrated to: https://github.com/cold-logic/heos-controller

## Screenshot

![](screenshot.png)

## Features
* Automatic detection of speakers
* User friendly volume dial
* Playback controls (previous, play/pause, next)

## Usage
1. [Download a release](https://github.com/cold-logic/heos-controller/releases) and extract the app into your Applications directory
2. Run the app and wait for speaker detection
3. Select a speaker from the dropdown and use the controls

## Development
1. Clone this repo
2. Install all the dependencies using the `pnpm install` command
3. Run the app using `pnpm start`
4. To preview changes made in the *app* directory while the app is running, refresh with the (cmd-r) hot key
5. Dev tools are available using the (cmd-opt-i) hot key

## Generating the compiled app
1. Rename `.env.example` to `.env`. This will disable code signing.
2. To generate only the app bundle run: `pnpm run pack`
3. To generate the app bundle, ZIP and DMG, run: `pnpm build`
4. Look in the `dist` folder for the results

## ToDo
* Detection and control of grouped speakers
* Details about the currently playing stream
* A slider to scrub and track playback position
* A "sources" media stream picker

## Reference Materials

- https://rn.dmglobal.com/usmodel/HEOS_CLI_ProtocolSpecification-Version-1.16.pdf
- http://rn.dmglobal.com/euheos/HEOS_CLI_ProtocolSpecification.pdf
- https://support.denon.com/app/answers/detail/a_id/6953/~/heos-control-protocol-%28cli%29
