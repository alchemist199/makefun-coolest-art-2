# coolest-art-01 entry

A cyberpunk samurai stands on a rain-soaked neon rooftop at night, katana
drawn, above a holographic city skyline. The artwork ships in the repo as
`entry.png` — a 896x597 PNG of 960,896 bytes, inside the 1 MiB and
1024x1024 limits. `main.py` checks the image and copies it unchanged to
`/output/`.

Two runs produce byte-identical output. Standard library only, no network.

Revision 2: the program now also accepts a JPEG (`entry.jpg`) when no PNG
is present, and verifies the file is complete — a PNG must end with its
IEND chunk, a JPEG with its EOI marker — instead of trusting the header
alone.
