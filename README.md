# Supplementary Material for Doubly robust estimation and sensitivity analysis for marginal structural quantile models ([arXiv preprint arXiv:2210.04100](https://arxiv.org/abs/2210.04100))

The Web appendix is available at "MSQM_Supplementary_Material.pdf".

The zip file "Simulation_Code_0124.zip" provides R code for repeating the simulation results in Section 6. In what follows, I provide the steps to run the simulation code.

## Below is code for the main simulation study (Section 6.1):

* Subfolder "Part_I" (code for bias, standard error, and Wald-type confidence interval based on the derived asymptotic variance)
  * folder "Scenario_I"
    * folder "MSQM25": Percent bias, standard error, and Wald-type CI in Web Table S3
    * folder "MSQM50": Percent bias, standard error, and Wald-type CI in Table 2
    * folder "MSQM75": Percent bias, standard error, and Wald-type CI in Web Table S2
  * folder "Scenario_II"
    * folder "MSQM25": Percent bias, standard error, and Wald-type CI in Web Table S6
    * folder "MSQM50": Percent bias, standard error, and Wald-type CI in Web Table S4
    * folder "MSQM75": Percent bias, standard error, and Wald-type CI in Web Table S5

* Subfolder Part_II (code for the bootstrap confidence interval)
  * folder "Scenario_I"
    * folder "MSQM25": Bootstrap CI in Web Table S3
    * folder "MSQM50": Bootstrap CI in Table 2
    * folder "MSQM75": Bootstrap CI in Web Table S2
  * folder "Scenario_II"
    * folder "MSQM25": Bootstrap CI in Web Table S6
    * folder "MSQM50": Bootstrap CI in Web Table S5
    * folder "MSQM75": Bootstrap CI in Web Table S4


For each folder, first implement the "main.slurm" file to generate the crude simulation results and then implement the "Gen_table.Rmd" to generate the latex table based on the crude simulation results.

## Below is code for the sensitivity analysis simulation (Section 6.2):

* Subfolder Part_III (code for sensitivity analysis simulation)
  * folder "SA_Correct": code for lower panels of Web Tables S7--S9
  * folder "SA_Wrong": code for upper panels of Web Tables S7--S9

For each folder, implement "main1.slurm", "main2.slurm", and "main3.slurm" file for crude simulation results for Web Tables S7--S9, then implement the "Gen_table.R" to generate the latex table based on the crude simulation results.
