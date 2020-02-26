table = {'ATA':'I', 'ATC':'I', 'ATT':'I',
'ATG':'M', 'ACA':'T', 'ACC':'T', 'ACG':'T',
'ACT':'T', 'AAC':'N', 'AAT':'N', 'AAA':'K',
'AAG':'K', 'AGC':'S', 'AGT':'S', 'AGA':'R',
'AGG':'R','CTA':'L', 'CTC':'L', 'CTG':'L',
'CTT':'L', 'CCA':'P', 'CCC':'P', 'CCG':'P',
'CCT':'P', 'CAC':'H', 'CAT':'H', 'CAA':'Q', 
'CAG':'Q', 'CGA':'R', 'CGC':'R', 'CGG':'R',
'CGT':'R', 'GTA':'V', 'GTC':'V', 'GTG':'V',
'GTT':'V', 'GCA':'A', 'GCC':'A', 'GCG':'A',
'GCT':'A', 'GAC':'D', 'GAT':'D', 'GAA':'E',
'GAG':'E', 'GGA':'G', 'GGC':'G', 'GGG':'G',
'GGT':'G', 'TCA':'S', 'TCC':'S', 'TCG':'S',
'TCT':'S', 'TTC':'F', 'TTT':'F', 'TTA':'L',
'TTG':'L', 'TAC':'Y', 'TAT':'Y', 'TAA':'_',
'TAG':'_', 'TGC':'C', 'TGT':'C', 'TGA':'_',
'TGG':'W'}
m=input('enter sequence= ')
print('your provided sequence is=',m)
aminoacidsequence=' '
for i in range(0,len(m),3):
    codon=m[i :i+3]
    b=table[codon]
    aminoacidsequence=aminoacidsequence +b + '_'
c=len(aminoacidsequence) 
print('aminoacidsequence is=',aminoacidsequence)
d=input('Enter the Short name of a amino acid=')
e=aminoacidsequence.count(d)
print('percentage of amino acid is=',(e/c)*100)
