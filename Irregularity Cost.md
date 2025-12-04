PK_TABLE_PAX Formula =IF(A2="";"";CONCATENATE(DATEVALUE(A2);".";B2))

KEY_OTP_TABLE Formula =IF(A2="";"";CONCATENATE(DATEVALUE(A2);".";B2))

PAX Formula =IF(AD2="";"";IFERROR(VLOOKUP(AD2;'[PAX_2020-2025.xlsx]Sheet1'!$G:$H;2;FALSE);""))

PAX (On PAX_2020-2025 table) Formula =IF(G2="";"";E2)

COMPENSATIO_COST Formula =  =IF(AC2="";"";IFERROR(VLOOKUP(AC2;compensation_policies!$A$1:$C$6;3;FALSE);"")*aims_flight!AE2)
