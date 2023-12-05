Meadows_Battery_Diagnostics_Tool

Battery health survey software

Write in: C, Shell

Note: Despite being a Meadows software piece, it is compatible with other Linux distributions

Sends diagnostics about your battery to a server once per hour, a ~4 kilobyte packet (just ~96 KB/day)

- Integration with GNOME Power Settings
- Gathering bathery data
- 100% voluntary
- Encrypted with 512 bit encryption

Internal flags

--charging
--discharging
--slow-charging
--fast-charging-i
--fast-charging-ii
--fullcharge
--lowbattery
--ac-power
--supply
--updates
--firmware
--inductive-charging
--wired-charging
--voltage.perminute
--voltage.persecond
--energy-design.full
--energy-design.current
--device-type.laptop
--device-type.pda
--device-type.cell-phone
--device-type.tv
--device-type.monitor
--device-type.mouse
--device-type.keyboard
--device-type.router
--device-type.battery-backup
--time-to-full
--time-to-empty
// Multiple system tasks can be done at once
--system-task.idle
--system-task.video-rendering
--system-task.video-playback
--system-task.audio-playback
--system-task.audio-converting
--system-task.video-converting
--system-task.sleep-mode
--system-task.hibernation
--system-task.video-games
--system-task.stress-test
--system-task.file-transfer
--system-task.uploading
--system-task.downloading
--system-task.image-editing
--system-task.image-viewing
--system-task.compiling
--system-task.decompiling
--system-task.forkbomb
--system-task.memory-leak
--system-task.installation
--system-task.uninstallation
--system-task.system-updates
--system-task.application-updates
--system-task.virtual-machines
--system-task.vector-images
--system-task.torrent
--system-task.standby
--system-task.document-editing
--system-task.document-viewing
// Required subflags
---program = ["gedit.desktop", "vlc.desktop", "firefox.desktop", "virtualbox.desktop"]
// Shortcut desktop files are placed in the battery diagnostics directory with a symbolic link to the specific program and version
---operating_system = ["ubuntu(22.04).cfg", "meadows(1).cfg"] // The second option indicates a dual-boot operating system
// Shortcut config files are placed in the battery diagnostics directory with a symbolic link to the specific setup and version
---number-of-programs = [4]
--time = 10101010 // UNIX time at the time of logging
