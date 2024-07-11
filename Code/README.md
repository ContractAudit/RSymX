# The source code

The code is shown in this dir, and we suggest the usage of docker. 

### The usage of RSymX (in docker environment)

Update the current running dir. 

```bash
cd /rsymx/rsymx-master
```

Detect contract source code and output the detailed and simply reports.

```bash
/rsymx/rsymx-master/dist/method_testcase_num_contracts_sourcedetection_system/method_testcase_num_contracts_sourcedetection_system /rsymx/test/RealOldFuckMaker.sol 0.4.24 /data/RealOldFuckMaker1 all,main
```

Detect contract bytecode and output the detailed and simply reports.

```bash
/rsymx/rsymx-master/dist/method_testcase_num_contracts_binarydetection_system/method_testcase_num_contracts_binarydetection_system /rsymx/test/RealOldFuckMaker_bin.json /data/RealOldFuckMaker2 all,main
```

Detect contrac opcode and output the detailed and simply reports.

```bash
/rsymx/rsymx-master/dist/method_testcase_num_contracts_evmdetection_system/method_testcase_num_contracts_evmdetection_system /rsymx/test/RealOldFuckMaker_evm.json /data/RealOldFuckMaker3 all,main
```

Detect contrac source code.

```bash
/rsymx/rsymx-master/dist/method_testcase_num_contracts_sourcedetection/method_testcase_num_contracts_sourcedetection /rsymx/test/RealOldFuckMaker.sol 0.4.24 /data/RealOldFuckMaker1-1
```

Detect contrac bytecode.

```bash
/rsymx/rsymx-master/dist/method_testcase_num_contracts_binarydetection/method_testcase_num_contracts_binarydetection /rsymx/test/RealOldFuckMaker_bin.json /data/RealOldFuckMaker2-1
```

Detect contrac opcode.

```bash
/rsymx/rsymx-master/dist/method_testcase_num_contracts_evmdetection/method_testcase_num_contracts_evmdetection /rsymx/test/RealOldFuckMaker_evm.json /data/RealOldFuckMaker3-1
```

Identify contrac behavior with source code.

```bash
/rsymx/rsymx-master/dist/method_testcase_transaction_detection_source/method_testcase_transaction_detection_source /rsymx/test/RealOldFuckMaker.sol 0.4.24 /rsymx/test/user_0000000f.tx.json /data/RealOldFuckMaker1-2
```

Identify contrac behavior with bytecode.

```bash
/rsymx/rsymx-master/dist/method_testcase_transaction_detection_binary/method_testcase_transaction_detection_binary /rsymx/test/RealOldFuckMaker_bin.json /rsymx/test/user_0000000f.tx.json /data/RealOldFuckMaker2-2
```

Identify contrac behavior with opcode.

```bash
/rsymx/rsymx-master/dist/method_testcase_transaction_detection_evm/method_testcase_transaction_detection_evm /rsymx/test/RealOldFuckMaker_evm.json /rsymx/test/user_0000000f.tx.json /data/RealOldFuckMaker3-2
```

Identify contrac behavior with init transaction.

```bash
/rsymx/rsymx-master/dist/method_testcase_transaction_detection_tx/method_testcase_transaction_detection_tx /rsymx/test/user_0000000f_init.tx.json /rsymx/test/user_0000000f.tx.json /data/RealOldFuckMaker3-2
```

Validate detection result of *arbitrary-send* vulnerability.

```bash
/rsymx/rsymx-master/dist/arbitrary-send_transaction_verification/arbitrary-send_transaction_verification /rsymx/test/Arbitrarysend_validation.sol 0.4.24 /rsymx/test/Arbitrarysend_validation/user_00000005.tx.json /data/Arbitrarysend-1
```

Validate detection result of *reentrancy-eth* vulnerability.

```bash
/rsymx/rsymx-master/dist/reentrancy_transaction_verification/reentrancy_transaction_verification /rsymx/test/Reentrance_validation.sol 0.4.24 /rsymx/test/Reentrance_validation/user_00000001.tx.json /data/Reentrance-1
```

Validate detection result of *suicidal* vulnerability.

```bash
/rsymx/rsymx-master/dist/suicidal_transaction_verification/suicidal_transaction_verification /rsymx/test/Suicidal_validation.sol 0.4.24 /rsymx/test/Suicidal_validation/user_00000001.tx.json /data/Suicidal_validation-1
```