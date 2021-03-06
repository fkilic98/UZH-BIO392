# Exploration of variant annotation formats

## Which "genomic" variant formats exist & what are their use cases?
* ISCN (**I**nternational **S**ystem for Human **C**ytogenetic **N**omenclature)
> ISCN is a book about the standard nomenclature thaat describes any chromosomal abberations. The genomic rearrangement are identified by techniques liek karyotyping, FISH, SKY, genomic microarray, various region specific assay and DNA sequencing. The nomeclature is used for molecular cytogenetics.
* HGVS (**H**uman **G**enome **V**ariation **S**ociety)
> This society provides an overview about several [databases](https://www.hgvs.org/content/databases-tools) for various variations/mutations. The website is a good starting point for gene variation research.
> HGVS offers also a [Sequence Variant Nomenclature](https://varnomen.hgvs.org/). The nomenclature gives an overview over the sequence variant description for human DNA, RNA, protein, etc. Be aware of the reference that the variant relates to. Such a standardized description of variants makes the international cooperation easier.
* VCF (**V**ariant **C**all **F**ormat)
> VCF is a file format and the standard for human genomic variant storage/representation. Variants such as insertions/deletions, single nucleotide, copy number and structural variants. It can store the results of a single or multiple interpretations of genome sequencing datasets. The variations are always in comparison to a reference genome. The VCF is good for short or common and not rare or structure variants.
* GA4GH Variation Representation Specification 
> The **G**lobal **A**lliance **for** **G**enomics and **H**ealth developed a Variant Representation Specification (VRS) to faciliate sharing of genetic information and improve international collaboration. The Specification covers many classed of genetic variations. VRS uses a terminology and information model, machine readable schema (JSON Schema), conventions that promore reliable data sharing, globally unique identifiers and a Python implementation. 

## Genomic coordinate systems
* 0 or 1-based
> 
* "interbase"

-------------------------------------------------------------------------------------------------

# Exploration of different file formats

## Which genomic file formats exist & what are their use cases?
*[This page](https://genome.ucsc.edu/FAQ/FAQformat.html) give a good overview about various data file formats*

* SAM (**S**equence **A**lignment **M**ap)
> SAM is a generic format for storing large nucelotide sequence alignments. It is flexible, simple and compact. Many NGS and analysis tools work with SAM.
* BAM (**B**inary **A**lignment **M**ap)
> BAM files are binary representation of the SAM format i.e. a compact and indexable representation of nucleotide sequence alignments. Many NGS and analysis tools work with BAM. For custom track display, it's advantegous that only the portions of the files needed to display a particular region are transferred to UCSC. 
* CRAM
> CRAM files are similar to BAM files but give a compressed repesentation of the alignment. This compression is driven by the reference the sequence data is aligned to. This file format was designed to reduce the disk foot print of alignment data. CRAM files are smaller than BAM files by taking advantage of an additional external "refernce sequence* file. This reference file is needed to compress and decompress the read information. 
* VCF (**V**ariant **C**all **F**ormat)
> VCF is a flexible and extendable file format and the standard for human genomic variant storage/representation. The format has a tab delimiter.  It can store the results of a single or multiple interpretations of genome sequencing datasets. The variations are always in comparison to a reference genome. 
* FASTA
> FASTA is a text format for linear annotation of single-letter nucleotides or amino acid codes. The format is readable and not optimized for size. FASTA starts always with a definition line. After '>' follows the identifier of the sequence (mostly with a unique SeqID) and a (optimal) description. There should be no space between '>' and the forst letter of identifier. All lines of text should be shorter than 80 chararacters in lentgh. Blank lines are not allowed in the middle of FASTA input.
>
> An example sequence in FASTA format:
>
>         >gi|129295|sp|P01013|OVAX_CHICK GENE X PROTEIN (OVALBUMIN-RELATED)
>	        QIKDLLVSSSTDLDTTLVLVNAIYFKGMWKTAFNAEDTREMPFHVTKQESKPVQMMCMNNSFNVATLPAE
>        	KMKILELPFASGDLSMLVLLPDEVSDLERIEKTINFEKLTEWTNPNTMEKRRVKVYLPQMKIEEKYNLTS
>	        VLMALGMTDLFIPSANLTGISSAESLKISQAVHGAFMELSEDGIEMAGSTGVIEDIKHSPESEQFRADHP
>	        FLFLIKHNPTNTIVYFGRYWSP
* MPEG-G
> The **M**oving **P**icture **E**xperts **G**roup produced a open standard to compress, store, transmit and process sequencing data (MPEG-G). MPEG-G solves the problem of efficient and cost-effective handling of genomic data. It provides functionalities such as native support for selective access, data protection mechanisms, flexible storage and streaming capabilities. This makes possible a real-time streaming of data from a sequencing machine to remote analysis centers during the sequencing and alignment processes. The MPEG-G standard is composed by five parts: Transport and Storage of genomic information, Coding of genomic information, Metadata and APIs, Reference Software and Conformance. 

--------------------------------------------------------------------------------------------------

# Estimate Storage Requirements for 1000 Genomes

## How much computer storage is required for 1000 Genomes?
* WES & WGS
> 
* Different file formats
  * SAM
  >
  * BAM
  >
  * CRAM
  >
  * VCF
  >
  * FASTA
  >
* Associated costs
  * Cost factors
  >
  * Raw Storage costs
  >
