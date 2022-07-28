buffer
------

This package provides a circular buffer implementation backed by an MMAP'd
file.  It's purpose is to provide a simple interface for storing arbitrary
records backed by a file which can handle failures and is suitable for
concurrent access.

Specifically, this is a fork of cloudflare/buffer which is a fork of
ashishgandhi's buffer implementation which suits our needs more effectively.
Namely, we updated this to allow for some additional file locking and optional
overwriting of existing records.

At this time, Gravwell nor Cloudflare provides *ANY* guarantees about the
stability of this package.

Please use vendoring to maintain this dependency in your project.
