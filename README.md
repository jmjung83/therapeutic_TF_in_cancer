## [Publication Title]
## Characterizing therapeutic signatures of tran-scription factors in cancer by incorporating profiles in compound treated cells (by Jinmyung Jung)

## [Environment]
* python: 3.7.3
* Anaconda: 2019.07

## [jupyter notebook files]
### << pre-proccess >>
* preProc1_expression(LINCS):
  * process compound induced gene expressions in LINCS(The Library of Integrated Network-Based Cellular Signatures)
* preProc2_IC50(GDSC):
  * process compound induced cell viabilities in GDSC(Genomics of Drug Sensitivity in Cancer)
  * get common compounds between LINCS and GDSC
* preProc3_FoldChange:
  * get fold-changes of expressions induced by the common compounds of the two databases
* preProc4_TFActivity(TRRUST2)&CompDose:
  * estimate TF activity based on the computed fold-changes and TF target interactions (TRUST2)
* preProc5_Effect&CellSelection:
  * estimate effectiveness of compound treatments and selecte cell lines by the three criteria (A375 and HT29)
### << main analysis >>
* mainAnal1_TFA_distribution:
  * scatter plots of the average and standard deviation of TF activities for each of 627 TFs
* mainAnal2_TT_Scores:
  * compute therapeutic TF (TT) scores and thier FDRs
* mainAnal3_TCP_scores:
  * compute therapeutically correlated TF pair (TCP) scores and thier FDRs
* mainAnal4_TTbox_and_TCPscatter:
  * draw box plots and scatter plots of TF activities for the top TTs and TCPs in A375 cell line
* mainAnal5_sigTT_sigTCP_visualization:
  * draw heatmap of TT scores and TCP scores for the characterized TTs and TCPs in the both cell line
* evaluation 1-2: evaluation
* discussion 1-2: discussion
