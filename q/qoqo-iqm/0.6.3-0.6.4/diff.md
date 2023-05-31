# Comparing `tmp/qoqo_iqm-0.6.3.tar.gz` & `tmp/qoqo_iqm-0.6.4.tar.gz`

## Comparing `qoqo_iqm-0.6.3.tar` & `qoqo_iqm-0.6.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/Cargo.toml
--rwxr-xr-x   0     1001      123    11363 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/LICENSE
--rwxr-xr-x   0     1001      123    20383 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/src/backend.rs
--rwxr-xr-x   0     1001      123     8067 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/src/devices/demo_device.rs
--rwxr-xr-x   0     1001      123     7209 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/src/devices.rs
--rwxr-xr-x   0     1001      123    11936 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/src/interface.rs
--rwxr-xr-x   0     1001      123      822 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/src/lib.rs
--rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 qoqo_iqm-0.6.3/Cargo.toml
--rwxr-xr-x   0     1001      123    11363 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/LICENSE
--rwxr-xr-x   0     1001      123     2653 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/README.md
--rw-r--r--   0     1001      123      835 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/pyproject.toml
--rw-r--r--   0     1001      123  1947151 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/qoqo_iqm/DEPENDENCIES
--rw-r--r--   0     1001      123    12241 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/qoqo_iqm/LICENSE_FOR_BINARY_DISTRIBUTION
--rw-r--r--   0     1001      123     6120 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/qoqo_iqm/OPENSSL_LICENSE
--rw-r--r--   0     1001      123     2404 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/qoqo_iqm/PYTHON_LICENSE
--rw-r--r--   0     1001      123     1330 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/qoqo_iqm/__init__.py
--rwxr-xr-x   0     1001      123    13787 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/src/backend.rs
--rwxr-xr-x   0     1001      123     8259 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/src/devices/demo_device.rs
--rwxr-xr-x   0     1001      123      841 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/src/devices/mod.rs
--rwxr-xr-x   0     1001      123     1482 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/src/lib.rs
--rw-r--r--   0     1001      123    44428 2023-05-23 13:34:14.000000 qoqo_iqm-0.6.3/Cargo.lock
--rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 qoqo_iqm-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/Cargo.toml
+-rwxr-xr-x   0     1001      123    11363 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/LICENSE
+-rwxr-xr-x   0     1001      123    21624 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/src/backend.rs
+-rwxr-xr-x   0     1001      123     8067 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/src/devices/demo_device.rs
+-rwxr-xr-x   0     1001      123     7209 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/src/devices.rs
+-rwxr-xr-x   0     1001      123    17000 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/src/interface.rs
+-rwxr-xr-x   0     1001      123      822 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/src/lib.rs
+-rw-r--r--   0        0        0     1333 1970-01-01 00:00:00.000000 qoqo_iqm-0.6.4/Cargo.toml
+-rwxr-xr-x   0     1001      123    11363 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/LICENSE
+-rwxr-xr-x   0     1001      123     2653 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/README.md
+-rw-r--r--   0     1001      123      835 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/pyproject.toml
+-rw-r--r--   0     1001      123  1947151 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/qoqo_iqm/DEPENDENCIES
+-rw-r--r--   0     1001      123    12241 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/qoqo_iqm/LICENSE_FOR_BINARY_DISTRIBUTION
+-rw-r--r--   0     1001      123     6120 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/qoqo_iqm/OPENSSL_LICENSE
+-rw-r--r--   0     1001      123     2404 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/qoqo_iqm/PYTHON_LICENSE
+-rw-r--r--   0     1001      123     1330 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/qoqo_iqm/__init__.py
+-rwxr-xr-x   0     1001      123    14388 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/src/backend.rs
+-rwxr-xr-x   0     1001      123     8259 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/src/devices/demo_device.rs
+-rwxr-xr-x   0     1001      123      841 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/src/devices/mod.rs
+-rwxr-xr-x   0     1001      123     1482 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/src/lib.rs
+-rw-r--r--   0     1001      123    44428 2023-05-31 15:54:23.000000 qoqo_iqm-0.6.4/Cargo.lock
+-rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 qoqo_iqm-0.6.4/PKG-INFO
```

### Comparing `qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/Cargo.toml` & `qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "roqoqo-iqm"
-version = "0.6.3"
+version = "0.6.4"
 edition = "2021"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 rust-version = "1.63.0"
 categories = ["science", "simulation"]
 # homepage = "https://github.com/HQSquantumsimulations/qoqo_iqm"
 # repository = "https://github.com/HQSquantumsimulations/qoqo_iqm"
