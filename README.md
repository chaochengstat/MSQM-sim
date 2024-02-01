We provide R codes for repeating the simulation results in Section 6 of **Doubly robust estimation and sensitivity analysis for marginal structural quantile models**. 

Below is code for the main simulation study (Section 6.1):

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


For each subfolder, first implement the "main.slurm" file to generate the crude simulation results and then implement the "Gen_table.Rmd" to generate the latex table based on the crude simulation results.
