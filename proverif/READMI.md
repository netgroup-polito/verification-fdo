# Proverif folder

This folder contains the Proverif source files used for verification.

## FDO_attack_OV_truncated.pv
Proverif model with the attack described in our conference paper "Formal Verification of the FDO Protocol" (2023). The attacker is an intermediate node in the supply chain and uses OV(c) ("truncated OV") to authenticate as the legitimate owner of the device.

## FDO_attack_appnote.pv
Proverif model with the attack described in the FDO appnote http://fidoalliance.org/specs/fidoiot/appnote1-ov-guidance-v1.0-fd-20230306.html (2023). The attacker is an intermediate node in the supply chain and uses OV(b) to authenticate as the legitimate owner of the device.

## FDO_countermeasures_FDO_solution.pv
Proverif model with the countermeasures described by FIDO in the appnote http://fidoalliance.org/specs/fidoiot/appnote1-ov-guidance-v1.0-fd-20230306.html (2023). The model shows that the countermeasure does not solve the MITM attack in the TO1 phase between the device and the server.

## FDO_countermeasure_my_solution.pv
Proverif model with the solution described in our paper. The proposed countermeasures solve all the attacks.

## FDO_countermeasure_my_solution_hashservercert_memory.pv
Proverif model with an alternative solution (described at the end of Section VII.C Note 2). In this case, the device stores a copy of the hash(serverCert) in the DI phase and can get server authentication in the TO1 phase.






