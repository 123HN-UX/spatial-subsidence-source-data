# Source data inventory

CSV files are UTF-8 (some include a BOM). Values and headers are preserved unchanged. Historical figure numbers in filenames can differ from the final manuscript. Units explicitly encoded in column names follow those names. Consult the manuscript for model codes and scenario definitions.

## Fig04_GNSS_neighborhood_series.csv

Matched GNSS and InSAR neighborhood histories. Historical figure number; GNSS_up_m retains its original origin, different from relative InSAR displacement.

Rows: 249. Columns: date, GNSS_up_m, InSAR_250m_m, InSAR_500m_m, InSAR_1000m_m, InSAR_2000m_m.

## Fig10_fixed_case_series.csv

Displacement histories for four selected grid cells. Historical figure number.

Rows: 249. Columns: date, E143_N497, E144_N497, E145_N496, E146_N496.

## GNSS_metrics.csv

GNSS/InSAR neighborhood comparison metrics at multiple radii.

Rows: 4. Columns: radius_m, pixels, epochs, nearest_pixel_m, mean_distance_m, GNSS_rate_mm_year, InSAR_rate_mm_year, rate_difference_mm_year, offset_aligned_RMSE_mm, coherence_median, jump_fraction.

## Supplementary_Fig_S1_selection_rules.csv

Selection descriptors for representative complete grid histories.

Rows: 4. Columns: grid_id, description, pixels, median_seasonal_rate_mm_yr, median_late_minus_early_rate_mm_yr, repeated_jump_fraction, selected_model.

## Supplementary_Fig_S1_series.csv

Representative grid histories, pixel envelopes and full-period fits.

Rows: 996. Columns: grid_id, date, median_mm, pixel_q25_mm, pixel_q75_mm, full_period_fit_mm.

## Supplementary_Fig_S2_fits_and_residuals.csv

Observed/fitted histories and model residuals.

Rows: 747. Columns: grid_id, model, date, observed_mm, fitted_mm, residual_mm.

## Supplementary_Fig_S2_residual_correlations.csv

Residual correlations by acquisition lag.

Rows: 36. Columns: grid_id, model, lag_acquisitions, residual_correlation.

## Supplementary_Fig_S3_extreme_node_histories.csv

Paired Hato model water-level histories; derived from the third-party FVCOM archive.

Rows: 192. Columns: source_node_index, time_mjd, hours_since_start, baseline_water_level_m, SLR03_water_level_m, synchronous_residual_m.

## Supplementary_Fig_S3_node_responses.csv

Paired Hato node response metrics; derived from the third-party FVCOM archive.

Rows: 9438. Columns: node_index, lon, lat, baseline_event_max_m, SLR03_event_max_m, event_max_difference_m, nonadditive_residual_m.

## land_cover_bootstrap.csv

Paired within-cell land-cover contrasts and bootstrap bounds.

Rows: 5. Columns: class_code, class_name, paired_cells, median_within_cell_difference_mm_year, bootstrap_p025, bootstrap_p975.

## rank_correlations.csv

Ranking correlation summaries under grid-size and offset settings.

Rows: 12. Columns: size_m, offset_x, offset_y, common_cells, pairwise_spearman_min, pairwise_spearman_median, pairwise_spearman_max.

## threshold_responses.csv

Areas classified by branch, scenario, quantile, year and elevation-loss threshold.

Rows: 70812. Columns: branch, scenario, path_quantile, year, threshold_m, domain_area_km2, S1_area_km2, S2_area_km2, S2_only_km2, S1_only_km2, both_km2, neither_km2.
