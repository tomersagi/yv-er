# Yad Vashem Entity Resolution Project Public Datasets
This repository contains datasets made public by the [Yad Vashem](http://www.yadvashem.org) foundation and [Hewlett Packard Labs](http://www.labs.hpe.com/israel/) to be used for Entity Resolution research. 
Data is provided as-is with no guarantees as to its quality and other properties. 

## Repository Content
The repository contains two datasets. 

1. A homogeneous dataset comprised of all records having **Italy** as the victim's place of residence. The Dataset contains 9499 records (italy_records.csv) and 12,749 tagged record pairs (italy_pairs.csv). 
2. A stratified random sample of the full Yad Vashem dataset. Six geographical regions where selected from the dataset, each representing a different pre-holocaust Jewish community. Differences were either cultural-linguistic or in the progression of persecution during WWII itself. This dataset contains 100,000 records. 

## Record File Structure
Each row in the file corresponds to a record. Fields are delimited by semi-colons. The first field in a row is the unique record-id in the Yad Vashem Names database. The rest are a bag of items prefixed by the item type. Item-types and their prefixes are described in the following table:

Prefix | Item Type | Values
------------ | ------------- | -------------
F | First Name | Disambiguated first name
L | Last Name / Surname | Disambiguated surname
S | Source | Name of submission and submission year for pages of testimony, list name for lists
G | Gender | 0-Male, 1-Female
B1 | Birth Day | Calendar day of birth
B2 | Birth Month | Calendar month of birth
B3 | Birth Year | Calendar year of birth
D1 | Birth Day | Calendar day of death
D2 | Birth Month | Calendar month of death
D3 | Birth Year | Calendar year of death
BP1 | Birth City | Disambiguated city of birth
BP2 | Birth County | Disambiguated county of birth
BP3 | Birth Region | Disambiguated region of birth
BP4 | Birth Country | Disambiguated country of birth
PP1 | Permanent residence City | Disambiguated city of Permanent residence
PP2 | Permanent residence County | Disambiguated county of Permanent residence
PP3 | Permanent residence Region | Disambiguated region of Permanent residence
PP4 | Permanent residence Country | Disambiguated country of Permanent residence
WP1 | War-time residence City | Disambiguated city of War-time residence or Camp name
WP2 | War-time residence County | Disambiguated county of War-time residence
WP3 | War-time residence Region | Disambiguated region of War-time residence
WP4 | War-time residence Country | Disambiguated country of War-time residence
DP1 | Death City | Disambiguated city of death or camp name
DP2 | Death County | Disambiguated county of death
DP3 | Death Region | Disambiguated region of death or camp type
DP4 | Death Country | Disambiguated country of death
FF | Father's First Name | Disambiguated father's first name
MF | Mother's First Name | Disambiguated mother's first name
SN | Spouse's First Name | Disambiguated spouse's first name
MN | Maiden Name | Disambiguated maiden surname
MMN | Mother's Maiden Name | Disambiguated mother's maiden surname
PR | Profession code | Code referring to the profession table (supplied separately)

## Record Pairs File Structure
The pairs were tagged by Yad Vashem archival experts with one of the following tags: {1-Yes, 2-Probably Yes, 3-Maybe, 4-Probably No, 5-No}. The tagged pairs are admittedly a subset of the matching pairs in the dataset. We are continuously improving it and adding to the known true matches. Researchers wishing to contribute additional pairs for review by Yad Vashem are invited to do so by submitting an issue. We will make a best-effort attempt at reviewing these suggestions. 