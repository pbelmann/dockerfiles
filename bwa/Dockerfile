FROM quay.io/biocontainers/bwa:0.7.17--h5bf99c6_8 AS bwa
FROM quay.io/biocontainers/samtools:0.1.19--h270b39a_9 AS samtools

FROM ubuntu:20.04
COPY --from=samtools /usr/local/bin/samtools /usr/local/bin 
COPY --from=bwa /usr/local/bin/bwa /usr/local/bin 
