This repo has some kernel mods used to make the BeagleBone Black into a
functioning USB Human Interface Device (HID) Keyboard *and* keep the existing
NIC/Mass Storage/TTY USB gadget functionality.  I couldn't do this without a
modified kernel even though it should in theory be possible via libcomposite.
I was hitting bugs like [this](https://github.com/torvalds/linux/commit/749494b6bdbbaf0899aa1c62a1ad74cd747bce47).

This can be used with [saipanel](https://github.com/andrewjjenkins/saipanel) to
turn your BeagleBone Black into a proxy for old game controllers that don't
have good windows drivers anymore.
