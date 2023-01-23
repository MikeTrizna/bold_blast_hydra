(on login node -- memory issues when running on interactive or compute)

`makeblastdb -in bold_coi_2023_01_20.fasta -parse_seqids -out /scratch/dbs/blast/bold/bold_blast_2023_01_20 -title "bold_blast_2023_01_20" -dbtype nucl`

Output

``` 
Building a new DB, current time: 01/23/2023 13:02:51
New DB name:   /scratch/dbs/blast/bold/bold_blast_2023_01_20
New DB title:  bold_blast_2023_01_20
Sequence type: Nucleotide
Keep MBits: T
Maximum file size: 1000000000B
FASTA-Reader: Ignoring invalid residues at position(s): On line 1242750: 2
FASTA-Reader: Ignoring invalid residues at position(s): On line 1242752: 2
FASTA-Reader: Ignoring invalid residues at position(s): On line 3489264: 660
FASTA-Reader: Ignoring invalid residues at position(s): On line 5327268: 1535
FASTA-Reader: Ignoring invalid residues at position(s): On line 10466484: 27
FASTA-Reader: Ignoring invalid residues at position(s): On line 15264630: 1-2
FASTA-Reader: Ignoring invalid residues at position(s): On line 15991922: 2
Adding sequences from FASTA; added 8193116 sequences in 224.836 seconds.
```

Getting BLAST db info:

`blastdbcmd -db /scratch/dbs/blast/bold/bold_blast_2023_01_20 -info`

Output

```
Database: bold_blast_2023_01_20
        8,193,116 sequences; 5,170,740,927 total bases

Date: Jan 23, 2023  1:10 PM     Longest sequence: 9,299 bases

BLASTDB Version: 5

Volumes:
        /scratch/dbs/blast/bold/bold_blast_2023_01_20.00
        /scratch/dbs/blast/bold/bold_blast_2023_01_20.01
```
