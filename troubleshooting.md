# Common troubleshooting Linux

### 1. Fix ping operation not permited

This problem is probably related to permission issues in the ping executable file.
To fix this problem is pretty simple.

```bash
which ping # Find folder location (Normally this output /usr/bin/ping/
sudo chmod 4711 /usr/bin/ping/
ping google.com
```
