The syntax is:

mxdpi <dpi level> <hidraw device>
<dpi level> should be an integer in {0,...,14}. Higher integers correspond to higher dpi settings.

<hidraw device> is the hidraw device that corresponds to your mouse. This should usually be /dev/hidraw< X >", where < X > is an integer. You can find the right device name by executing

cat /sys/class/hidraw/hidraw< X >/device/uevent
for all integers < X > for which this file exists.
