

`bcftools mpileup -Q 20 -d 100000 -L 100000 -a AD,DP,SP --min-ireads 20 --gap-frac 0.5 --no-BAQ -f /Users/dlu/Documents/genomes/MN908947.3.fa small_test.bam | bcftools call --ploidy 1 -c - | bcftools view -c 1 -Ov > small_test_no_BAQ.vcf`
