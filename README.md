# RSEA_data (staging)

Staging area for the raw measurement data of the RSEA paper.


awdata-v1 (draft release) holds the packed archive split into zenodo.zip.partNN
(15 parts, 150 MB each) because a single 2 GB upload from this network is not viable.

.github/workflows/to-zenodo.yml downloads the parts on a GitHub runner, concatenates them
back into one zenodo.zip (sha256 verified), and uploads that **single file** to the Zenodo
draft. Once Zenodo has the file this repository/release can be deleted.
