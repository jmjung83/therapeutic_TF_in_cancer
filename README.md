## [Publication Title]
## Characterizing therapeutic signatures of tran-scription factors in cancer by incorporating profiles in compound treated cells (by Jinmyung Jung)

## [Environment]
* python: 3.7.3
* Anaconda: 2019.07

## [jupyter notebook files]
### << pre-proccess >>
* preProc1_expression(LINCS).ipynb:
  * process compound induced gene expressions in LINCS(The Library of Integrated Network-Based Cellular Signatures)
* preProc2_IC50(GDSC).ipynb:
  * process compound induced cell viabilities in GDSC(Genomics of Drug Sensitivity in Cancer)
  * get common compounds between LINCS and GDSC
* preProc3_FoldChange.ipynb:
  * get fold-changes of expressions induced by the common compounds of the two databases
* preProc4_TFActivity(TRRUST2)&CompDose.ipynb:
  * estimate TF activity based on the computed fold-changes and TF target interactions (TRUST2)
* preProc5_Effect&CellSelection.ipynb:
  * estimate effectiveness of compound treatments and selecte cell lines by the three criteria (A375 and HT29)
### << main analysis >>
* mainAnal1_TFA_distribution.ipynb:
  * scatter plots of the average and standard deviation of TF activities for each of 627 TFs
* mainAnal2_TT_Scores.ipynb:
  * compute therapeutic TF (TT) scores and thier FDRs
* mainAnal3_TCP_scores.ipynb:
  * compute therapeutically correlated TF pair (TCP) scores and thier FDRs
* mainAnal4_TTbox_and_TCPscatter.ipynb:
  * draw box plots and scatter plots of TF activities for the top TTs and TCPs in A375 cell line
* mainAnal5_sigTT_sigTCP_visualization.ipynb:
  * draw heatmap of TT scores and TCP scores for the characterized TTs and TCPs in the both cell line
### << evaluation >>
* evaluation1_significant_TTs.ipynb:
  * hypergeometric tests for TTs with CRISPR-cas9 (essential genes), TTD (therapeutic targets), TSgene (Tumor suppressors), uniprot (oncogenes and tumor suppressors)
  * draw bar plots presenting their p-values
* evaluation2_enrichmentTest_TFs_in_BTCPs.ipynb:
  * functional enrichment test for TCPs with biologial processes
### << discussion >>
* discussion1_TCPscatter.ipynb:

* discussion 1-2: discussion
