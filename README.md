# metagratingModCMAES

Metasurfaces-based immersed diffraction grating optimized using mod-CMA-ES

---

## Overview

This project uses a modified Covariance Matrix Adaptation Evolution Strategy (mod-CMA-ES) to design and optimize immersed diffraction gratings in metasurfaces. The goal is to find grating geometries that maximize performance metrics (e.g. diffraction efficiency, spectral response) under given constraints.

---

## Structure

| Directory / File | Description |
|---|---|
| `CMA_ES_run.ipynb` | Main notebook that ran the mod-CMA ES optimization. |
| `baselineResults_SV_SWIR3/` | Contains baseline results from the Sentinel-5 SWIR-3 blazed grating. |
| `data_loc_CMAES/data_f1121_metagrating/` | The logger that saved the evolution of the FOM and DOF for each iterations of the optimization. |
| `simulation_files_lumerical/` | Lumerical files for each data point ran and saved with results. They are used to extract results. |
| `cmaes_results.npz` | Stored results from the CMA-ES runs. |
| `CMA_ES_run_result.txt` | Stored results from the CMA-ES runs. |
| `cmaesbestPoint_analysis_plots.ipynb` | Notebook for analyzing and plotting the results from the best candidate from CMA-ES. |
| `finerMeshConfirm_cmaes_bestPoint.ipynb` | Notebook to verify the best solution from the optimization run with a finer mesh. |
| `man_tol_study.ipynb` | Notebook for studying the effect of tolerance parameter (“man tol” = manual tolerance) on performance. |
| `sawtooth_grating_data_opRange.npz` | Data for sawtooth grating performance over a range of operating conditions. |
| `visualization.fsp` | A Lumerical file for visualization of the best design. |

---

## Requirements / Dependencies

- Python (version X.Y or higher)  
- Main Packages required: `numpy`, `scipy`, `matplotlib`, `modCMA` 
- Lumerical simulation tools (if running `.fsp` files)  
- Jupyter notebook environment  

---

## License

MIT

---

## Citation

If you use this repository in your research, please cite it as:

```bibtex
@misc{patel2025_metagratingModCMAES,
  author       = {Patel, Dhwanil and de Nobel, Jacob and Kohlhaas, Ralf},
  title        = {metagratingModCMAES},
  year         = {2025},
  publisher    = {GitHub},
  howpublished = {\url{https://github.com/dhwanilpate1/metagratingModCMAES}},
}
