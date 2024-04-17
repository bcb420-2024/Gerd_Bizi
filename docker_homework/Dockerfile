# inherit base Docker image
FROM risserlin/bcb420-base-image:winter2024

# Install R packages
RUN R -e 'install.packages("pheatmap", repos = "http://cran.us.r-project.org")'
RUN R -e 'if (!requireNamespace("BiocManager", quietly = TRUE)) install.packages("BiocManager", repos = "http://cran.us.r-project.org"); BiocManager::install(c("DESeq2", "enrichplot"))'