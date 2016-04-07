John Davis BIS180L
###Part 1: Getting Organized

1. Created directories using mkdir -p Data/Species/(organism)
2. Move genome data by going to Taxonomy file created prior
3. enter command cp * /home/bis180lstudent/Data/Species/(organism)
4. gunzip files
5. rename files using mv old new

###Part 2: Lab Notebook

Created directory using mkdir -p Lab1_Sequence_Alignment
Create READ.md using touch READ.md
opened READ.md in Remarkable

|Organism|Genome File Size (bits)|Protein File Size (bits)|# of Chromosomes|Size of Genome in bp|# of Protein-coding genes|Average Protein Length|
|---|---|---|---|---|---|---|
|A.thaliana|121183082|20006289|5 chromosomes, 1 chloroplast chromosome 1, mitochondrial chromosome|119667750 bp|35386 proteins| 409.2820 AA|
|C.elegans|102292161|6209267|5 chromosomes, 1 sex chromosome, 1 mitochondrial chromosome|100286401 bp|26769 proteins|445.3565 AA|
|D.melanogaster|172113892|32872415|3 chromosomes, 1 sex chromosome|68736537 bp|30307 proteins|659.2903 AA|

1. Genome and Protein file size found using ls -lF (file)
2. Chromosome count found using grep ">" file
3. Base Pair count found using grep -v ">" file | wc  
    * Returns character count and line count
    * Subtract line count from character count to account for returns
4. Proteins found using grep -c ">" file
5. Average Protein Length found using grep -v ">" file | wc
    * Returns character count and line count
    * Subtract line count from character count to account for returns
    * Divide count by number of Proteins to get average length

###Part 3: Local Alignment

1. used head (file1) to find lines of first protein
2. used sed -n 'start,endp' (file1) > (file2)
3. check by using cat (file2)
4. move the 3 created files to Lab1_Sequence_Alignment
4. used water -at1.fa ce1.fa -gapopen 10 -gapextend 5 -outfile at_ce.water

### Part 4: Random Expectation
1. The shape of the curve is not normal. It is skewed right
2. Most comparions should have a similar shape since higher scores are harder to achieve than lower scores. Low scores will be more common when comparing most proteins.
3. The longer the two proteins are, the less likely that they wil be similar to eachother and the scores will decrease across the whole sequence.
4. Sequences will have different scores based on differences in scoring matrices and gap penalities. The smaller the gap penalty the higher the scores will be. The score will also be higher if the matches are scored higher.
5. Real sequences may have more segments of similiarity since certain sequences and patterns are consserved in nature unlike random sequences where no patterns are conserved.

### Part 5: Alignment Significance
B0213.10 = 499 AA
A.thaliana = 14482855 AA
D.melanogaster = 19981113 AA
Total = 34464467 AA
34464467 differenct AA will be aligned

time water 1kplant 1kfly gapopen-10 gapextend- 5 outfile- speed.test
Time = .805s characters = 153903
Speed = 191183.85characters/second
Predicted align fly proteome to plant proteome = 276.59 seconds
Real time to align B0213.10 to A.thaliana = 1 Min 47 Secs
Real time to align B0213.10 to D.melanogaster = 3 Min 19 Secs

B0213.10 is a cytochrome protein
best match of B0213.10 with D.melanogaster = FBpp0074380

* Cyp18a1-PB
* 1: B0213.10
 2: FBpp0074380
 Matrix: EBLOSUM62
 Gap_penalty: 10.0
 Extend_penalty: 5.0
 Length: 506
 Identity:     133/506 (26.3%)
 Similarity:   227/506 (44.9%)
 Gaps:          29/506 ( 5.7%)
 Score: 333.0

best match of B0213.10 with A.thaliana = AT2G23190.1

* cytochrome P450, family 81, subfamily D, polypeptide 7
* 1: B0213.10
 2: AT2G23190.1
 Matrix: EBLOSUM62
 Gap_penalty: 10.0
 Extend_penalty: 5.0
 Length: 493
 Identity:     139/493 (28.2%)
 Similarity:   228/493 (46.2%)
 Gaps:          30/493 ( 6.1%)
 Score: 337.0

Highest score from a random alignment = 78
Score is statistically significant
Score is biologically siginificant since all 3 proteins are fount to be cytochrome P450 proteins