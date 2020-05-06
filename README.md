# maf_consensus


### SNP with different positions in MAF


#### 1. makes sense to me and is fine for now. Others are indels.
this call in freebayes
```
15	60051998	.	TA	TG	1.94099	.	AB=0.235294;ABP=13.3567;AC=1;AF=0.5;AN=2;AO=4;CIGAR=1M1X;DP=17;DPB=17.5;DPRA=0;EPP=3.0103;EPPR=4.51363;GTI=0;LEN=1;MEANALT=1;MQM=52.25;MQMR=48.0769;NS=1;NUMALT=1;ODDS=0.573581;PAIRED=1;PAIREDR=1;PAO=0.5;PQA=17.5;PQR=17.5;PRO=0.5;QA=124;QR=456;RO=13;RPL=4;RPP=11.6962;RPPR=3.17734;RPR=0;RUN=1;SAF=2;SAP=3.0103;SAR=2;SRF=7;SRP=3.17734;SRR=6;TYPE=snp;technology.illumina=1	GT:DP:RO:QR:AO:QA:GL	0/1:17:13:456:4:124:-5.54789,0,-32.2759
```

translates to 
```
   Hugo_Symbol Entrez_Gene_Id Center NCBI_Build Chromosome Start_Position End_Position Strand  ... gnomAD_AMR_AF gnomAD_ASJ_AF gnomAD_EAS_AF gnomAD_FIN_AF gnomAD_NFE_AF gnomAD_OTH_AF gnomAD_SAS_AF   vcf_pos
41     Unknown              0      .     GRCh37         15       60051999     60051999      +  ...                                                                                                    60051998
```



### indels in MAF:

types: 'indel', 'insertion', 'deletion', 'sequence_alteration'
