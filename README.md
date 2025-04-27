# M1M1PAS
This is analysis code for the article: Ermolova, M., Kozak, G., Belardinelli, P., & Ziemann, U. (2025). Plasticity of interhemispheric motor cortex connectivity induced by brain state-dependent cortico-cortical paired-associative stimulation. bioRxiv, 2025-04.

Dataset used in the analysis: Ermolova, M., Kozak, G., Belardinelli, P., & Ziemann, U. (2025). Dataset for the article "Plasticity of interhemispheric motor cortex connectivity induced by brain state-dependent cortico-cortical paired-associative stimulation" [Data set]. Zenodo. https://doi.org/10.5281/zenodo.15126575

File description:
"1 - preprocessing.m" code for EEG preprocessing.
  "1 - auto_preproc.m" automatic preprocessing of EEG data.
  "2 - check_ica_comps.m" manual selection of artifactual ICA components.
  "3 - truncate_1_run.m" truncates the first 10-min EEG recording in each session to 5 mins to match the rest of the recordings in the session.
"2 - source" code for source reconstruction.
  "1 - calculate_leadfield.m" compute leadfield for each subject and each session
  "2 - beamformer.m" reconstruct source signals from right and left sensorimotor cortex
"3 - fc" code for functional connectivity and phase lag analysis.
  "connectivity_calc.ipynb" functional connectivity analysis
  "phase_lags_calc.ipynb" phase lag analysis
  "phase_lags_vis.ipynb" visualization of phase lags
"4 - stats" code for statistical analysis.
  "SIHI_stats" statistical analysis of SIHI
  "FC_stats" statistical analysis of functional connectivity
  "Phl_stats" statistical analysis of phase lag distribution
  "MEP_conditioning_stats" statistical analysis of MEP amplitudes from the conditioning pulses (right FDI)
  "MEP_conditioned_stats" statistical analysis of MEP amplitudes from the conditioned pulses (left FDI)
  "MEP_unconditioned_stats" statistical analysis of MEP amplitudes from the unconditioned pulses (left FDI)
