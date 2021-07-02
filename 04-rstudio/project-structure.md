# Project Folder Structure

For a new project, I use the following folder structure:

- **Project Directory**
  - .Rproj (R Project File)
  - *0_data*
     - dataset1.csv
     - dataset2.csv
  - *1_script*
    - *0_functions*
      - myfunction.R
    - 1_load_data.R
    - 2_preprare_data.R
    - 3_core.R
    - 4_output.R
    - 5_graphs.R
  - *2_output*
    - regression_output.csv
    - plot.png
  - *3_docs*
    - manual.Rmd
    
## How to use it

* The `data` folder consists of raw data files, typically in .csv or .xlsx format. Once a file has been put into the data folder, it should not be modified anymore. Think of it as a read-only folder.
* The `script` folder contains all the code for this project. The numbers indicate the order of execution. There may be an additional subfolder for smaller functions which are sourced by the script files. 
* The `output` folder contains any output that has been generated by the script files. For example, plots, tables or .csv files.
* The `docs` folder typically contains a single R Markdown file with a brief explanation on the data and on how the scripts work. 
* I try to leave my folder structure as flat as possible with two layers of subfolders within the project folder at maximum. This is a trade-off between being economical on clicks and preserving a high degree of structuredness. 
* My working directory is set to the project folder, the corresponding subfolders and -files are addressed using relative paths. This way, the whole project folder can easily be moved to another location or computer. 