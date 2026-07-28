# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Hansen Panel Threshold Regression Use ptr_hansen (tsqr) With (In) R Software
install.packages("tsqr")
library("tsqr")
# Estimation Hansen Panel Threshold Regression Use ptr_hansen (tsqr) With (In) R Software
ptr_hansen = read.csv("https://raw.githubusercontent.com/timbulwidodostp/ptr_hansen/main/ptr_hansen/ptr_hansen.csv",sep = ";")
ptr_hansen = read.csv("C:\\ptr_hansen.csv",sep = ";")
ptr_hansen <- ptr_hansen(formula= ln_GDVA ~ ln_HYV + MCDS_days + Irrigation_pct, data = ptr_hansen, 
threshold_var = "MCDS_days", index = c("district", "year"), n_boot = 50, seed = 42, verbose = FALSE)
summary(ptr_hansen)
# Hansen Panel Threshold Regression Use ptr_hansen (tsqr) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished