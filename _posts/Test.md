---
layout: single
title: "2023 Test"
---
# 국내
## 추세
### 분석

```python
%%capture
%%SASK
filename _inbox "%sysfunc(getoption(work))/nation.sas7bdat";
 
proc http method="get" 
 URL='https://www.googleapis.com/drive/v3/files/1ByG8nRINtT_IR72IUXYoMQIyNIo6allh?alt=media&key=AIzaSyBfJIzuu9x7AZjgtr0UhbrxNTz0vqbYWv0'
 out=_inbox 
;
run;

filename _inbox clear;
```