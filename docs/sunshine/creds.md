# Forgotten Credentials

If you forgot your credentials to the web UI, try this.

## General

```bash
sunshine --creds {new-username} {new-password}
```

## AppImage (Linux)

```bash
./sunshine.AppImage --creds {new-username} {new-password}
```

## Flatpak (Linux)

### From github.com/LizardByte releases

```bash
flatpak run --command=sunshine dev.lizardbyte.Sunshine --creds {new-username} {new-password}
```

### From Flathub

```bash
flatpak run --command=sunshine dev.lizardbyte.app.Sunshine --creds {new-username} {new-password}
```

This information is also available in our
[troubleshooting docs](https://docs.lizardbyte.dev/projects/sunshine/en/latest/troubleshooting/general.html#forgotten-credentials)
