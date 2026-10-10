# SOARC-ATV
SOARC Software Suite Amateur TV Android App
# SOARC ATV Studio

**Android Amateur Television Camera & Production App**

Part of the **SOARC Radio Suite**

Copyright NB7N - Beaner Industries in Association with Jack Ruby Productions

---

## About

SOARC ATV Studio is an Android application designed for amateur radio operators experimenting with analog Amateur Television (ATV).

The app turns a compatible Android phone into a portable ATV camera and production console. It provides a live camera view, ATV-friendly framing, station identification, test patterns, photo/video recording, and external HDMI program output for use with an external analog television modulator and RF equipment.

The project is being developed for practical amateur-radio use rather than commercial broadcasting. The goal is a simple, reliable and good-looking system that can be used for local ATV contacts, demonstrations, club activities and experimentation.

SOARC ATV Studio is part of the **SOARC Radio Suite**, a family of amateur-radio applications developed around Southern Oregon Amateur Radio Club activities.

---

## Current Status

**Alpha software**

The application is actively being developed and tested with real Android hardware and an analog ATV equipment chain.

Some hardware behavior varies by phone model, HDMI adapter, television/modulator and Android version.

---

## Features

- Live Android camera preview
- Rear and front camera selection
- Phone screen remains usable as a live filming monitor
- External HDMI/program display support
- 4:3 ATV/NTSC framing
- Optional 16:9 display mode
- Callsign overlay
- SOARC station bug/logo
- Clock/date overlay
- Color-bar test pattern
- Standby/test screen
- Front/rear camera switching
- Camera zoom controls
- Smoother incremental zoom
- Camera torch control where supported
- Still-photo capture
- MP4 video recording
- Screen rotation support
- Portrait and landscape phone layouts
- Microphone/audio monitoring options
- Audio level adjustment
- Device temperature monitoring
- Thermal protection options for extended operation
- Multiple interface themes
- Remembered user settings
- Shared media storage with other SOARC applications

---

## SOARC Radio Suite

Photos and recordings created by SOARC applications are organized under:

`DCIM/SOARC Radio Suite`

Files retain an application-specific prefix so they remain easy to identify.

Examples:

`SOARC_ATV_...`

`SOARC_SSTV_...`

This allows SOARC ATV Studio, SOARC SSTV and future SOARC applications to share a clean and consistent media location.

---

## Typical Analog ATV Setup

A basic system can look like this:

Android Phone  
↓  
USB-C to HDMI Adapter  
↓  
HDMI Cable  
↓  
Analog TV / ATV Modulator  
↓  
Linear RF Amplifier  
↓  
RF Filter  
↓  
50-ohm Feedline  
↓  
70 cm Antenna

A television, monitor, dummy load and appropriate test equipment can be used during bench testing.

### Important

**SOARC ATV Studio is not an RF transmitter.**

The application produces and manages the camera/audio/program content. RF modulation, amplification, filtering and transmission are performed by external amateur-radio hardware.

---

## Tested Development Concept

Development has included testing with equipment such as:

- Samsung Galaxy Android phones with USB-C HDMI output
- HDMI-to-analog-TV RF modulation
- Analog NTSC television monitoring
- UHF/70 cm RF amplifier hardware
- 50-ohm amateur-radio RF equipment

Not every Android phone supports wired HDMI output. Check the specifications of your device before purchasing adapters.

---

## Picture Quality

Analog ATV is standard-definition television.

Do not expect modern HD streaming quality after the signal passes through an analog NTSC modulator and amateur-radio RF link.

The goal is a stable, clearly recognizable and enjoyable picture suitable for amateur-radio communication.

Signal quality will depend heavily on:

- RF power
- Amplifier linearity
- Feedline loss
- Antenna gain
- Terrain
- Distance
- Interference
- Receiver quality
- Modulator setup

---

## Recording

SOARC ATV Studio can capture:

- Still photographs
- MP4 video recordings

Media is stored in the shared:

`DCIM/SOARC Radio Suite`

folder.

Recording is independent of the transmitted analog RF signal and provides a local copy of what the camera is seeing.

---

## Building the Android App

The project includes one primary Windows build file:

`BUILD RELEASE.bat`

Double-click it to build the release.

The build system is designed to handle the normal Android build process automatically, including:

- Java detection
- Android SDK detection
- Required SDK components
- Gradle
- Automated tests
- Android lint checks
- Signed release APK
- Google Play AAB
- Release packaging

Finished files are placed in the:

`RELEASE`

folder.

### Signing

Android applications must be digitally signed.

The build system automatically creates and then reuses the same local signing identity so later versions can be installed as upgrades over earlier versions.

The signing key is kept outside the source project and **must not be uploaded to GitHub**.

Do not commit passwords, private signing keys or other credentials to the repository.

---

## Installing

For direct Android installation, use the APK generated in the `RELEASE` folder.

A newer version should install over an older version when:

- The Android package name has not changed
- The same signing identity is used
- The new build has a higher Android version code

User settings should normally remain intact during an upgrade.

---

## Google Play

The release builder also generates an Android App Bundle (`.aab`) for Google Play distribution.

Google Play releases may have additional store, privacy, signing and policy requirements.

---

## Amateur Radio Use

This software is intended for licensed amateur-radio experimentation.

Users are responsible for ensuring that their complete transmitting system complies with applicable laws and regulations, including requirements involving:

- Authorized amateur frequencies
- Station identification
- Necessary bandwidth
- RF emissions
- Spurious emissions
- Transmitter power
- Interference
- Equipment safety

Band plans and local coordination recommendations may also be useful when choosing an operating frequency.

---

## RF Safety

Always test new RF hardware into a suitable dummy load before connecting an antenna.

Make sure that:

- The amplifier has the correct supply voltage and polarity
- The RF output is properly terminated
- The dummy load has adequate power handling
- The amplifier has adequate cooling
- Appropriate filtering is used
- 50-ohm RF equipment is used where required
- RF output is not accidentally connected directly to a television or phone

---

## Known Limitations

SOARC ATV Studio is still under active development.

Current limitations may include:

- HDMI behavior varies between Android devices
- Some phones do not support wired HDMI output
- External displays may behave differently depending on Samsung DeX or manufacturer-specific software
- Analog NTSC output resolution is inherently much lower than the phone camera resolution
- Some camera and microphone capabilities depend on the individual Android device
- External RF equipment is not automatically controlled unless a supported hardware interface is added

---

## Project Goals

The project is intended to remain:

- Easy to operate
- Useful in the field
- Reliable
- Visually clean
- Amateur-radio focused
- Free of unnecessary complexity
- Friendly to inexpensive experimental hardware
- Suitable for both individual operators and radio-club use

Future development may expand the SOARC Radio Suite with additional amateur-radio tools and greater integration between applications.

---

## Related Project

**SOARC SSTV**

SOARC SSTV is the companion Slow Scan Television application in the SOARC Radio Suite.

The applications share common branding, file-management conventions and an overall amateur-radio-focused design philosophy.

---

## Feedback and Testing

This project is under active development.

Bug reports, hardware compatibility reports and useful feature suggestions are welcome through the GitHub Issues section.

When reporting a problem, it is helpful to include:

- App version
- Android phone/model
- Android version
- HDMI adapter or external hardware being used
- What you expected to happen
- What actually happened
- Screenshots or build logs when applicable

---

## License / Copyright

Copyright NB7N - Beaner Industries in Association with Jack Ruby Productions

SOARC and Southern Oregon Amateur Radio Club branding remains associated with its respective organization.

See the repository license and accompanying documentation for redistribution terms.
