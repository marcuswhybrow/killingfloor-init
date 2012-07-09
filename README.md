# KillingFloor Init

A Debian init script for starting, stopping and updating a single KillingFloor server.

I don't expect to develop this much further, but it may however be of help to others.

## Installation

1. Visit the TripwireInteractive [wiki page for installing a server][wiki-install].

1. Once installed, just copy the `killingfloor` file to your `/etc/init.d` directory, and update your rc.d links:

    ```
    sudo wget https://raw.github.com/marcuswhybrow/killingfloor-init/latest/killingfloor -O /etc/init.d/kf
    sudo chmod 755  /etc/init.d/kf
    sudo update-rc.d kf defaults
    ```

2. Then, edit `/etc/init.d/kf` and change the variables to point to your installation location.


[wiki-install]: http://wiki.tripwireinteractive.com/index.php/Dedicated_Server_(KillingFloor)
