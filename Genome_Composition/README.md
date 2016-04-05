John Davis BIS180L
###Mononucleotide:
####Guess
**C. elegans:** 

* 30% A 
* 30% C 
* 20% G 
* 20% T  

**Arabidopsis:**  

* 15% A
* 30% C
* 15% G
* 40% T

**Drosophila:**  

* 25% A
* 25% C
* 25% G
* 25% T

####Computed Frequencies
Counts made using "grep -c  "^*" (file name)
Calculations made using Mononucleotide Calc Script

**C. elegans:**  

* 32.27% A
* 17.74% C
* 17.68% G
* 32.29% T

**Arabidopis:**  

* 31.99% A
* 17.96% C
* 18.03% G
* 32.00% T

**Drosophila:**  

* 29.18% A
* 20.89% C
* 20.86% G
* 29.06% T

###Dinucleotide

####Predicted Dinucleotide

Using frequencies calculated in mononucleotide experiment
Calculations made using Dinucleotide Prediction Script

**C. elegans:**  

* AA: 10.41%
* AC: 5.72%
* AG: 5.38%
* AT: 10.41%
* CA: 5.72%
* CC: 3.14%
* CG: 2.95%
* CT: 5.72%
* GA: 5.38%
* GC: 2.95%
* GG: 2.78%
* GT: 5.38%
* TA: 10.41%
* TC: 5.72%
* TG: 5.38%
* TT: 10.42%

**Arabidopsis:**  

* AA: 10.23%
* AC: 5.74%
* AG: 5.76%
* AT: 10.23%
* CA: 5.74%
* CC: 3.22%
* CG: 3.23%
* CT: 5.74%
* GA: 5.76%
* GC: 3.23%
* GG: 3.25%
* GT: 5.76%
* TA: 10.23%
* TC: 5.74%
* TG: 5.76%
* TT: 10.24%

**Drosophila:**  

* AA: 8.51%
* AC: 6.09%
* AG: 6.08%
* AT: 8.47%
* CA: 6.09%
* CC: 4.36%
* CG: 4.35%
* CT: 6.07%
* GA: 6.08%
* GC: 4.35%
* GG: 4.35%
* GT: 6.06%
* TA: 8.47%
* TC: 6.07%
* TG: 6.06%
* TT: 8.44%

####Calculated Dinucleotide Frequencies:
Counts made using "grep -c  "^**" (file name)
Calculations made using Dinucleotide Calc Script

**C.elegans:**  

* AA: 13.52%
* AC: 4.84%
* AG: 5.06%
* AT: 8.84%
* CA: 6.19%
* CC: 3.38%
* CG: 3.11%
* CT: 5.03%
* GA: 6.19%
* GC: 3.33%
* GG: 3.32%
* GT: 4.82%
* TA: 6.36%
* TC: 6.18%
* TG: 6.25%
* TT: 13.49%

**Arabidopsis:**  

* AA: 11.55%
* AC: 5.22%
* AG: 5.97%
* AT: 9.23%
* CA: 6.32%
* CC: 3.37%
* CG: 2.33%
* CT: 5.92%
* GA: 6.43%
* GC: 3.00%
* GG: 3.38%
* GT: 5.21%
* TA: 7.69%
* TC: 6.41%
* TG: 6.34%
* TT: 11.55%

**Drosophila:**  

* AA: 10.24%
* AC: 5.26%
* AG: 5.44%
* AT: 8.22%
* CA: 6.74%
* CC: 4.62%
* CG: 4.10%
* CT: 5.42%
* GA: 5.60%
* GC: 5.38%
* GG: 4.59%
* GT: 5.27%
* TA: 6.55%
* TC: 5.58%
* TG: 6.73%
* TT: 10.18%

####Mononucleotide Calc Script

scale = 4
a = 
c = 
g = 
t = 
total = a + c + g + t

fa = a/total
fc = c/total
fg = g/total
ft = t/total

fa
fc
fg
ft
quit

####Dinucleotide Prediction Script

scale = 4
a = 
c = 
g = 
t = 

aa = a*a
ac = a*c
ag = a*g
at = a*t
ca = c*a
cc = c*c
cg = c*g
ct = c*t
ga = g*a
gc = g*c
gg = g*g
gt = g*t
ta = t*a
tc = t*c
tg = t*g
tt = t*t

aa
ac
ag
at
ca
cc
cg
ct
ga
gc
gg
gt
ta
tc
tg
tt

quit

####Dinucleotide Calc Script

scale= 4
aa = 
ac = 
ag = 
at = 
ca = 
cc = 
cg = 
ct = 
ga = 
gc = 
gg = 
gt = 
ta = 
tc = 
tg = 
tt = 
total = aa + ac + ag + at + ca + cc + cg + ct + ga + gc + gg + gt + ta + tc + tg + tt
faa = aa/total
fac = ac/total
fag = ag/total
fat = at/total
fca = ca/total
fcc = cc/total
fcg = cg/total
fct = ct/total
fga = ga/total
fgc = gc/total
fgg = gg/total
fgt = gt/total
fta = ta/total
ftc = tc/total
ftg = tg/total
ftt = tt/total

faa
fac
fag
fat
fca
fcc
fcg
fct
fga
fgc
fgg
fgt
fta
ftc
ftg
ftt

quit

