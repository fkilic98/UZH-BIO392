#Variant formats

## Variant Call Format (VCF9
    ### Three main sections
    1. Meta Information Lines - Multiple lines prefixed by double pound symbols (##).
    Describes the format and content of that specific VCF file.
    2. Header Line - Single line prefixed with a one pound symbol (#).
CHROM | POS | ID | REF | ALT | QUAL | FILTER | INFO
----- | --- | -- | --- | --- | ---- | ------ | ----

Content cell 1 | Content cell 2
Content column 1 | Content column 2

    3. Data Lines - Remainder of the file with 1 position per line.