```

### Comparing `qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/LICENSE` & `qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/src/backend.rs` & `qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/src/backend.rs`

 * *Files 9% similar despite different names*

```diff
@@ -179,14 +179,27 @@
     let token: Token = serde_json::from_str(&text).map_err(|_| TokenError::JsonError {
         msg: "Token JSON not well formatted".to_string(),
     })?;
 
     Ok(token.access_token)
 }
 
+// Helper function to get number of qubits in a qoqo Circuit
+fn _get_number_qubits(qc: &Circuit) -> Option<usize> {
+    let mut number_qubits_vec: Vec<usize> = vec![];
+    for op in qc.iter() {
+        if let InvolvedQubits::Set(s) = op.involved_qubits() {
+            if let Some(x) = s.iter().max() {
+                number_qubits_vec.push(*x)
+            }
+        }
+    }
+    number_qubits_vec.iter().max().map(|x| x + 1)
+}
+
 /// IQM backend
 ///
 /// Provides functions to run circuits and measurements on IQM devices.
 #[derive(Eq, PartialEq, Debug, Clone, Serialize, Deserialize)]
 pub struct Backend {
     /// IQM device used by the backend
     pub device: IqmDevice,
@@ -245,57 +258,64 @@
     /// Check if the circuit is well-defined according to the device specifications.
     ///
     /// # Arguments
     ///
     /// `qc` - The [roqoqo::Circuit] to be checked
     pub fn validate_circuit(&self, qc: &Circuit) -> Result<(), RoqoqoBackendError> {
         // Check that the circuit doesn't contain more qubits than the device supports
-        let involved_qubits = qc.involved_qubits();
         let mut measured_qubits: Vec<usize> = vec![];
-
-        if let InvolvedQubits::Set(s) = involved_qubits {
-            for qb in s {
-                // equal is also a problem since qoqo starts numbering qubits from 0
-                if qb >= self.device.number_qubits() {
-                    return Err(RoqoqoBackendError::GenericError {
-                        msg: format!(
-                            "Circuit has more qubits than the selected backend device ({}).",
-                            self.device.number_qubits()
-                        ),
-                    });
-                }
+        let number_qubits = match _get_number_qubits(qc) {
+            Some(x) => x,
+            None => {
+                return Err(RoqoqoBackendError::GenericError {
+                    msg: "Empty circuit was passed to the backend.".to_string(),
+                })
             }
-        }
+        };
 
         // Check that
         // 1) The circuit respects the device's connectivity
         // 2) Every qubit is only measured once
+        // 3) Output registers are large enough
         for op in qc.iter() {
             match op {
                 Operation::MeasureQubit(o) => {
                     let qubit = *o.qubit();
                     if measured_qubits.contains(&qubit) {
                         return Err(RoqoqoBackendError::GenericError {
                             msg: format!("Qubit {} is being measured more than once.", &qubit),
                         });
                     } else {
                         measured_qubits.push(qubit)
                     }
                 }
-                Operation::PragmaRepeatedMeasurement(_) => {
+                Operation::PragmaRepeatedMeasurement(o) => {
                     if !measured_qubits.is_empty() {
                         return Err(RoqoqoBackendError::GenericError {
                            msg: "Qubits are being measured more than once. When using
                                 PragmaRepeatedMeasurement, there should not be individual qubit
                                 measurements, and the PragmaRepeatedMeasurement operation can appear only
                                 once in the circuit.".to_string(),
                         });
                     } else {
                         measured_qubits.extend(0..self.device.number_qubits())
                     }
+
+                    let mut readout_length: usize = 0;
+                    for def in qc.definitions() {
+                        if let Operation::DefinitionBit(reg) = def {
+                            readout_length = *reg.length()
+                        }
+                    }
+
+                    if number_qubits > readout_length {
+                        return Err(RoqoqoBackendError::GenericError {
+                            msg: format!("Readout register {} is not large enough.", o.readout()),
+                        });
+                    }
                 }
                 _ => {
                     if let Ok(inner_op) = SingleQubitOperation::try_from(op) {
                         if self
                             .device
                             .single_qubit_gate_time(inner_op.hqslang(), inner_op.qubit())
                             .is_none()
@@ -489,24 +509,40 @@
         Ok((bit_registers, float_registers, complex_registers))
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
+    use std::f64::consts::PI;
 
     #[test]
     fn test_qubit_name_conversion_iqm_to_qoqo() {
         let qubit = String::from("QB2");
         let converted_name = _convert_qubit_name_iqm_to_qoqo(qubit);
 
         assert_eq!(converted_name, 1)
     }
 
     #[test]
+    fn test_get_number_qubits() {
+        let mut qc = Circuit::new();
+
+        assert!(_get_number_qubits(&qc).is_none());
+
+        qc += RotateXY::new(0, PI.into(), 0.0.into());
+        qc += RotateXY::new(2, PI.into(), 0.0.into());
+        qc += RotateXY::new(6, PI.into(), 0.0.into());
+        qc += DefinitionBit::new("my_reg".to_string(), 2, true);
+        qc += PragmaRepeatedMeasurement::new("my_reg".to_string(), 10, None);
+
+        assert_eq!(_get_number_qubits(&qc), Some(7))
+    }
+
+    #[test]
     fn test_results_to_registers() {
         let mut bit_registers: HashMap<String, BitOutputRegister> = HashMap::new();
         bit_registers.insert(
             "reg1".to_string(),
             vec![
                 vec![false, false, false, false, false],
                 vec![false, false, false, false, false],
```

### Comparing `qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/src/devices/demo_device.rs` & `qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/src/devices/demo_device.rs`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/src/devices.rs` & `qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/src/devices.rs`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/src/interface.rs` & `qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/src/interface.rs`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,26 @@
 use std::collections::HashMap;
 
 use qoqo_calculator::CalculatorFloat;
 use roqoqo::operations::*;
 use roqoqo::registers::BitOutputRegister;
 use roqoqo::RoqoqoBackendError;
 
+// Pragma operations that are ignored by backend and do not throw an error
+const ALLOWED_OPERATIONS: &[&str; 8] = &[
+    "PragmaBoostNoise",
+    "PragmaStopParallelBlock",
+    "PragmaGlobalPhase",
+    "InputSymbolic",
+    "InputBit",
+    "PragmaRepeatedMeasurement",
+    "PragmaStartDecompositionBlock",
+    "PragmaStopDecompositionBlock",
+];
+
 /// Convert a qubit number into the format accepted by IQM.
 // e.g. "QB2" for qoqo_qubit number 1 (IQM qubits start from 1)
 #[inline]
 fn _convert_qubit_name_qoqo_to_iqm(qoqo_qubit: usize) -> String {
     format!("QB{}", qoqo_qubit + 1)
 }
 
@@ -59,15 +71,17 @@
     pub qubits: Vec<String>,
     /// Arguments of the instruction. They depend on the type of operation, and can hold both gate
     ///parameters or measurement names. The latter are used as register names when converting the
     /// results into roqoqo registers.
     pub args: HashMap<String, CalculatorFloat>,
 }
 
-// HashMap that to each register name associates the indices in the register that are being affected by measurements. These indices are saved in the order in which the measurement operations appear in the circuit, since this is the order in which the backend returns the results.
+// HashMap that associates to each register name the indices in the register that are being affected
+// by measurements. These indices are saved in the order in which the measurement operations appear
+// in the circuit, since this is the order in which the backend returns the results.
 type RegisterMapping = HashMap<String, Vec<usize>>;
 
 /// Converts all operations in a [roqoqo::Circuit] into instructions for IQM Hardware or IQM Simulators
 ///
 /// # Arguments
 ///
 /// `circuit` - The [roqoqo::Circuit] that is converted
@@ -84,51 +98,67 @@
 pub fn call_circuit<'a>(
     circuit: impl Iterator<Item = &'a Operation>,
     device_number_qubits: usize,
     output_registers: &mut HashMap<String, BitOutputRegister>,
 ) -> Result<(IqmCircuit, RegisterMapping, usize), RoqoqoBackendError> {
     let mut circuit_vec: Vec<IqmInstruction> = Vec::new();
     let mut number_measurements: usize = 1;
+    let mut measured_qubits: Vec<usize> = vec![];
     let mut register_mapping: RegisterMapping = HashMap::new();
 
     for op in circuit {
         match op {
             Operation::DefinitionBit(o) => {
                 // initialize output registers with default `false` values
                 if *o.is_output() {
                     output_registers
                         .insert((*o).name().to_string(), vec![vec![false; *o.length()]]);
                     register_mapping.insert((*o).name().to_string(), vec![]);
                 }
             }
             Operation::MeasureQubit(o) => {
                 let readout = o.readout().clone();
+                measured_qubits.push(*o.qubit());
+
                 match register_mapping.get_mut(&readout) {
                     Some(x) => x.push(*o.readout_index()),
                     None => {
                         return Err(RoqoqoBackendError::GenericError {
                             msg: "A MeasureQubit operation is writing to an undefined register."
                                 .to_string(),
                         })
                     }
                 }
                 let mut found: bool = false;
                 // Check if we already have a measurement to the same register
                 // if yes, add the qubit being measured to that measurement
-                for i in &mut circuit_vec {
-                    if i.name == "measurement" {
+                for instr in &mut circuit_vec {
+                    if instr.name == "measurement" {
                         let meas_readout =
-                            i.args.get("key").ok_or(RoqoqoBackendError::GenericError {
+                            instr
+                                .args
+                                .get("key")
+                                .ok_or(RoqoqoBackendError::GenericError {
                                 msg: "A measurement must contain a `key` entry in the `args` field"
                                     .to_string(),
                             })?;
                         if let CalculatorFloat::Str(s) = meas_readout {
                             if s == &readout {
                                 found = true;
-                                i.qubits.push(_convert_qubit_name_qoqo_to_iqm(*o.qubit()));
+                                let iqm_qubit = _convert_qubit_name_qoqo_to_iqm(*o.qubit());
+                                if !instr.qubits.contains(&iqm_qubit) {
+                                    instr.qubits.push(iqm_qubit);
+                                } else {
+                                    return Err(RoqoqoBackendError::GenericError {
+                                        msg: format!(
+                                            "Qubit {} is being measured twice.",
+                                            *o.qubit()
+                                        ),
+                                    });
+                                }
                                 break;
                             }
                         }
                     }
                 }
                 if !found {
                     // If no measurement to the same register was found, create a new IqmInstruction
@@ -136,29 +166,107 @@
                         name: "measurement".to_string(),
                         qubits: vec![_convert_qubit_name_qoqo_to_iqm(*o.qubit())],
                         args: HashMap::from([("key".to_string(), CalculatorFloat::Str(readout))]),
                     };
                     circuit_vec.push(meas)
                 }
             }
+            Operation::PragmaSetNumberOfMeasurements(o) => {
+                if number_measurements > 1 {
+                    return Err(RoqoqoBackendError::GenericError {
+                        msg: "Only one repeated measurement is allowed in the circuit.".to_string(),
+                    });
+                }
+
+                number_measurements = *o.number_measurements();
+                let readout = o.readout().clone();
+
+                if !output_registers.contains_key(&readout) {
+                    return Err(RoqoqoBackendError::GenericError {
+                        msg: format!(
+                            "PragmaSetNumberOfMeasurements writes to an undefined register {}",
+                            &readout
+                        ),
+                    });
+                } else {
+                    let readout_length = match output_registers
+                        .get(&readout)
+                        .expect("PragmaSetNumberOfMeasurements writes to an undefined register.")
+                        .first()
+                    {
+                        Some(v) => v.len(),
+                        None => {
+                            return Err(RoqoqoBackendError::GenericError {
+                                msg: format!(
+                                    "Output register {} has not been initialized correctly.",
+                                    &readout
+                                ),
+                            })
+                        }
+                    };
+
+                    if measured_qubits.len() > readout_length {
+                        return Err(RoqoqoBackendError::GenericError {
+                            msg: format!("PragmaSetNumberOfMeasurements writes to register {}, which is too small.", &readout) });
+                    }
+
+                    // remove MeasureQubit operations
+                    let mut old_measurement_indices = vec![];
+                    for (i, meas) in circuit_vec.iter().enumerate() {
+                        if meas.name == "measurement" {
+                            old_measurement_indices.push(i);
+                        }
+                    }
+                    for i in old_measurement_indices.into_iter().rev() {
+                        circuit_vec.remove(i);
+                    }
+
+                    // update register mapping with the only register specified by PragmaSetNumberOfMeasurements
+                    register_mapping = HashMap::new();
+                    register_mapping.insert(readout.clone(), measured_qubits.clone());
+
+                    // add single measurement instruction for all the qubits that were measured with MeasureQubit
+                    let meas = IqmInstruction {
+                        name: "measurement".to_string(),
+                        qubits: measured_qubits
+                            .iter()
+                            .map(|x| _convert_qubit_name_qoqo_to_iqm(*x))
+                            .collect(),
+                        args: HashMap::from([("key".to_string(), CalculatorFloat::Str(readout))]),
+                    };
+                    circuit_vec.push(meas)
+                }
+            }
             Operation::PragmaRepeatedMeasurement(o) => {
+                if number_measurements > 1 {
+                    return Err(RoqoqoBackendError::GenericError {
+                        msg: "Only one repeated measurement is allowed in the circuit.".to_string(),
+                    });
+                }
+                if !measured_qubits.is_empty() {
+                    return Err(RoqoqoBackendError::GenericError {
+                        msg: "Some qubits are being measured twice.".to_string(),
+                    });
+                }
+
                 number_measurements = *o.number_measurements();
                 let readout = o.readout().clone();
 
                 match o.qubit_mapping() {
                     None => {
                         if output_registers.contains_key(&readout) {
                             let readout_length = match output_registers
                                 .get(&readout)
                                 .expect("Tried to access a register that is not a key of output_registers.")
                                 .first() {
                                     Some(v) => v.len(),
                                     None => return Err(RoqoqoBackendError::GenericError {
                                         msg: format!("Output register {} has not been initialized correctly.", &readout) })
                                 };
+
                             register_mapping.insert(
                                 o.readout().to_string(),
                                 (0..readout_length).collect(),
                             );
                         } else {
                             return Err(RoqoqoBackendError::GenericError {
                                 msg: "A PragmaRepeatedMeasurement operation is writing to an undefined register.".to_string() })
@@ -193,22 +301,24 @@
                             "Only Loops with non-symbolic repetitions are supported by the backend."
                                 .to_string(),
                     }
                         })?;
                 let reps = (*reps_ref) as i32;
                 for _ in 0..reps {
                     for i in o.circuit().iter() {
-                        let instruction = call_operation(i)?;
-                        circuit_vec.push(instruction);
+                        if let Some(instruction) = call_operation(i)? {
+                            circuit_vec.push(instruction);
+                        }
                     }
                 }
             }
             _ => {
-                let instruction = call_operation(op)?;
-                circuit_vec.push(instruction)
+                if let Some(instruction) = call_operation(op)? {
+                    circuit_vec.push(instruction)
+                }
             }
         };
     }
 
     if number_measurements > 1 {
         for (_, value) in output_registers.iter_mut() {
             *value = vec![(*value)[0].to_vec(); number_measurements];
@@ -233,43 +343,49 @@
 ///
 /// `operation` - The [roqoqo::operations::Operation] that is converted
 ///
 /// # Returns
 ///
 /// `Ok(IqmInstruction)` - Converted instruction  
 /// `Err(RoqoqoBackendError::OperationNotInBackend)` - Error when [roqoqo::operations::Operation] can not be converted
-pub fn call_operation(operation: &Operation) -> Result<IqmInstruction, RoqoqoBackendError> {
+pub fn call_operation(operation: &Operation) -> Result<Option<IqmInstruction>, RoqoqoBackendError> {
     let mut op_parameters = HashMap::new();
 
     match operation {
         Operation::RotateXY(op) => {
             op_parameters.insert(
                 "angle_t".to_string(),
                 CalculatorFloat::Float(*op.theta().float()?),
             );
             op_parameters.insert(
                 "phase_t".to_string(),
                 CalculatorFloat::Float(*op.phi().float()?),
             );
 
-            Ok(IqmInstruction {
+            Ok(Some(IqmInstruction {
                 name: "phased_rx".to_string(),
                 qubits: vec![_convert_qubit_name_qoqo_to_iqm(*op.qubit())],
                 args: op_parameters,
-            })
+            }))
         }
         Operation::ControlledPauliZ(op) => {
             let control = _convert_qubit_name_qoqo_to_iqm(*op.control());
             let target = _convert_qubit_name_qoqo_to_iqm(*op.target());
 
-            Ok(IqmInstruction {
+            Ok(Some(IqmInstruction {
                 name: "cz".to_string(),
                 qubits: vec![control, target],
                 args: op_parameters,
-            })
+            }))
+        }
+        _ => {
+            if ALLOWED_OPERATIONS.contains(&operation.hqslang()) {
+                Ok(None)
+            } else {
+                Err(RoqoqoBackendError::OperationNotInBackend {
+                    backend: "IQM",
+                    hqslang: operation.hqslang(),
+                })
+            }
         }
-        _ => Err(RoqoqoBackendError::OperationNotInBackend {
-            backend: "IQM",
-            hqslang: operation.hqslang(),
-        }),
     }
 }
```

### Comparing `qoqo_iqm-0.6.3/local_dependencies/roqoqo-iqm/src/lib.rs` & `qoqo_iqm-0.6.4/local_dependencies/roqoqo-iqm/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/Cargo.toml` & `qoqo_iqm-0.6.4/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qoqo-iqm"
-version = "0.6.3"
+version = "0.6.4"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 homepage = "https://github.com/HQSquantumsimulations/qoqo_iqm"
 repository = "https://github.com/HQSquantumsimulations/qoqo_iqm"
 documentation = "https://docs.rs/qoqo_iqm/"
 readme = "README.md"
 edition = "2021"
```

### Comparing `qoqo_iqm-0.6.3/LICENSE` & `qoqo_iqm-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/README.md` & `qoqo_iqm-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/pyproject.toml` & `qoqo_iqm-0.6.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qoqo_iqm"
-version = "0.6.3"
+version = "0.6.4"
 dependencies = [
   'numpy',
   'qoqo_calculator_pyo3>=1.1',
   'qoqo>=1.4',
 ]
 description = "IQM-backend for the qoqo/roqoqo quantum toolkit by HQS Quantum Simulations."
```

### Comparing `qoqo_iqm-0.6.3/qoqo_iqm/DEPENDENCIES` & `qoqo_iqm-0.6.4/qoqo_iqm/DEPENDENCIES`

 * *Files 0% similar despite different names*

```diff
@@ -1504,15 +1504,15 @@
 00005df0: 5457 4152 4520 4f52 2054 4845 2055 5345  TWARE OR THE USE
 00005e00: 204f 5220 4f54 4845 520a 4445 414c 494e   OR OTHER.DEALIN
 00005e10: 4753 2049 4e20 5448 4520 534f 4654 5741  GS IN THE SOFTWA
 00005e20: 5245 2e0a 0a0a 3d3d 3d3d 3d3d 3d3d 3d3d  RE....==========
 00005e30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00005e40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00005e50: 3d3d 3d3d 3d3d 3d3d 3d3d 0a62 6173 6536  ==========.base6
-00005e60: 3420 302e 3231 2e31 0a68 7474 7073 3a2f  4 0.21.1.https:/
+00005e60: 3420 302e 3231 2e32 0a68 7474 7073 3a2f  4 0.21.2.https:/
 00005e70: 2f67 6974 6875 622e 636f 6d2f 6d61 7273  /github.com/mars
 00005e80: 6861 6c6c 7069 6572 6365 2f72 7573 742d  hallpierce/rust-
 00005e90: 6261 7365 3634 0a62 7920 416c 6963 6520  base64.by Alice 
 00005ea0: 4d61 7a20 3c61 6c69 6365 4061 6c69 6365  Maz <alice@alice
 00005eb0: 6d61 7a2e 636f 6d3e 2c20 4d61 7273 6861  maz.com>, Marsha
 00005ec0: 6c6c 2050 6965 7263 6520 3c6d 6172 7368  ll Pierce <marsh
 00005ed0: 616c 6c40 6d70 6965 7263 652e 6f72 673e  all@mpierce.org>
@@ -28360,15 +28360,15 @@
 0006ec70: 454e 2049 4620 4144 5649 5345 4420 4f46  EN IF ADVISED OF
 0006ec80: 2054 4845 2050 4f53 5349 4249 4c49 5459   THE POSSIBILITY
 0006ec90: 204f 4620 5355 4348 2044 414d 4147 452e   OF SUCH DAMAGE.
 0006eca0: 0d0a 0a0a 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ....============
 0006ecb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0006ecc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0006ecd0: 3d3d 3d3d 3d3d 3d3d 0a69 6f2d 6c69 6665  ========.io-life
-0006ece0: 7469 6d65 7320 312e 302e 3130 0a68 7474  times 1.0.10.htt
+0006ece0: 7469 6d65 7320 312e 302e 3131 0a68 7474  times 1.0.11.htt
 0006ecf0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 0006ed00: 7375 6e66 6973 6863 6f64 652f 696f 2d6c  sunfishcode/io-l
 0006ed10: 6966 6574 696d 6573 0a62 7920 4461 6e20  ifetimes.by Dan 
 0006ed20: 476f 686d 616e 203c 6465 7640 7375 6e66  Gohman <dev@sunf
 0006ed30: 6973 6863 6f64 652e 6f6e 6c69 6e65 3e0a  ishcode.online>.
 0006ed40: 4120 6c6f 772d 6c65 7665 6c20 492f 4f20  A low-level I/O 
 0006ed50: 6f77 6e65 7273 6869 7020 616e 6420 626f  ownership and bo
@@ -64143,15 +64143,15 @@
 000fa8e0: 6720 7065 726d 6973 7369 6f6e 7320 616e  g permissions an
 000fa8f0: 640a 2020 206c 696d 6974 6174 696f 6e73  d.   limitations
 000fa900: 2075 6e64 6572 2074 6865 204c 6963 656e   under the Licen
 000fa910: 7365 2e0a 0a0a 3d3d 3d3d 3d3d 3d3d 3d3d  se....==========
 000fa920: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000fa930: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000fa940: 3d3d 3d3d 3d3d 3d3d 3d3d 0a71 6f71 6f2d  ==========.qoqo-
-000fa950: 6971 6d20 302e 362e 330a 6874 7470 733a  iqm 0.6.3.https:
+000fa950: 6971 6d20 302e 362e 340a 6874 7470 733a  iqm 0.6.4.https:
 000fa960: 2f2f 6769 7468 7562 2e63 6f6d 2f48 5153  //github.com/HQS
 000fa970: 7175 616e 7475 6d73 696d 756c 6174 696f  quantumsimulatio
 000fa980: 6e73 2f71 6f71 6f5f 6971 6d0a 6279 2048  ns/qoqo_iqm.by H
 000fa990: 5153 2051 7561 6e74 756d 2053 696d 756c  QS Quantum Simul
 000fa9a0: 6174 696f 6e73 203c 696e 666f 4071 7561  ations <info@qua
 000fa9b0: 6e74 756d 7369 6d75 6c61 7469 6f6e 732e  ntumsimulations.
 000fa9c0: 6465 3e0a 4951 4d20 6261 636b 656e 6420  de>.IQM backend 
@@ -73863,15 +73863,15 @@
 00120860: 6e67 2070 6572 6d69 7373 696f 6e73 2061  ng permissions a
 00120870: 6e64 0a20 2020 6c69 6d69 7461 7469 6f6e  nd.   limitation
 00120880: 7320 756e 6465 7220 7468 6520 4c69 6365  s under the Lice
 00120890: 6e73 652e 0a0a 0a3d 3d3d 3d3d 3d3d 3d3d  nse....=========
 001208a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 001208b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 001208c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 726f 716f  ===========.roqo
-001208d0: 716f 2d69 716d 2030 2e36 2e33 0a62 7920  qo-iqm 0.6.3.by 
+001208d0: 716f 2d69 716d 2030 2e36 2e34 0a62 7920  qo-iqm 0.6.4.by 
 001208e0: 4851 5320 5175 616e 7475 6d20 5369 6d75  HQS Quantum Simu
 001208f0: 6c61 7469 6f6e 7320 3c69 6e66 6f40 7175  lations <info@qu
 00120900: 616e 7475 6d73 696d 756c 6174 696f 6e73  antumsimulations
 00120910: 2e64 653e 0a49 514d 2069 6e74 6572 6661  .de>.IQM interfa
 00120920: 6365 2066 6f72 2072 6f71 6f71 6f20 7275  ce for roqoqo ru
 00120930: 7374 2071 7561 6e74 756d 2063 6f6d 7075  st quantum compu
 00120940: 7469 6e67 2074 6f6f 6c6b 6974 0a4c 6963  ting toolkit.Lic
@@ -93775,15 +93775,15 @@
 0016e4e0: 2055 5345 204f 5220 4f54 4845 520a 4445   USE OR OTHER.DE
 0016e4f0: 414c 494e 4753 2049 4e20 5448 4520 534f  ALINGS IN THE SO
 0016e500: 4654 5741 5245 2e0a 0a0a 3d3d 3d3d 3d3d  FTWARE....======
 0016e510: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0016e520: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0016e530: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a75  ==============.u
 0016e540: 6e69 636f 6465 2d69 6465 6e74 2031 2e30  nicode-ident 1.0
-0016e550: 2e38 0a68 7474 7073 3a2f 2f67 6974 6875  .8.https://githu
+0016e550: 2e39 0a68 7474 7073 3a2f 2f67 6974 6875  .9.https://githu
 0016e560: 622e 636f 6d2f 6474 6f6c 6e61 792f 756e  b.com/dtolnay/un
 0016e570: 6963 6f64 652d 6964 656e 740a 6279 2044  icode-ident.by D
 0016e580: 6176 6964 2054 6f6c 6e61 7920 3c64 746f  avid Tolnay <dto
 0016e590: 6c6e 6179 4067 6d61 696c 2e63 6f6d 3e0a  lnay@gmail.com>.
 0016e5a0: 4465 7465 726d 696e 6520 7768 6574 6865  Determine whethe
 0016e5b0: 7220 6368 6172 6163 7465 7273 2068 6176  r characters hav
 0016e5c0: 6520 7468 6520 5849 445f 5374 6172 7420  e the XID_Start
```

### Comparing `qoqo_iqm-0.6.3/qoqo_iqm/LICENSE_FOR_BINARY_DISTRIBUTION` & `qoqo_iqm-0.6.4/qoqo_iqm/LICENSE_FOR_BINARY_DISTRIBUTION`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/qoqo_iqm/OPENSSL_LICENSE` & `qoqo_iqm-0.6.4/qoqo_iqm/OPENSSL_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/qoqo_iqm/PYTHON_LICENSE` & `qoqo_iqm-0.6.4/qoqo_iqm/PYTHON_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/qoqo_iqm/__init__.py` & `qoqo_iqm-0.6.4/qoqo_iqm/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/src/backend.rs` & `qoqo_iqm-0.6.4/src/backend.rs`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,25 @@
         Ok(Self {
             internal: Backend::new(iqm_device, access_token).map_err(|err| {
                 PyRuntimeError::new_err(format!("No access token found {:?}", err))
             })?,
         })
     }
 
+    /// Overwrite the number of measurements that will be executed on the [qoqo::Circuit] or the
+    /// [qoqo::QuantumProgram]. The default number of measurements is the one defined in the submitted
+    /// circuits.
+    ///
+    /// WARNING: this function will overwrite the number of measurements set in a Circuit or
+    /// QuantumProgram. Changing the number of measurments WILL change the accuracy of the result.
+    pub fn _overwrite_number_of_measurements(&mut self, number_measurements: usize) {
+        self.internal
+            ._overwrite_number_of_measurements(number_measurements)
+    }
+
     /// Return a copy of the Backend (copy here produces a deepcopy).
     ///
     /// Returns:
     ///     Backend: A deep copy of self.
     pub fn __copy__(&self) -> BackendWrapper {
         self.clone()
     }
```

### Comparing `qoqo_iqm-0.6.3/src/devices/demo_device.rs` & `qoqo_iqm-0.6.4/src/devices/demo_device.rs`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/src/devices/mod.rs` & `qoqo_iqm-0.6.4/src/devices/mod.rs`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/src/lib.rs` & `qoqo_iqm-0.6.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo_iqm-0.6.3/Cargo.lock` & `qoqo_iqm-0.6.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "base64"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3f1e31e207a6b8fb791a38ea3105e6cb541f55e4d029902d3039a4ad07cc4105"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "bincode"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
@@ -368,17 +368,17 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
@@ -869,15 +869,15 @@
  "serde_json",
  "syn 2.0.16",
  "thiserror",
 ]
 
 [[package]]
 name = "qoqo-iqm"
-version = "0.6.3"
+version = "0.6.4"
 dependencies = [
  "bincode",
  "pyo3",
  "pyo3-build-config",
  "qoqo",
  "qoqo_calculator",
  "qoqo_calculator_pyo3",
@@ -1065,15 +1065,15 @@
  "proc-macro2",
  "quote",
  "syn 2.0.16",
 ]
 
 [[package]]
 name = "roqoqo-iqm"
-version = "0.6.3"
+version = "0.6.4"
 dependencies = [
  "itertools",
  "ndarray",
  "qoqo_calculator",
  "reqwest",
  "roqoqo",
  "serde",
@@ -1428,17 +1428,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
```

### Comparing `qoqo_iqm-0.6.3/PKG-INFO` & `qoqo_iqm-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_iqm
-Version: 0.6.3
+Version: 0.6.4
 Requires-Dist: numpy
 Requires-Dist: qoqo_calculator_pyo3 >=1.1
 Requires-Dist: qoqo >=1.4
 Requires-Dist: sphinx >=2.1 ; extra == 'docs'
 Requires-Dist: nbsphinx ; extra == 'docs'
 Requires-Dist: pygments ; extra == 'docs'
 Requires-Dist: recommonmark ; extra == 'docs'
```

