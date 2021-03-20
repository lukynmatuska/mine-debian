# Mine Debian
Custom debian iso for automatic mining (e. g. in netboot)

## How to
I recommend use Debian Buster.
1. Install dependecies
`sudo apt install -y live-build`
2. Configure the live-build
`lb config --archive-areas "main contrib non-free" --distribution buster --debian-installer-distribution buster --bootappend-live "boot=live components hostname=live-mine-debian"`
3. Build the image
`lb build`
