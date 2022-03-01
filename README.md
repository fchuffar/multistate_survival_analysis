# multistate_survival_analysis
A set of scripts an vignettes dealing with multistate survival analysis, including TCGA dataset and a Markovian process simulator.


## In practice

```
# test definition and implementation of transitions
echo 'rmarkdown::render("vignettes/01_stress_test.Rmd")' | Rscript -

# launch msm and mstate models
echo 'rmarkdown::render("vignettes/02_data_msm_updated.Rmd")' | Rscript -

# screen censor_param
echo 'rmarkdown::render("vignettes/03_censor_effect.Rmd")' | Rscript -
echo 'rmarkdown::render("vignettes/03_censor_effect_covar.Rmd")' | Rscript -

# all models on BRCA cancer (then all cancers)
echo 'rmarkdown::render("vignettes/04_full_kc_stage_study.Rmd")' | Rscript -
echo 'rmarkdown::render("vignettes/04_full_kc_stage_study_synthesis.Rmd")' | Rscript -

# exploring parameters
echo 'rmarkdown::render("vignettes/05_sensitivity_analysis.Rmd")' | Rscript -
```