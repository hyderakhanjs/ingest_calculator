# ingest_calculator

- Download the **_diag.ipynb_** file and open it in colab.research.google.com
- It requires two files **indices.json** and **ilm_polices.json** from the diagnostic tar
- Make sure the files are uploaded to your google drive. You can connect your google drive to colab.research.google.com
- Once connected the files should show up in the left nav bar and you should be able to copy / paste the path to each file in the code.
- This script will also produce two files, merged_index.csv and merged_ilm.csv . You need to provide a path in your code on where to drop these files
- Keep in mind that the daily ingest number for each ILM policy is the storage on disk. You will have to manually calculate the raw ingest size using a compression factor based on your use case
- The calculations are only done for the primary shards and do not include data for replicas.
- Run the first notebook fragment. It should take longer to run. Once completed, run the second notebook fragment which should be much quicker
