## [Publication Title]
## Characterizing therapeutic signatures of tran-scription factors in cancer by incorporating profiles in compound treated cells (Jinmyung Jung)

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

* mainAnal 1-5: main analysis
* evaluation 1-2: evaluation
* discussion 1-2: discussion
