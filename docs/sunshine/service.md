# Service

## Windows

If you installed sunshine through the installer:

Press `WIN+R`, then type `services.msc` and hit `enter`.

Scroll down until you find `SunshineService`.
 
If you found it, make sure it is running and set to start automatically.

If you can't find it, go to `C:\Program Files\Sunshine\scripts` and run `install-service.bat` as admin (right click).

## Linux

Check if the service is running:

```bash
systemctl status sunshine
```

If it is not running, start it:

```bash
systemctl --user start sunshine
```

If you want to enable it to start on boot, run:

```bash
systemctl --user enable sunshine
```

If you want to disable the service, run:

```bash
systemctl --user disable sunshine
```

## Homebrew
If you installed sunshine through Homebrew, you can check the status of the service with:

```bash
brew services list
```

If you want to enable it to start on boot, run:

```bash
brew services start sunshine
```

If you want to enable it to run on user login, run:

```bash
brew services run sunshine
```

If you want to disable the service, run:

```bash
brew services stop sunshine
```

For more information see our
[getting started docs](https://docs.lizardbyte.dev/projects/sunshine/latest/md_docs_2getting__started.html)
