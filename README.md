# BOLD BLAST on Hydra walkthrough

- Web BLAST and BOLD ID Engine
    [Screenshots](web_blast/README.md)
    - **Pros:** no setup necessary
    - **Cons:** not very scalable beyond a handful of sequences
- BLAST against NCBI db on Hydra
    - Show job file, and stats on resource usage
    - **Pros:** Set it and forget it. Pretty comprehensive, if you want to filter results afterwards.
    - **Cons:** Takes a long time, lots of memory
- BLAST against custom COI db
    - Fast enough to show interactively, but also include job file and stats
    - **Pros:** Does have taxonomy included
    - **Cons:** Custom COI db is complicated to build, not all represented
- BLAST against BOLD db
    - Fast enough to show interactively, but also include job file and stats
    - **Pros:** Probably more comprehensive than NCBI, since many BOLD records do not get published.
    - **Cons:** Need to link taxonomy as an extra step -- but also pulls in geographic and specimen data.

## Next steps
- BLAST alternatives (like https://github.com/bbuchfink/diamond or https://github.com/torognes/vsearch)
- Standardizing database updates
- Non-COI markers
