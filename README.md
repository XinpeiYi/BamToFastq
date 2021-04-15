# BamToFastq

https://gatk.broadinstitute.org/hc/en-us/articles/360036485372-SamToFastq-Picard-

java -jar picard.jar SamToFastq \
     I=input.bam \
     FASTQ=output.fastq

https://www.jianshu.com/p/901c1cdf8a45

samtools sort -n Aligned.sortedByCoord.out.bam -o sort.bam

java -Xmx2g -jar /data/xyi/software/picard/picard.jar SamToFastq \
I=/data/xyi/CPTACProject/UCEC/FusionIdentification/TCGA/RNASeq/3c6dc2f5-8da9-459f-b03f-79200820cabe/18c52fe6-5cb0-4e59-91a2-e9845c0527c6_gdc_realn_rehead.bam \
FASTQ=test_1.fastq.gz \
SECOND_END_FASTQ=test_2.fastq.gz \
UNPAIRED_FASTQ=test_0.fastq.gz
