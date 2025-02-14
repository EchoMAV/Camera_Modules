# Camera_Modules
Device tree overlays and setup scripts for applicable camera modules.

This repo currently contains a device tree overlay for the EchoMAV IMX477 (standalone and used in the Fermion) to be used with the EchoPilot AI.
Add the `tegra234-p3767-camera-p3768-imx477-custom-echopilot-ai-overlay.dtbo` overlay to the rootfs `/boot/` folder and modify the `/boot/extlinux/extlinux.conf` to include the following lines on an existing or new boot entry.

```
      FDT /boot/dtb/edit-me-with-name-of-dtb-in-this-folder.dtb
      OVERLAYS /boot/tegra234-p3767-camera-p3768-imx477-custom-echopilot-ai-overlay.dtbo
```

