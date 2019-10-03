# PanelAppGE
Command line tool to nicely print Genomics England Panel App results.

Pipe in single gene or line delimited list of genes to program (case insensitive)

Use -f or --fields to specify comma delimited list of fields to report instead of defaults of 
[penetrance, mode_of_pathogenicity, evidence, phenotypes, mode_of_origin]. 
Do **not** put a space between commas for field argument.


Example usage with default fields:
>python3 ppa.py -g GFI1

Example usage with custom fields:
>cat gene_list.txt | while read line; do python ppa.py -f publications,evidence -g $line; done

