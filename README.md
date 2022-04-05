# match-gene-ID-from-different-database
許多資料庫，整理GENE ID可能沒有統一一種版本。
策略: 先配對大多數的基因，並從ENSP轉換成HGNC，再轉換成ENSG。篩出沒有配對到的，地毯式搜尋其他版本的ensembl，直到找到其對應的HGNC，再轉成ENSG


範例: 
TCGA gene id is provided by ENSG, but another database is provided by ENSP.
We are not sure those version result in hard to match and merge the information from two resource.
The gene id from TCGA is ENCOD v36, however we are not sure that which ensembl version of ENSP list is  from COMPARTMENTS database.
