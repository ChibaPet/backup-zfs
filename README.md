## backup-zfs

This is an elaboration of what I've been using myself for some years. It
can be used to back up systems, to populate off-site back-up media from a
back-up pool, etc.

It's intended to run unproblematically on both FreeBSD and GNU/Linux using
their respective Almquist-derived system shells.

Don't forget to create a dataset to hold pools from your system.

Don't forget to test this before setting it running like the Sorcerer's
Apprentice.

Don't forget to test your back-ups rather than assuming they're usable.

Note that if you restore from back-ups made with this, we're setting
canmount=off when we ship snapshots from the original system, but we store
the original values in the archive:canmount property.

Please read the script before running it. Please tell me about bugs you
see in it.
