# GeneSymbolUniform_Rtoolkit
An R script that helps uniform gene symbols of different single-cell RNA sequencing data

Welcome to use Gene Symbol Uniform R toolkit!

# Steps
0. Please ensure that the dependencies are properly installed: Seurat, stringr, dplyr. The number in parentheses are recomended version.    
  
1. According to the limitation of github, please unzip "GeneSymbolRef_SelectAll_upd0731.csv.zip" first. Keep the names of other files in this folder unchanged.  
  
2. Change the working directory to this directory:  
`cd path_to_this_dir`  
  
    Then execute the following command:  
`Rscript Rtoolkit_GeneSymbolUniform.R [query_path] [output_dir]`  
  
    where:  
    query_path: The absolute path of query dataset to be processed (txt or csv).    
    output_dir: The absolute path to receive output files.    
  
3. There would be some notices if one processing stage is finished.  
  
5. When finished, the toolkit would write down two csv files in the "output_dir":  
UniformedExpression.csv，the expression matrix with uniformed gene symbol list (43878 HGNC genes). The number of cells are similar to that of Seurat object.  
ModificationReport.csv，The records for the modified gene symbols. The gene list is the same as input Seurat object.  


# Acknowledgement
Many thanks to **Qiuchen Meng** and **Ziheng Zou** for their efforts in building and testing this toolkit. We would also thank **Yixin Chen**, **Minsheng Hao** and **Sijie Chen** for their suggestions in optimizing this toolkit.

# Contact
Please contact Jiaqi Li at li-jq18@mails.tsinghua.edu.cn if you have any question or suggestions while using this toolkit.
