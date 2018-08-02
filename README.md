# Prepositional Phrase (PP) Idioms
Analyzing PP idioms in the Oxford Dictionary of English (ODE)

Each PP idiom consists of a multiple word expression (MWE), i.e., containing at least two words. Idioms were obtained from ODE entries either beginning or ending with a preposition from the Pattern Dictionary of English Prepositions (PDEP, <http://www.clres.com/db/TPPEditor.html>). This repository contains description of the analysis and files supporting the analysis.

Files
-----
- ACKNOWLEDGMENTS.md: Contributors inspiring this research

Initial Data
------------
- pp-begin.txt: 2484 entries beginning with a PDEP preposition (potentially idiomatic), with senses, a part of speech, and a definition
- pp-final.txt: 2785 entries ending with a PDEP preposition (potentially idiomatic), with senses, a part of speech, and a definition

Data for Beginning PP Idioms
----------------------------
- pp-beg-cats.tsv: Categories of beginning phrases, containing a line number, the PDEP preposition, a code, and the line from pp-begin.txt (in a tab-separated file)
- pp-beg-stats.tsv: Counts for each of the 63 beginning prepositions, with the name and the number of instances, unique MWEs, and distinct senses
- pp-idioms-good-a.txt: Lines of the 1891 phrases initially judged as valid PP idioms (categorized a "1" in pp-beg-cats.tsv)
- pp-idioms-good.txt: The first three columns of the previous file (the line number, the PDEP preposition, and the idiom), enabling to identify the 1561 unique idioms

Data for Ending PP Idioms
-------------------------
- pp-fin-cats.tsv: Categories of ending phrases, containing a line number, the PDEP preposition, a code, and the line from pp-final.txt (in a tab-separated file)
- pp-fin-stats.tsv: Counts for each of the 66 ending prepositions, with the name and the number of instances in pp-final.txt
- pp-final-in.txt: Lines of the 182 ending phrases corresponding to phrases already in PDEP
- pp-final-poss.txt: Lines of the 146 ending phrases corresponding to phrases that possibly need to be added in PDEP

Data for PP Idioms in Streusle Corpus
-------------------------------------
- Streusle-4.0.PPIdioms.parse: The 170 lines from the Streusle parses that have a LEXLEMMA PP (13th column), indicating that the annotators felt the presence of PP idiom
- Streusle-4.0.PPIdioms-sorted.tsv: Parsed lines from above sorting the PP idioms
- Streusle-4.0.PPIdioms-unique.tsv: List of the 95 unique idioms in these lines
- Streusle-4.0.PPIdioms-stats.tsv: Statistics about the 95 idioms: a count of their frequency, whether having different role and function supersenses, whether found in a dictionary, and comments about the idiom if not found in the dictionary
- Streusle-4.0.PPIdioms-analysis.tsv: Summary analysis for each idiom whether found and analysis in two dictionaries
