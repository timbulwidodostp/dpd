# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Dynamic Panel Data Models Use dpd (dynpanel) With (In) R Software
install.packages("dynpanel")
library("dynpanel")
# Estimation Dynamic Panel Data Models Use dpd (dynpanel) With (In) R Software
dpd = read.csv("https://raw.githubusercontent.com/timbulwidodostp/dpd/main/dpd/dpd.csv",sep = ";")
dpd <- dpd(log(dpd) ~ log(dpd_1) + log(dpd_2) + log(dpd_3) + dpd_4, dpd, index = c("state", "year"), 1,4)
summary(dpd)
# Dynamic Panel Data Models Use dpd (dynpanel) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished