# **Copy number variation detection for next generation sequencing data using TV-L1**

## **Input:**

- Sorted BAM files of the tumour and control (matched normal) samples

- Duplicate reads must be removed from BAM files

## **Output:**

- Copy number variation segments


## **Method:**

## **Preprocessing**
<!--- considering only exonic reagions-->
{% comment %} considering only exonic reagions {% endcomment %}
- samtools view -bh -L exom.bed tumor.bam > tumor_filteredexon.bam
- samtools view -bh -L exom.bed normal.bam > control_filteredexon.bam



## **Segmentation**
