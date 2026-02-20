# CUNY Libraries — Indication and Normalization Rules

Configuration rules for Ex Libris Alma and Primo VE used across CUNY libraries, maintained by the CUNY Office of Library Services (OLS).

## Overview

This repository houses indication rules and normalization rules applied in the Alma library management system. These rules shape how bibliographic and holdings metadata is evaluated, transformed, and surfaced in Primo VE discovery.

## Repository Structure
```
rules/
├── indication rules/                  # Rules that evaluate conditions to filter sets of records
├── normalization (discovery) rules/   # Rules applied to externally loaded records for Primo VE discovery
└── normalization rules/               # Rules applied to bibliographic metadata managed within Alma
```

## Rule Types

**Indication Rules** evaluate conditions against MARC or other metadata fields to filter sets of records — for example, identifying records that meet specific criteria so they can be targeted for bulk processing or review.

**Normalization Rules** transform or enrich bibliographic metadata managed within Alma. Written in Drool syntax or XSL, they can add, remove, modify, or reorder fields and subfields. They may be applied when records are saved in the Metadata Editor, imported via import profiles, or processed in bulk through normalization jobs.

**Normalization (Discovery) Rules** are a distinct rule type used specifically for records loaded into Primo VE from external sources that are not managed in Alma — such as Dublin Core or generic XML records. Rather than operating on MARC fields directly, these rules use a separate syntax to map source metadata to Primo VE discovery fields to control how records display and are indexed in Primo VE.

## Related Resources

> **Note:** The Ex Libris Knowledge Center is under construction as of February 2026. Some links below may not work.

- [Alma > Metadata Management > Working with Rules > Working with Normalization Rules](https://knowledge.exlibrisgroup.com/Alma/Product_Documentation/010Alma_Online_Help_(English)/Metadata_Management/016Working_with_Rules/020Working_with_Normalization_Rules)
- [Alma Normalization Rule Examples – Ex Libris Developer Network](https://developers.exlibrisgroup.com/blog/alma-normalization-rule-examples/)
- [Primo VE > Loading Records from External Sources into Primo VE > Configuring Normalization Rules for External Resources](https://knowledge.exlibrisgroup.com/Primo/Product_Documentation/020Primo_VE/Primo_VE_(English)/100Loading_Records_from_External_Sources_into_Primo_VE/Configuring_Normalization_Rules_for_External_Resources_(Primo_VE))

## Maintainers

Maintained by CUNY Office of Library Services. For questions, [contact the OLS systems team](mailto:support@cuny-ols.libanswers.com).
