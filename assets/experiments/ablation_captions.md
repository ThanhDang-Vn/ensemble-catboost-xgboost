# Ablation Study: Figure Captions and Interpretations

## fig_reg_xgb_regalpha
Figure: Effect of XGBoost L1 regularization (reg_alpha) on validation RMSE (mean ± std across 3 seeds). Higher reg_alpha slightly increases validation RMSE, suggesting limited underfitting benefits on this dataset. Training time and number of features used remain stable across the tested range.

## fig_reg_xgb_reglambda
Figure: Effect of XGBoost L2 regularization (reg_lambda) on validation RMSE (mean ± std across 3 seeds). Within the tested range, reg_lambda produced minor RMSE fluctuations, indicating L2 regularization plays a small role for this dataset/setting.

## fig_reg_cat_l2
Figure: Effect of CatBoost L2 regularization (l2_leaf_reg) on RMSE (mean ± std). Larger L2 reduced overfitting (train RMSE increases) and slightly increased validation RMSE, indicating a trade-off between bias and variance.

## fig_sampling_xgb_heatmap
Figure: Heatmap of XGBoost validation RMSE (mean over seeds) across (subsample, colsample_bytree). Moderate subsampling and feature sampling produced marginal RMSE improvements in some cells, but overall differences are small.

## fig_sampling_cat_bag
Figure: CatBoost bagging_temperature effect on RMSE (mean ± std). Changes in bagging temperature had negligible impact on validation RMSE for this dataset.

## fig_tree_xgb_growpolicy
Figure: XGBoost grow policy comparison (depthwise vs lossguide). RMSE (mean ± std) is similar between policies; lossguide shows a modest increase in training time here.

## fig_tree_cat_depth
Figure: CatBoost symmetric-tree depth sweep: RMSE (mean ± std) and nodes per tree (theoretical). Deeper trees reduce RMSE marginally at the cost of significantly more nodes and longer training time.
