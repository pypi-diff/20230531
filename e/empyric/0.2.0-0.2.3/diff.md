# Comparing `tmp/empyric-0.2.0.tar.gz` & `tmp/empyric-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empyric-0.2.0.tar", max compression
+gzip compressed data, was "empyric-0.2.3.tar", max compression
```

## Comparing `empyric-0.2.0.tar` & `empyric-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1057 2022-02-05 04:17:18.866045 empyric-0.2.0/LICENSE
--rw-r--r--   0        0        0     7090 2023-05-26 05:49:13.218533 empyric-0.2.0/README.md
--rw-r--r--   0        0        0     2260 2023-05-22 05:18:01.391399 empyric-0.2.0/empyric/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 05:42:12.136341 empyric-0.2.0/empyric/__main__.py
--rw-r--r--   0        0        0    39265 2023-05-17 05:28:01.619337 empyric-0.2.0/empyric/adapters.py
--rw-r--r--   0        0        0       36 2023-03-29 06:16:12.180511 empyric-0.2.0/empyric/collection/__init__.py
--rw-r--r--   0        0        0     1711 2023-04-06 03:05:54.032558 empyric-0.2.0/empyric/collection/barometers.py
--rw-r--r--   0        0        0    11216 2023-05-17 04:53:19.432757 empyric-0.2.0/empyric/collection/controllers.py
--rw-r--r--   0        0        0     8578 2023-04-06 03:05:54.036020 empyric-0.2.0/empyric/collection/generators.py
--rw-r--r--   0        0        0     1212 2023-04-06 03:05:54.036470 empyric-0.2.0/empyric/collection/humans.py
--rw-r--r--   0        0        0     9460 2023-04-06 03:05:54.037384 empyric-0.2.0/empyric/collection/instrument.py
--rw-r--r--   0        0        0     3205 2023-04-06 03:05:54.038856 empyric-0.2.0/empyric/collection/io.py
--rw-r--r--   0        0        0    17409 2023-05-17 04:53:19.433598 empyric-0.2.0/empyric/collection/multimeters.py
--rw-r--r--   0        0        0    22050 2023-05-10 03:42:21.592096 empyric-0.2.0/empyric/collection/scopes.py
--rw-r--r--   0        0        0    28190 2023-04-14 06:00:29.449094 empyric-0.2.0/empyric/collection/sourcemeters.py
--rw-r--r--   0        0        0     3742 2023-04-06 03:05:54.041505 empyric-0.2.0/empyric/collection/spectrometers.py
--rw-r--r--   0        0        0     6851 2023-04-06 03:05:54.042207 empyric-0.2.0/empyric/collection/supplies.py
--rw-r--r--   0        0        0     2131 2023-04-06 03:05:54.042818 empyric-0.2.0/empyric/collection/thermometers.py
--rw-r--r--   0        0        0    10099 2023-04-06 03:05:54.044153 empyric-0.2.0/empyric/collection/virtual.py
--rw-r--r--   0        0        0    30149 2023-05-17 04:53:19.434369 empyric-0.2.0/empyric/experiment.py
--rw-r--r--   0        0        0    37572 2023-05-26 05:42:17.608271 empyric-0.2.0/empyric/graphics.py
--rw-r--r--   0        0        0      760 2023-04-21 03:37:51.903945 empyric-0.2.0/empyric/instruments.py
--rw-r--r--   0        0        0    32803 2023-05-26 05:42:17.608698 empyric-0.2.0/empyric/routines.py
--rw-r--r--   0        0        0     2329 2023-05-17 04:53:19.435384 empyric-0.2.0/empyric/runcard_schema.yaml
--rw-r--r--   0        0        0       16 2022-09-30 05:37:52.005391 empyric-0.2.0/empyric/tests/__init__.py
--rw-r--r--   0        0        0     1420 2023-05-26 05:42:12.137905 empyric-0.2.0/empyric/tests/henon_runcard_example.yaml
--rw-r--r--   0        0        0      639 2022-10-24 21:12:17.723978 empyric-0.2.0/empyric/tests/test_adapter.py
--rw-r--r--   0        0        0     2123 2023-05-22 05:13:53.511443 empyric-0.2.0/empyric/tests/test_experiment.py
--rw-r--r--   0        0        0      637 2023-05-22 04:40:36.449679 empyric-0.2.0/empyric/tests/test_variable.py
--rw-r--r--   0        0        0     8006 2023-05-17 05:28:01.545894 empyric-0.2.0/empyric/tools.py
--rw-r--r--   0        0        0     6359 2023-05-26 05:42:12.138274 empyric-0.2.0/empyric/types.py
--rw-r--r--   0        0        0    16057 2023-05-17 04:53:19.436169 empyric-0.2.0/empyric/variables.py
--rw-r--r--   0        0        0      799 2023-05-26 05:50:15.862611 empyric-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7899 1970-01-01 00:00:00.000000 empyric-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2022-02-05 04:17:18.866045 empyric-0.2.3/LICENSE
+-rw-r--r--   0        0        0     6412 2023-05-31 15:01:11.750049 empyric-0.2.3/README.md
+-rw-r--r--   0        0        0     2312 2023-05-31 15:01:11.751075 empyric-0.2.3/empyric/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-27 14:57:14.109740 empyric-0.2.3/empyric/__main__.py
+-rw-r--r--   0        0        0    38454 2023-05-31 15:01:11.751723 empyric-0.2.3/empyric/adapters.py
+-rw-r--r--   0        0        0       36 2023-03-29 06:16:12.180511 empyric-0.2.3/empyric/collection/__init__.py
+-rw-r--r--   0        0        0     1686 2023-05-31 15:01:11.752149 empyric-0.2.3/empyric/collection/barometers.py
+-rw-r--r--   0        0        0    10912 2023-05-31 15:01:11.752528 empyric-0.2.3/empyric/collection/controllers.py
+-rw-r--r--   0        0        0     8565 2023-05-31 15:01:11.752878 empyric-0.2.3/empyric/collection/generators.py
+-rw-r--r--   0        0        0     1182 2023-05-31 15:01:11.753110 empyric-0.2.3/empyric/collection/humans.py
+-rw-r--r--   0        0        0    10487 2023-05-31 15:01:11.753366 empyric-0.2.3/empyric/collection/instrument.py
+-rw-r--r--   0        0        0     3177 2023-05-31 15:01:11.753753 empyric-0.2.3/empyric/collection/io.py
+-rw-r--r--   0        0        0    17628 2023-05-31 15:01:11.753942 empyric-0.2.3/empyric/collection/multimeters.py
+-rw-r--r--   0        0        0    22234 2023-05-31 15:01:11.754634 empyric-0.2.3/empyric/collection/scopes.py
+-rw-r--r--   0        0        0    28089 2023-05-31 15:01:11.755229 empyric-0.2.3/empyric/collection/sourcemeters.py
+-rw-r--r--   0        0        0     3639 2023-05-31 15:01:11.755459 empyric-0.2.3/empyric/collection/spectrometers.py
+-rw-r--r--   0        0        0     6525 2023-05-31 15:01:11.755664 empyric-0.2.3/empyric/collection/supplies.py
+-rw-r--r--   0        0        0     2167 2023-05-31 15:01:11.755920 empyric-0.2.3/empyric/collection/thermometers.py
+-rw-r--r--   0        0        0     9763 2023-05-31 15:01:11.756218 empyric-0.2.3/empyric/collection/virtual.py
+-rw-r--r--   0        0        0    29892 2023-05-31 15:01:11.756509 empyric-0.2.3/empyric/experiment.py
+-rw-r--r--   0        0        0    37351 2023-05-31 15:01:11.756847 empyric-0.2.3/empyric/graphics.py
+-rw-r--r--   0        0        0      761 2023-05-31 15:01:11.757347 empyric-0.2.3/empyric/instruments.py
+-rw-r--r--   0        0        0    32083 2023-05-31 15:01:11.757721 empyric-0.2.3/empyric/routines.py
+-rw-r--r--   0        0        0     2329 2023-05-17 04:53:19.435384 empyric-0.2.3/empyric/runcard_schema.yaml
+-rw-r--r--   0        0        0       16 2022-09-30 05:37:52.005391 empyric-0.2.3/empyric/tests/__init__.py
+-rw-r--r--   0        0        0     1420 2023-05-27 14:57:14.113113 empyric-0.2.3/empyric/tests/henon_runcard_example.yaml
+-rw-r--r--   0        0        0      634 2023-05-31 15:01:11.758110 empyric-0.2.3/empyric/tests/test_adapter.py
+-rw-r--r--   0        0        0     2122 2023-05-31 15:01:11.758329 empyric-0.2.3/empyric/tests/test_experiment.py
+-rw-r--r--   0        0        0      638 2023-05-31 15:01:11.759672 empyric-0.2.3/empyric/tests/test_variable.py
+-rw-r--r--   0        0        0     8112 2023-05-31 15:01:11.760402 empyric-0.2.3/empyric/tools.py
+-rw-r--r--   0        0        0     6296 2023-05-31 15:01:11.760792 empyric-0.2.3/empyric/types.py
+-rw-r--r--   0        0        0    15879 2023-05-31 15:01:11.761215 empyric-0.2.3/empyric/variables.py
+-rw-r--r--   0        0        0      799 2023-05-31 15:01:11.762859 empyric-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7221 1970-01-01 00:00:00.000000 empyric-0.2.3/PKG-INFO
```

### Comparing `empyric-0.2.0/LICENSE` & `empyric-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `empyric-0.2.0/README.md` & `empyric-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 # Empyric 
 ## A Python Library for Experiment Automation
 
 For more details, [read the docs](https://empyric.readthedocs.io/en/latest/).
 
-Empyric, at its most basic level, is an easy to use Python interface for communication with and controlling scientific instruments, such as digital multimeters, digital oscilloscopes, and power supplies. On top of that is a general purpose experiment-building architecture, which allows the user to combine process control, measurements and data plotting in a highly customizable fashion, using a straightforward "runcard" formalism, which additionally serves the purpose of experiment documentation.
+Empyric, at its most basic level, is an easy-to-use Python interface for communication with and controlling laboratory instruments, such as digital multimeters, oscilloscopes, and power supplies. On top of that is a general purpose experiment-building architecture, which allows the user to combine process control, measurements and data plotting in a highly customizable fashion, using a straightforward "runcard" formalism, which additionally serves the purpose of experiment documentation.
 
-The preferred method of installing Empyric is via pip:
+Empyric can be installed with pip:
 ```commandline
 pip install empyric
 ```
 
 ### Instruments and Adapters
 
 Empyric contains a number of *instruments* with various associated methods of communication, such as serial or GPIB. For example, to remotely control a Keithley 2400 Sourcemeter from your PC, simply import the `Keithley2400` object from the library and instantiate it with its GPIB address:
 
 ```
 from empyric.instruments import Keithley2400
 
 keithley2400 = Keithley2400(1)  # if GPIB address is 1
 
-kiethley2400.set('voltage', 10)
-current = keithley2400.measure('current')
+kiethley2400.set_voltage(10)  # sets output voltage to 10 volts
+current = keithley2400.measure_current()  # measures current in amperes
 ```
 
 Communication with instruments is facilitated through Empyric's library of *adapters*. If you have an instrument that is not in the Empyric library but which uses one of the more common communication protocols (Serial, GPIB, USBTMC, Modbus, etc.), you can still make use of Empyric's adapters, which automatically manage many of the underlying details of the communication backends:
 
 ```
 from empyric.instruments import Instrument
 from empyric.adapters import Modbus
 
 class MyInstrument(Instrument):
 	"""
 	Basic template of an instrument object in Empyric
 	"""
 
-	name = 'My Instrument'
+	name = 'MyInstrument'
 	
 	supported_adapters = ((Modbus, {'baud_rate':115200}),)
 	
-	knobs = ('knob',)
-	meters = ('meter',)
+	knobs = ('some knob',)
+	meters = ('some meter',)
 	
-	def set_knob(self, value):
-		# ... set your knob
+	def set_some_knob(self, value):
+		# set your knob
 	
-	def measure_meter(self):
-		# ... measure your meter
+	def measure_some_meter(self):
+		# measure your meter
 	
 instrument = MyInstrument('COM5::1')  # connect to your instrument
 
-meter_value = instrument.measure_meter()  # take a measurement
+some_meter_value = instrument.measure_some_meter()  # take a measurement
 
 ```
 
 ### Experiments
 
 The real purpose of Empyric is to simplify and standardize construction of an experiment, and automate its execution. The two main elements of an experiment are its *variables* which are controlled and/or measured by your instruments, and *routines* which are the various processes that you run on your controllable variables.
 
-*Variables* come in four flavors: knobs, meters, expressions and parameters. A knob is a variable that you can directly control through an instrument, such as voltage from a power supply. A meter is a variable that you directly measure through an instrument, such as temperature from a thermocouple. In some cases, a meter can be controlled indirectly through a feedback loop. For example, PID temperature controllers provide a temperature knob (the setpoint) as well as a temperature meter (the actual temperature measured with a thermocouple or RTD). An expression is a variable that is evaluated in terms of other experiment variables, such as the power delivered by a power supply being the product of the voltage knob value and the current meter value. A parameter is a user-defined value that is relevant to the experiment, such as a unit conversion factor, a variable setpoint (e.g. used in a routine) or a quantity that must be manually logged.
+*Variables* come in five flavors: knobs, meters, expressions, parameters and remotes. A knob is a variable that you can directly control through an instrument, such as voltage from a power supply. A meter is a variable that you directly measure through an instrument, such as temperature from a thermocouple. In some cases, a meter can be controlled indirectly through a feedback loop. For example, PID temperature controllers provide a temperature knob (the setpoint) as well as a temperature meter (the actual temperature measured with a thermocouple or RTD). An expression is a variable that is evaluated in terms of other experiment variables, such as the power delivered by a power supply being the product of the voltage knob value and the current meter value. A parameter is a user-defined value that is relevant to the experiment, such as a unit conversion factor, a variable setpoint (e.g. used in a routine) or a quantity that must be manually logged. A remote variable is a variable defined in another experiment with a server routine running, that can be read or controlled remotely. A variable's value can be read and set through its `value` property.
 
-Here is an example showing how to define and use experiment variables in Empyric:
+Here is an example showing how to define and use variables in Empyric:
 ```
 from empyric.variables import Knob, Meter, Parameter, Expression
 from empyric.instruments import Keithley2400
 
 keithley2400 = Keithley2400(1)
 
 voltage = Knob(instrument=keithley2400, knob='voltage')
@@ -72,17 +72,16 @@
 power = Expression(expression='V * I / mW', definitions={'V':voltage, 'I':current, 'mW':milliwatt})
 
 voltage.value = 10 # sets the voltage of the Keithley 2400 to 10 V
 
 # Obtain 10 measurements of current, voltage and power sourced by a Keithley 2400
 measurements = [[current.value, voltage.value, power.value] for i in range(10)]
 ```
-Assigning a value to the `value` property of a knob-type variable commands the corresponding instrument to set the associated knob accordingly, and the value is stored in the corresponding attribute of the instrument (`[instrument].[knob]`). Calling the `value` property of a meter-type variable commands the corresponding instrument to record a measurement of the associated meter, and then return the value as well as store it as an attribute of the instrument  (`[instrument].measured_[meter]`). Calling the `value` property of an expression-type variable retrieves the values of the variables that define it from the stored attributes of the corresponding knobs, meters and other expressions; it does not trigger any new measurements. Therefore, for repeated calls, be sure to trigger measurements or retrievals of the values of any defining variables prior to each evaluation of the expression.
 
-*Routines* allow one to define the trajectory that an experiment takes through parameter space over the duration of the experiment. Every routine has a start and end, assigned variables and assigned values. Routines update their associated variables based on a given state, containing the current time (in seconds) and values of all variables. The most basic routine is the `Hold` routine:
+*Routines* allow one to define the trajectory that an experiment takes through parameter space over the duration of the experiment. Every routine has a set of knobs that it updates based on a given state, containing the current time (in seconds) and values of all relevant variables. The most basic routine is the `Set` routine:
 ```
 import time
 
 # ... define knob1 and knob2 as instances of Knob from above
 
 knobs = {'Knob 1': knob1, 'Knob 2': knob2}
 values = [10, 20]
@@ -102,8 +101,8 @@
 	
 	state['Knob 1] = knob1.value
 	state['Knob 2] = knob2.value
 	
 	print(state)  # prints "{'Time': ..., 'Knob 1': 10, 'Knob 2': 20}"
 ```
 
-An *Experiment* monitors a set of variables as a set of routines takes action on them. In Empyric, the `Experiment` object is an iterable that updates routines and records data on each iteration. It also has `start`, `hold` and `stop` methods which initiate/resume the experiment, holds routines while continuing to measure meters, and stops all routines and measurements, respectively. The `terminate` method saves the collected data to a file in the working directory and raises the `StopIteration` exception. An experiment will terminate automatically when all routines are finished. See henon_python_eaxmple.py in the 'examples/Henon Map Experiment' directory to see how a basic experiment is set up as a python script. This particular example uses a virtual instrument (`HenonMapper`), so the only requirement to run it is having Python installed along with the usual scientific packages (numpy, scipy, pandas and matplotlib).
+An *Experiment* monitors a set of variables as a set of routines takes action on them. In Empyric, the `Experiment` object is an iterable that updates routines and records data on each iteration, which has a defined state. It also has `start`, `hold` and `stop` methods which initiate/resume the experiment, holds routines while continuing to measure meters, and stops all routines and measurements, respectively. The `terminate` method saves the collected data to a file in the working directory and raises the `StopIteration` exception. An experiment will terminate automatically when all routines are finished. See henon_python_eaxmple.py in the 'examples/Henon Map Experiment' directory to see how a basic experiment is set up as a python script. This particular example uses a virtual instrument (`HenonMapper`), so the only requirement to run it is having Python installed along with the usual scientific packages (numpy, scipy, pandas and matplotlib).
```

### Comparing `empyric-0.2.0/empyric/adapters.py` & `empyric-0.2.3/empyric/adapters.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,78 +14,71 @@
     handles communication issues.
 
     :param method: (callable) method to be wrapped
     :return: (callable) wrapped method
     """
 
     def wrapped_method(self, *args, validator=None, **kwargs):
-
         if not self.connected:
             raise AdapterError(
-                'Adapter is not connected for instrument '
-                f'at address {self.instrument.address}'
+                "Adapter is not connected for instrument "
+                f"at address {self.instrument.address}"
             )
 
         while self.busy:  # wait for turn to talk to the instrument
             time.sleep(0.05)
 
         self.busy = True  # block other methods from talking to the instrument
 
         # Catch communication errors and either try to repeat communication
         # or reset the connection
         attempts = 0
         reconnects = 0
 
         while reconnects <= self.max_reconnects:
             while attempts < self.max_attempts:
-
                 try:
-
                     response = method(self, *args, **kwargs)
 
                     if validator and not validator(response):
-
-                        if hasattr(response, '__len__') and len(response) > 100:
-                            response = str(response[:50]) \
-                                       + '...' + str(response[-50:])
+                        if hasattr(response, "__len__") and len(response) > 100:
+                            response = str(response[:50]) + "..." + str(response[-50:])
 
                         raise ValueError(
-                            f'invalid response, {response}, '
-                            f'from {method.__name__} method'
+                            f"invalid response, {response}, "
+                            f"from {method.__name__} method"
                         )
 
                     elif attempts > 0 or reconnects > 0:
-                        print('Resolved')
+                        print("Resolved")
 
                     self.busy = False
                     return response
 
                 except BaseException as err:
                     print(
-                        f'Encountered {err} while trying '
-                        f'to talk to {self.instrument.name}'
-                        '\nRetrying...'
+                        f"Encountered {err} while trying "
+                        f"to talk to {self.instrument.name}"
+                        "\nRetrying..."
                     )
                     attempts += 1
 
             # repeats have maxed out, so try reconnecting with the instrument
-            print('Reconnecting...')
+            print("Reconnecting...")
             self.disconnect()
             time.sleep(self.delay)
             self.connect()
 
             attempts = 0
             reconnects += 1
 
         # Getting here means that both repeats
         # and reconnects have been maxed out
         self.busy = False
-        raise AdapterError(
-            f'Unable to communicate with {self.instrument.name}!'
-        )
+        raise AdapterError(f"Unable to communicate with {self.instrument.name}!")
 
     wrapped_method.__doc__ = method.__doc__  # keep method doc string
 
     return wrapped_method
 
 
 class AdapterError(BaseException):
@@ -104,25 +97,23 @@
     #: Maximum number of times to try to reset communications,
     # in the event of a communication error
     max_reconnects = 1
 
     kwargs = []
 
     # Library used by adapter; overwritten in children classes.
-    lib = 'python'
+    lib = "python"
 
     # If upon instantiation no valid library is found for adapter, raise
     # AdapterError with the following message; overwritten in children classes.
-    no_lib_msg = 'no valid library found for adapter; ' \
-                 'check library installation'
+    no_lib_msg = "no valid library found for adapter; " "check library installation"
 
     delay = 0.1  # delay between successive communication attempts
 
     def __init__(self, instrument, **kwargs):
-
         if self.lib is None:
             # determined by class attribute `lib`
             raise AdapterError(self.no_lib_msg)
 
         # general parameters
         self.instrument = instrument
         self.backend = None
@@ -141,21 +132,21 @@
 
     def __del__(self):
         # Try to cleanly close communications when adapters are deleted
         if self.connected:
             try:
                 self.disconnect()
             except BaseException as err:
-                print(f'Error while disconnecting {self.instrument.name}:', err)
+                print(f"Error while disconnecting {self.instrument.name}:", err)
                 pass
 
     # All methods below should be overwritten in child class definitions
 
     def __repr__(self):
-        return 'Adapter'
+        return "Adapter"
 
     def connect(self):
         """
         Establishes communications with the instrument through the appropriate
         backend.
         """
         self.connected = True
@@ -169,34 +160,33 @@
         :param validator: (callable) function that returns True if its input
                           looks right or False if it does not
         :param kwargs: any keyword arguments for the write method
 
         :return: (str) literal 'Success' if write operation is successful
         """
 
-        if hasattr(self, '_write'):
+        if hasattr(self, "_write"):
             return self._write(*args, **kwargs)
         else:
-            raise AttributeError(
-                self.__name__ + " adapter has no _write method")
+            raise AttributeError(self.__name__ + " adapter has no _write method")
 
     @chaperone
     def read(self, *args, validator=None, **kwargs):
         """
         Read an awaiting message.
 
         :param args: any arguments for the read method
         :param validator: (callable) function that returns True if its input
                           looks right or False if it does not
         :param kwargs: any keyword arguments for the read method
 
         :return: instrument response
         """
 
-        if hasattr(self, '_read'):
+        if hasattr(self, "_read"):
             return self._read(*args, **kwargs)
         else:
             raise AttributeError(self.__name__ + " adapter has no _read method")
 
     @chaperone
     def query(self, *args, validator=None, **kwargs):
         """
@@ -206,20 +196,18 @@
         :param validator: (callable) function that returns True if its input
                           looks right or False if it does not
         :param kwargs: any keyword arguments for the query method
 
         :return: instrument response
         """
 
-        if hasattr(self, '_query'):
+        if hasattr(self, "_query"):
             return self._query(*args, **kwargs)
         else:
-            raise AttributeError(
-                self.__name__ + " adapter has no _query method"
-            )
+            raise AttributeError(self.__name__ + " adapter has no _query method")
 
     def disconnect(self):
         """
         Close communication port/channel
         """
         self.connected = False
 
@@ -229,198 +217,182 @@
     Handles communications with serial instruments through either PyVISA or
     PySerial. If both are installed, it defaults to PyVISA.
     """
 
     baud_rate = 9600
     timeout = 0.1
     delay = 0.1
-    parity = 'N'
+    parity = "N"
     stop_bits = 1
-    read_termination = '\n'
-    write_termination = '\r'
+    read_termination = "\n"
+    write_termination = "\r"
 
     kwargs = [
-        'baud_rate', 'timeout', 'delay', 'byte_size', 'parity', 'stop_bits',
+        "baud_rate",
+        "timeout",
+        "delay",
+        "byte_size",
+        "parity",
+        "stop_bits",
     ]
 
     # Get serial library
-    if importlib.util.find_spec('pyvisa'):
-        lib = 'pyvisa'
-    elif importlib.util.find_spec('serial'):
-        lib = 'pyserial'
+    if importlib.util.find_spec("pyvisa"):
+        lib = "pyvisa"
+    elif importlib.util.find_spec("serial"):
+        lib = "pyserial"
     else:
         lib = None
 
-    no_lib_msg = 'No serial library was found! ' \
-                 'Please install either PySerial or PyVISA.'
+    no_lib_msg = (
+        "No serial library was found! " "Please install either PySerial or PyVISA."
+    )
 
     def connect(self):
-
         # First try connecting with PyVISA
-        if self.lib == 'pyvisa':
-
-            pyvisa = importlib.import_module('pyvisa')
+        if self.lib == "pyvisa":
+            pyvisa = importlib.import_module("pyvisa")
 
             self.backend = pyvisa.open_resource(
                 self.instrument.address,
                 baud_rate=self.baud_rate,
                 stop_bits=self.stop_bits,
                 parity=self.parity,
                 timeout=self.timeout,
                 write_termination=self.write_termination,
-                read_terimation=self.read_termination
+                read_terimation=self.read_termination,
             )
 
         # Then try connecting with PySerial
-        elif self.lib == 'pyserial':
-
-            serial = importlib.import_module('serial')
+        elif self.lib == "pyserial":
+            serial = importlib.import_module("serial")
 
             self.backend = serial.Serial(
                 port=self.instrument.address,
                 baudrate=self.baud_rate,
                 stopbits=self.stop_bits,
                 parity=self.parity,
-                timeout=self.timeout
+                timeout=self.timeout,
             )
 
         else:
-            raise AdapterError(f'invalid library specification, {self.lib}')
+            raise AdapterError(f"invalid library specification, {self.lib}")
 
         self.connected = True
 
     def _write(self, message):
-
-        if self.lib == 'pyvisa':
+        if self.lib == "pyvisa":
             self.backend.write(message)
-        elif self.lib == 'pyserial':
+        elif self.lib == "pyserial":
             self.backend.write((message + self.write_termination).encode())
 
         return "Success"
 
     def _read(self, bytes=None, until=None, decode=True):
-
-        if self.lib == 'pyvisa':
+        if self.lib == "pyvisa":
             if bytes:
                 response = self.backend.read_bytes(bytes)
             elif until:
-                response = b''
+                response = b""
                 while until.encode() not in response:
                     response = response + self.backend.read_raw(1)
             else:
                 return self.backend.read(decode=False)  # decoded below
 
-        elif self.lib == 'pyserial':
+        elif self.lib == "pyserial":
             if bytes:
                 response = self.backend.read(bytes)
             elif until:
                 response = self.backend.read_until(until)
             else:
-                response = self.backend.read_until(
-                    self.read_termination.encode()
-                )
+                response = self.backend.read_until(self.read_termination.encode())
 
         else:
-            response = b''
+            response = b""
 
         if decode:
             response = response.decode().strip()
 
         return response
 
     def _query(self, question, bytes=None, until=None, decode=True):
-
         self._write(question)
         time.sleep(self.delay)
         return self._read(bytes=bytes, until=until, decode=decode)
 
     def disconnect(self):
-
-        if self.lib == 'pyvisa':
+        if self.lib == "pyvisa":
             self.backend.clear()
 
-        elif self.lib == 'pyserial':
+        elif self.lib == "pyserial":
             self.backend.reset_input_buffer()
             self.backend.reset_output_buffer()
 
         self.backend.close()
 
         self.connected = False
 
     def __repr__(self):
-        return 'Serial'
+        return "Serial"
 
     @classmethod
-    def list(cls, verbose=True):
+    def list(cls):
         """
         List all connected serial devices
 
         :param verbose: (bool) if True, list of devices will be printed
                         (defaults to True).
 
         :return: (list of str) List of connected serial devices
         """
 
-        if cls.lib == 'pyvisa':
-
-            pyvisa = importlib.import_module('serial')
+        if cls.lib == "pyvisa":
+            pyvisa = importlib.import_module("pyvisa")
             resource_manager = pyvisa.ResourceManager()
 
             devices = resource_manager.list_resources()
 
-            if verbose:
-                print('Connected serial devices (via PyVISA)')
-                print('\n'.join(devices))
-
-        elif cls.lib == 'pyserial':
-
-            list_ports = importlib.import_module(
-                'serial.tools.list_ports'
-            ).comports
+        elif cls.lib == "pyserial":
+            list_ports = importlib.import_module("serial.tools.list_ports").comports
 
             devices = [port.device for port in list_ports()]
 
-            if verbose:
-                print('Connected serial devices (via PySerial)')
-                print('\n'.join(devices))
-
         else:
             raise AdapterError(cls.no_lib_msg)
 
         return devices
 
     @classmethod
     def locate(cls):
         """
         Determine the address of a serial instrument via the
         "unplug-it-then-plug-it-back-in" method.
 
         :return: None (address is printed to console)
         """
 
-        input('Press enter when the instrument is disconnected')
+        input("Press enter when the instrument is disconnected")
 
         other_devices = Serial.list(verbose=False)
 
-        input('Press enter when the instrument is connected')
+        input("Press enter when the instrument is connected")
 
         all_devices = Serial.list(verbose=False)
 
         try:
-
             instrument_address = [
                 device for device in all_devices if device not in other_devices
             ][0]
 
-            print(f'Address: {instrument_address}\n')
+            print(f"Address: {instrument_address}\n")
 
         except IndexError:
-            print('Instrument not found!\n')
+            print("Instrument not found!\n")
 
-        again = 'y' in input('Try again? [y/n]').lower()
+        again = "y" in input("Try again? [y/n]").lower()
         if again:
             Serial.locate()
 
 
 class GPIB(Adapter):
     """
     Handles communications with GPIB instruments through either PyVISA,
@@ -444,121 +416,112 @@
         10: 300e-3,
         11: 1,
         12: 3,
         13: 10,
         14: 30,
         15: 100,
         16: 300,
-        17: 1000
+        17: 1000,
     }
 
-    kwargs = ['prologix_address']
+    kwargs = ["prologix_address"]
 
     prologix_address = None
     prologix_controllers = {}
 
     delay = 0.05
     _timeout = None
 
     # Get GPIB library
-    if importlib.util.find_spec('pyvisa'):
-        lib = 'pyvisa'
-    elif importlib.util.find_spec('gpib_ctypes'):
-        lib = 'linux-gpib'
+    if importlib.util.find_spec("pyvisa"):
+        lib = "pyvisa"
+    elif importlib.util.find_spec("gpib_ctypes"):
+        lib = "linux-gpib"
     else:
-        if importlib.util.find_spec('serial'):
-            lib = 'prologix-gpib'
+        if importlib.util.find_spec("serial"):
+            lib = "prologix-gpib"
 
-    no_lib_msg = 'No valid library found for GPIB adapters!' \
-                 'Please install PyVISA (with GPIB drivers), Linux-GPIB, or' \
-                 'use a Prologix GPIB-USB or GPIB-ETHERNET adapter ' \
-                 '(requires PySerial)'
+    no_lib_msg = (
+        "No valid library found for GPIB adapters!"
+        "Please install PyVISA (with GPIB drivers), Linux-GPIB, or"
+        "use a Prologix GPIB-USB or GPIB-ETHERNET adapter "
+        "(requires PySerial)"
+    )
 
     def __init__(self, instrument, **kwargs):
         super().__init__(instrument, **kwargs)
         self._descr = None
 
     @property
     def timeout(self):
         return self._timeout
 
     @timeout.setter
     def timeout(self, timeout):
-
         if self.connected:
-            if self.lib == 'pyvisa' or self.lib == 'prologix-gpib':
+            if self.lib == "pyvisa" or self.lib == "prologix-gpib":
                 # pyvisa records timeouts in milliseconds
                 if timeout is None:
                     self.backend.timeout = None
                 else:
                     self.backend.timeout = timeout * 1000
                 self._timeout = timeout
-            elif self.lib == 'linux-gpib':
+            elif self.lib == "linux-gpib":
                 self._timeout = self._linux_gpib_set_timeout(timeout)
-            elif self.lib == 'prologix-gpib':
+            elif self.lib == "prologix-gpib":
                 self.backend.timeout = timeout
                 self._timeout = timeout
         else:
             self._timeout = None
 
     def connect(self):
-
         if self.prologix_address is not None:
-            self.lib = 'prologix-gpib'
-
-        if self.lib == 'pyvisa':
+            self.lib = "prologix-gpib"
 
-            visa = importlib.import_module('pyvisa')
+        if self.lib == "pyvisa":
+            visa = importlib.import_module("pyvisa")
 
             manager = visa.ResourceManager()
 
             full_address = None
             for address in manager.list_resources():
-
                 instrument_address = str(self.instrument.address)
 
-                address_format = 'GPIB[0-9]::' + instrument_address + '::INSTR'
+                address_format = "GPIB[0-9]::" + instrument_address + "::INSTR"
 
-                address_match = re.match(
-                    address_format,
-                    address
-                )
+                address_match = re.match(address_format, address)
 
                 if address_match:
                     full_address = address
 
             if full_address:
                 self.backend = manager.open_resource(full_address)
             else:
                 AdapterError(
-                    'GPIB device at address '
-                    f'{self.instrument.address} not found!'
+                    "GPIB device at address " f"{self.instrument.address} not found!"
                 )
 
-        elif self.lib == 'linux-gpib':
-            self.backend = importlib.import_module('gpib')
+        elif self.lib == "linux-gpib":
+            self.backend = importlib.import_module("gpib")
 
-            self._descr = self.backend.dev(
-                0, self.instrument.address, 0, 9, 1, 0
-            )
-
-        elif self.lib == 'prologix-gpib':
+            self._descr = self.backend.dev(0, self.instrument.address, 0, 9, 1, 0)
 
+        elif self.lib == "prologix-gpib":
             if self.prologix_address is None:
                 raise AdapterError(
-                    'trying to connect to Prologix GPIB adapter but no address '
-                    'was provided (prologix_address argument was not set); '
-                    'must be either an IP address (for Prologix GPIB-LAN) or '
-                    'serial port (for Prologix GPIB-USB)'
+                    "trying to connect to Prologix GPIB adapter but no address "
+                    "was provided (prologix_address argument was not set); "
+                    "must be either an IP address (for Prologix GPIB-LAN) or "
+                    "serial port (for Prologix GPIB-USB)"
                 )
 
             if self.prologix_address in GPIB.prologix_controllers:
                 self.backend = GPIB.prologix_controllers[self.prologix_address]
             else:
-                if re.match('\d+\.\d+\.\d+\.\d+', self.prologix_address):
+                if re.match("\d+\.\d+\.\d+\.\d+", self.prologix_address):
                     self.backend = PrologixGPIBLAN(self.prologix_address)
                 else:
                     self.backend = PrologixGPIBUSB(self.prologix_address)
 
                 GPIB.prologix_controllers[self.prologix_address] = self.backend
 
             if self.instrument.address not in self.backend.devices:
@@ -570,80 +533,76 @@
                 f"'linux-gpib' or 'prologix-gpib'. If using a Prologix GPIB "
                 "adapter, its 'prologix address' argument must be specified"
             )
 
         self.connected = True
 
     def _write(self, message):
-
-        if self.lib == 'pyvisa':
+        if self.lib == "pyvisa":
             self.backend.write(message)
-        elif self.lib == 'linux-gpib':
+        elif self.lib == "linux-gpib":
             self.backend.write(self._descr, message)
-        elif self.lib == 'prologix-gpib':
+        elif self.lib == "prologix-gpib":
             self.backend.write(message, address=self.instrument.address)
 
         return "Success"
 
     def _read(self, bytes=1024):
-
-        if self.lib == 'pyvisa':
+        if self.lib == "pyvisa":
             return self.backend.read()
-        elif self.lib == 'linux-gpib':
+        elif self.lib == "linux-gpib":
             return self.backend.read(self._descr, bytes).decode()
-        elif self.lib == 'prologix-gpib':
+        elif self.lib == "prologix-gpib":
             return self.backend.read(address=self.instrument.address)
 
     def _query(self, question):
         self._write(question)
         time.sleep(self.delay)
         return self._read()
 
     def _linux_gpib_set_timeout(self, timeout):
-
         if timeout is None:
             self.backend.timeout(self.descr, 0)
             return None
         else:
             for index, allowed_timeout in self.linux_gpib_timeouts.items()[1:]:
                 if allowed_timeout >= timeout:
                     self.backend.timeout(self.descr, index)
                     break
 
             return allowed_timeout
 
     def disconnect(self):
-
-        if self.lib == 'pyvisa':
+        if self.lib == "pyvisa":
             self.backend.clear()
             self.backend.close()
-        elif self.lib == 'linux-gpib':
+        elif self.lib == "linux-gpib":
             self.backend.clear(self._descr)
             self.backend.close(self._descr)
-        elif self.lib == 'prologix-gpib':
-
+        elif self.lib == "prologix-gpib":
             # clear the instrument buffers
-            self.backend.write('clr', to_controller=True,
-                               address=self.instrument.address)
+            self.backend.write(
+                "clr", to_controller=True, address=self.instrument.address
+            )
 
             # return instrument to local control
-            self.backend.write('loc', to_controller=True)
+            self.backend.write("loc", to_controller=True)
 
             # unlink device from controller
             self.backend.devices.remove(self.instrument.address)
 
             # if no more devices are connected to the controller, close it
             if len(self.backend.devices) == 0:
                 self.backend.close()
                 GPIB.prologix_controllers.pop(self.prologix_address)
 
         self.connected = False
 
     def __repr__(self):
-        return 'GPIB'
+        return "GPIB"
 
 
 class PrologixGPIBUSB:
     """
     Wraps serial communications with the Prologix GPIB-USB adapter unit.
     """
 
@@ -652,79 +611,76 @@
         return self.serial_port.timeout
 
     @timeout.setter
     def timeout(self, timeout):
         self.serial_port.timeout = timeout
 
     def __init__(self, port):
-
         try:
-            serial = importlib.import_module('serial')
+            serial = importlib.import_module("serial")
         except ImportError:
             raise AdapterError(
-                'Please install the PySerial library '
-                'to connect a Prologix GPIB-USB adapter.'
+                "Please install the PySerial library "
+                "to connect a Prologix GPIB-USB adapter."
             )
 
         self.serial_port = serial.Serial(port=port, timeout=1)
 
         # set adapter to "controller" mode
-        self.write('mode 1', to_controller=True)
+        self.write("mode 1", to_controller=True)
 
         # instruments talk only when requested to
-        self.write('auto 0', to_controller=True)
+        self.write("auto 0", to_controller=True)
 
         # set timeout to 0.5 seconds
-        self.write('read_tmo_ms 500', to_controller=True)
+        self.write("read_tmo_ms 500", to_controller=True)
 
         # Do not append CR or LF to messages
-        self.write('eos 3', to_controller=True)
+        self.write("eos 3", to_controller=True)
 
         # Assert EOI with last byte to indicate end of data
-        self.write('eoi 1', to_controller=True)
+        self.write("eoi 1", to_controller=True)
 
         # Append CR to responses from instruments to indicate message
         # termination
-        self.write('eot_char 13', to_controller=True)
-        self.write('eot_enable 1', to_controller=True)
+        self.write("eot_char 13", to_controller=True)
+        self.write("eot_enable 1", to_controller=True)
 
         self.address = None
         self.devices = []
 
     def write(self, message, to_controller=False, address=None):
-
         if address and address != self.address:
-            self.write(f'addr {address}', to_controller=True)
+            self.write(f"addr {address}", to_controller=True)
             self.address = address
 
             if address not in self.devices:
                 self.devices.append(address)
 
-        proper_message = message.encode() + b'\r'
+        proper_message = message.encode() + b"\r"
 
         if to_controller:
-            proper_message = b'++' + proper_message
+            proper_message = b"++" + proper_message
 
         self.serial_port.write(proper_message)
 
         return "Success"
 
     def read(self, from_controller=False, address=None):
-
         if address and address != self.address:
-            self.write(f'addr {address}', to_controller=True)
+            self.write(f"addr {address}", to_controller=True)
             self.address = address
 
             if address not in self.devices:
                 self.devices.append(address)
 
         if not from_controller:
-            self.write(f'read eoi', to_controller=True)
+            self.write(f"read eoi", to_controller=True)
 
-        response = self.serial_port.read_until(b'\r').decode().strip()
+        response = self.serial_port.read_until(b"\r").decode().strip()
 
         return response
 
     def close(self):
         self.serial_port.close()
 
 
@@ -742,71 +698,68 @@
         return self.socket.gettimeout()
 
     @timeout.setter
     def timeout(self, timeout):
         self.socket.settimeout(timeout)
 
     def __init__(self, ip_address):
-
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
         self.socket.connect((ip_address, 1234))
 
         self.socket.settimeout(1)
 
         # set adapter to "controller" mode
-        self.write('mode 1', to_controller=True)
+        self.write("mode 1", to_controller=True)
 
         # instruments talk only when requested to
-        self.write('auto 0', to_controller=True)
+        self.write("auto 0", to_controller=True)
 
         # set timeout to 0.5 seconds
-        self.write('read_tmo_ms 500', to_controller=True)
+        self.write("read_tmo_ms 500", to_controller=True)
 
         # Do not append CR or LF to messages
-        self.write('eos 3', to_controller=True)
+        self.write("eos 3", to_controller=True)
 
         # Assert EOI with last byte to indicate end of data
-        self.write('eoi 1', to_controller=True)
+        self.write("eoi 1", to_controller=True)
 
         # Append CR to responses from instruments to indicate message
         # termination
-        self.write('eot_char 13', to_controller=True)
-        self.write('eot_enable 1', to_controller=True)
+        self.write("eot_char 13", to_controller=True)
+        self.write("eot_enable 1", to_controller=True)
 
         self.devices = []
         self.address = None
 
     def write(self, message, to_controller=False, address=None):
-
         if address and address != self.address:
-            self.write(f'addr {address}', to_controller=True)
+            self.write(f"addr {address}", to_controller=True)
             self.address = address
 
             if address not in self.devices:
                 self.devices.append(address)
 
         if to_controller:
-            message = '++' + message
+            message = "++" + message
 
         write_to_socket(self.socket, message)
 
         return "Success"
 
     def read(self, from_controller=False, address=None):
-
         if address and address != self.address:
-            self.write(f'addr {address}', to_controller=True)
+            self.write(f"addr {address}", to_controller=True)
             self.address = address
 
             if address not in self.devices:
                 self.devices.append(address)
 
         if not from_controller:
-            self.write(f'read eoi', to_controller=True)
+            self.write(f"read eoi", to_controller=True)
 
         return read_from_socket(self.socket)
 
     def close(self):
         self.socket.shutdown(socket.SHUT_RDWR)
         self.socket.close()
 
@@ -815,52 +768,45 @@
     """
     Handles communications with pure USB instruments through PyVISA or USBTMC.
     """
 
     timeout = 0.5
 
     # Get USB library
-    if importlib.util.find_spec('pyvisa'):
-        lib = 'pyvisa'
-    elif importlib.util.find_spec('usbtmc'):
-        lib = 'usbtmc'
+    if importlib.util.find_spec("pyvisa"):
+        lib = "pyvisa"
+    elif importlib.util.find_spec("usbtmc"):
+        lib = "usbtmc"
     else:
         lib = None
 
-    no_lib_msg = 'No USB library was found! ' \
-                 'Please install either PyVISA or USBTMC.'
+    no_lib_msg = "No USB library was found! " "Please install either PyVISA or USBTMC."
 
     def connect(self):
-
         serial_number = str(self.instrument.address)
 
-        if self.lib == 'pyvisa':
-
-            visa = importlib.import_module('pyvisa')
+        if self.lib == "pyvisa":
+            visa = importlib.import_module("pyvisa")
 
             manager = visa.ResourceManager()
 
             for address in manager.list_resources():
                 if serial_number in address:
                     self.backend = manager.open_resource(
-                        address,
-                        open_timeout=self.timeout
+                        address, open_timeout=self.timeout
                     )
                     self.backend.timeout = self.timeout
 
-        elif self.lib == 'usbtmc':
+        elif self.lib == "usbtmc":
+            usbtmc = importlib.import_module("usbtmc")
 
-            usbtmc = importlib.import_module('usbtmc')
-
-            self.backend = usbtmc.Instrument(
-                'USB::' + serial_number + '::INSTR'
-            )
+            self.backend = usbtmc.Instrument("USB::" + serial_number + "::INSTR")
 
         else:
-            raise AdapterError(f'invalid library specification, {self.lib}')
+            raise AdapterError(f"invalid library specification, {self.lib}")
 
         self.connected = True
 
     def _write(self, message):
         self.backend.write(message)
         return "Success"
 
@@ -869,187 +815,176 @@
 
     def _query(self, question):
         self._write(question)
         time.sleep(self.delay)
         return self._read()
 
     def disconnect(self):
-
         self.backend.close()
 
         self.connected = False
 
     def __repr__(self):
-        return 'USB'
+        return "USB"
 
 
 class Socket(Adapter):
     """
     Handles communications between sockets using Python's built-in socket module
     """
 
     ip_address = None
     port = None
 
-    read_termination = '\r'
-    write_termination = '\r'
+    read_termination = "\r"
+    write_termination = "\r"
     timeout = 1
 
-    kwargs = ['read_termination', 'write_termination', 'timeout']
+    kwargs = ["read_termination", "write_termination", "timeout"]
 
     def connect(self):
-
         if self.connected:
             self.disconnect()
 
         self.backend = socket.socket()
 
         self.backend.settimeout(self.timeout)
 
         address = self.instrument.address
-        remote_ip_address, remote_port = address.split('::')
+        remote_ip_address, remote_port = address.split("::")
 
         self.backend.connect((remote_ip_address, int(remote_port)))
 
         self.connected = True
 
     def _write(self, message):
         write_to_socket(
-            self.backend, message, termination=self.write_termination,
-            timeout=self.timeout
+            self.backend,
+            message,
+            termination=self.write_termination,
+            timeout=self.timeout,
         )
 
-        return 'Success'
+        return "Success"
 
     def _read(self, **kwargs):
-
-        termination = kwargs.pop('termination', self.read_termination)
-        timeout = kwargs.pop('timeout', self.timeout)
+        termination = kwargs.pop("termination", self.read_termination)
+        timeout = kwargs.pop("timeout", self.timeout)
 
         return read_from_socket(
-            self.backend,
-            termination=termination,
-            timeout=timeout,
-            **kwargs
+            self.backend, termination=termination, timeout=timeout, **kwargs
         )
 
     def _query(self, question, **kwargs):
-
         self._write(question)
         return self._read(**kwargs)
 
     def disconnect(self):
-
         # Clear out any unread messages
         unread = self._read(decode=False, nbytes=np.inf)
         while unread:
             unread = self._read(decode=False, nbytes=np.inf)
 
         self.backend.shutdown(socket.SHUT_RDWR)
         self.backend.close()
 
         self.connected = False
 
     def __repr__(self):
-        return 'Socket'
+        return "Socket"
 
 
 class ModbusSerial(Adapter):
     """
     (TO BE REMOVED)
 
     Handles communications with modbus serial instruments through the
     Minimal ModbusSerial package
     """
 
     # Common defaults
-    slave_mode = 'rtu'
+    slave_mode = "rtu"
     baud_rate = 38400
     timeout = 0.05
     byte_size = 8
     stop_bits = 1
-    parity = 'N'
+    parity = "N"
     delay = 0.05
 
-    kwargs = [
-        'close_port_after_each_call', 'slave_mode', 'byte_order'
-    ]
+    kwargs = ["close_port_after_each_call", "slave_mode", "byte_order"]
 
     # For traffic control of modbus adapters using the same serial ports
     adapters = {}
 
     _busy = False
 
     # Get Minimal Modbus library
-    if importlib.util.find_spec('minimalmodbus'):
-        lib = 'minimalmodbus'
+    if importlib.util.find_spec("minimalmodbus"):
+        lib = "minimalmodbus"
     else:
         lib = None
 
-    no_lib_msg = 'No ModbusSerial library was found! ' \
-                 'Please install the minimalmodbus library'
+    no_lib_msg = (
+        "No ModbusSerial library was found! " "Please install the minimalmodbus library"
+    )
 
     @property
     def busy(self):
-        return bool(sum([
-            adapter._busy
-            for adapter in ModbusSerial.adapters.get(self.port, [])
-        ]))
+        return bool(
+            sum([adapter._busy for adapter in ModbusSerial.adapters.get(self.port, [])])
+        )
 
     @busy.setter
     def busy(self, busy):
         self._busy = busy
 
     def __repr__(self):
-        return 'ModbusSerial'
+        return "ModbusSerial"
 
     def connect(self):
-
-        minimal_modbus = importlib.import_module('minimalmodbus')
+        minimal_modbus = importlib.import_module("minimalmodbus")
 
         # Get port and channel
-        self.port, self.channel = self.instrument.address.split('::')
+        self.port, self.channel = self.instrument.address.split("::")
 
         if self.port in ModbusSerial.adapters:
             ModbusSerial.adapters[self.port].append(self)
         else:
             ModbusSerial.adapters[self.port] = [self]
 
         # Handshake with instrument
         self.backend = minimal_modbus.Instrument(
-            self.port,
-            int(self.channel),
-            mode=self.slave_mode
+            self.port, int(self.channel), mode=self.slave_mode
         )
 
         self.backend.serial.baudrate = self.baud_rate
         self.backend.serial.timeout = self.timeout
         self.backend.serial.bytesize = self.byte_size
         self.backend.serial.parity = self.parity
         self.backend.serial.stopbits = self.stop_bits
         self.backend.close_port_after_each_call = True
         time.sleep(self.delay)
 
         self.connected = True
 
-    def _write(self, register, message, dtype='uint16', byte_order=0):
-        if dtype == 'uint16':
+    def _write(self, register, message, dtype="uint16", byte_order=0):
+        if dtype == "uint16":
             self.backend.write_register(register, message)
-        elif dtype == 'float':
+        elif dtype == "float":
             self.backend.write_float(register, message, byteorder=byte_order)
         time.sleep(self.delay)
 
         return "Success"
 
-    def _read(self, register, dtype='uint16', byte_order=0):
+    def _read(self, register, dtype="uint16", byte_order=0):
         self.backend.serial.timeout = self.timeout
 
-        if dtype == 'uint16':
+        if dtype == "uint16":
             return self.backend.read_register(register)
-        elif dtype == 'float':
+        elif dtype == "float":
             return self.backend.read_float(register, byteorder=byte_order)
 
     def disconnect(self):
         if not self.backend.close_port_after_each_call:
             self.backend.serial.close()
         self.connected = False
 
@@ -1061,115 +996,113 @@
 class Modbus(Adapter):
     """
     Handles communication with instruments via the Modbus communication
     protocol, over either TCP or serial ports, using PyModbus.
     """
 
     kwargs = (
-        'slave id',
-        'byte order',
-        'word order',
-
-        'baud rate',
-        'timeout',
-        'byte size',
-        'stop bits',
-        'parity',
-        'delay'
+        "slave id",
+        "byte order",
+        "word order",
+        "baud rate",
+        "timeout",
+        "byte size",
+        "stop bits",
+        "parity",
+        "delay",
     )
 
     slave_id = 0
     # Byte and word order is either little-endian (<) or big-endian (>)
-    byte_order = '>'
-    word_order = '>'
+    byte_order = ">"
+    word_order = ">"
 
     types = [
-        '8bit_uint', '16bit_uint', '32bit_uint', '64bit_uint',
-        '8bit_int', '16bit_int', '32bit_int', '64bit_int',
-        '16bit_float', '32bit_float', '64bit_float',
+        "8bit_uint",
+        "16bit_uint",
+        "32bit_uint",
+        "64bit_uint",
+        "8bit_int",
+        "16bit_int",
+        "32bit_int",
+        "64bit_int",
+        "16bit_float",
+        "32bit_float",
+        "64bit_float",
     ]
 
     baud_rate = 19200
     timeout = 0.05
     byte_size = 8
     stop_bits = 1
-    parity = 'N'
+    parity = "N"
     delay = 0.05
 
     _protocol = None
     _serial_adapters = {}  # for Modbus Serial
 
     # Locate PyModbus library
-    if importlib.util.find_spec('pymodbus'):
-        lib = 'pymodbus'
+    if importlib.util.find_spec("pymodbus"):
+        lib = "pymodbus"
     else:
         lib = None
 
     @property
     def busy(self):
-
-        if self._protocol == 'Serial':
-            return bool(sum([
-                adapter._busy
-                for adapter in Modbus.adapters.get(self.port, [])
-            ]))
+        if self._protocol == "Serial":
+            return bool(
+                sum([adapter._busy for adapter in Modbus.adapters.get(self.port, [])])
+            )
         else:
             return self._busy
 
     @busy.setter
     def busy(self, busy):
         self._busy = busy
 
     def connect(self):
-
-        client = importlib.import_module('.client', package='pymodbus')
+        client = importlib.import_module(".client", package="pymodbus")
 
         # Get port (Serial) or address & port (TCP)
-        address = self.instrument.address.split('::')
-
-        if re.match('\d+\.\d+\.\d+\.\d+', address[0]):
+        address = self.instrument.address.split("::")
 
+        if re.match("\d+\.\d+\.\d+\.\d+", address[0]):
             # Modbus TCP
-            self._protocol = 'TCP'
+            self._protocol = "TCP"
 
             if len(address) == 1:
                 address.append(502)  # standard Modbus TCP port
 
-            self.backend = client.ModbusTcpClient(
-                host=address[0],
-                port=int(address[1])
-            )
+            self.backend = client.ModbusTcpClient(host=address[0], port=int(address[1]))
 
         else:
-
             # Modbus Serial
-            self._protocol = 'Serial'
+            self._protocol = "Serial"
 
             if len(address) == 1:
                 raise ValueError(
-                    'Modbus over serial requires both the '
-                    'serial port address and slave address'
+                    "Modbus over serial requires both the "
+                    "serial port address and slave address"
                 )
 
             if address[0] in Modbus._serial_adapters:
                 ModbusSerial.adapters[address[0]].append(self)
             else:
-
                 ModbusSerial.adapters[self.port] = [self]
 
                 self.backend = client.ModbusSerialClient(
                     address=address[0],
                     baudrate=self.baud_rate,
                     bytesize=self.byte_size,
                     parity=self.parity,
                     stopbits=self.stop_bits,
                 )
 
         # Get data reading/writing utility classes
-        payload_module = importlib.import_module('.payload', package='pymodbus')
+        payload_module = importlib.import_module(".payload", package="pymodbus")
 
         # Utility for encoding data
         self._builder_cls = payload_module.BinaryPayloadBuilder
 
         # Utility for decoding data
         self._decoder_cls = payload_module.BinaryPayloadDecoder
 
@@ -1183,64 +1116,62 @@
         The Modbus data type for decoding registers is specified by the `_type`
         argument. Valid values for `_type` are listed in the `_types` attribute.
         """
 
         values = np.array([values]).flatten()
 
         if func_code not in [5, 15, 6, 16]:
-            raise ValueError(f'invalid Modbus function code {func_code}')
+            raise ValueError(f"invalid Modbus function code {func_code}")
 
         if _type and _type not in self.types:
             raise TypeError(
-                'invalid _type argument; must be one of:\n' + ', '.join(
-                    self.types
-                )
+                "invalid _type argument; must be one of:\n" + ", ".join(self.types)
             )
 
-        if '5' in str(func_code):
+        if "5" in str(func_code):
             # Write coils
 
             bool_values = [bool(value) for value in values]
 
             response = self.backend.write_coils(
                 address, bool_values, slave=self.slave_id
             )
 
             if response.function_code == 15:
-                return 'Success'
+                return "Success"
             else:
                 raise AdapterError(
-                    f'error writing to coil(s) on {self.instrument.name}'
+                    f"error writing to coil(s) on {self.instrument.name}"
                 )
 
         else:
             # Write registers
 
             if _type is None:
-                _type = '16bit_uint'
+                _type = "16bit_uint"
 
             builder = self._builder_cls(
                 byteorder=self.byte_order, wordorder=self.word_order
             )
 
             for value in values:
-                builder.__getattribute__('add_'+_type)(value)
+                builder.__getattribute__("add_" + _type)(value)
 
             register_values = builder.to_registers()
 
             response = self.backend.write_registers(
                 address, register_values, slave=self.slave_id
             )
 
             if response.function_code == 16:
-                return 'Success'
+                return "Success"
             else:
                 raise AdapterError(
-                    f'error writing to register(s) on {self.instrument.name} '
-                    'for writing coils/registers'
+                    f"error writing to register(s) on {self.instrument.name} "
+                    "for writing coils/registers"
                 )
 
     def _read(self, func_code, address, count=1, _type=None):
         """
         Read from coils (func_code = 1), discrete inputs (func_code = 2),
         holding registers (func_code = 3), or input registers (func_code = 4).
 
@@ -1248,16 +1179,15 @@
         (`func_code`) and address; the data can be converted to the desired
         data type (`_type` = `int` or `float`). Multiple sequential addresses
         are read by specifying the count.
         """
 
         if _type and _type not in self.types:
             raise TypeError(
-                'invalid _type argument; must be one of:\n'
-                ', '.join(self.types)
+                "invalid _type argument; must be one of:\n" ", ".join(self.types)
             )
 
         # Enumerate modbus read functions
         read_functions = {
             1: self.backend.read_coils,
             2: self.backend.read_discrete_inputs,
             3: self.backend.read_holding_registers,
@@ -1285,64 +1215,62 @@
                 address, count=count, slave=self.slave_id
             ).registers
 
             decoder = self._decoder_cls.fromRegisters(
                 registers, byteorder=self.byte_order, wordorder=self.word_order
             )
 
-            n_values = int(16 * count / (int(_type.split('bit')[0])))
+            n_values = int(16 * count / (int(_type.split("bit")[0])))
 
             values = [
-                decoder.__getattribute__('decode_' + _type)()
-                for _ in range(n_values)
+                decoder.__getattribute__("decode_" + _type)() for _ in range(n_values)
             ]
 
             if len(values) == 1:
                 return values[0]
             else:
                 return values
 
         else:
             # Invalid function code
             raise ValueError(
-                f'invalid Modbus function code {func_code} for '
-                'reading coils/registers'
+                f"invalid Modbus function code {func_code} for "
+                "reading coils/registers"
             )
 
     def _query(self, *args, **kwargs):
         """Alias of `_read` method"""
         return self._read(*args, **kwargs)
 
     def disconnect(self):
-
         self.backend.close()
 
 
 class Phidget(Adapter):
     """
     Handles communications with Phidget devices
     """
 
     delay = 0.2
     timeout = 5
 
-    if importlib.util.find_spec('Phidget22'):
-        lib = 'phidget'
+    if importlib.util.find_spec("Phidget22"):
+        lib = "phidget"
     else:
         lib = None
 
-    no_lib_msg = 'Phidget library was not found! ' \
-                 'Please install (pip[3] install Phidget22).'
+    no_lib_msg = (
+        "Phidget library was not found! " "Please install (pip[3] install Phidget22)."
+    )
 
     def __repr__(self):
-        return 'Phidget'
+        return "Phidget"
 
     def connect(self):
-
-        address_parts = self.instrument.address.split('::')
+        address_parts = self.instrument.address.split("::")
         address_parts = [int(part) for part in address_parts]
 
         serial_number = address_parts[0]
 
         self.PhidgetException = importlib.import_module(
             "Phidget22.PhidgetException"
         ).PhidgetException
@@ -1359,25 +1287,28 @@
 
         self.backend.openWaitForAttachment(1000 * self.timeout)
 
         self.connected = True
         self.busy = False
 
     def _write(self, parameter, value):
-        self.backend.__getattribute__('set' + parameter)(value)
+        self.backend.__getattribute__("set" + parameter)(value)
         return "Success"
 
     def _query(self, parameter):
-        return self.backend.__getattribute__('get' + parameter)()
+        return self.backend.__getattribute__("get" + parameter)()
 
     def disconnect(self):
         self.backend.close()
         self.connected = True
 
 
-supported = {key: value for key, value in vars().items()
-             if type(value) is type and issubclass(value, Adapter)}
+supported = {
+    key: value
+    for key, value in vars().items()
+    if type(value) is type and issubclass(value, Adapter)
+}
 
 kwargs = []
 for cls in supported.values():
     for kwarg in cls.kwargs:
         kwargs.append(kwarg)
```

### Comparing `empyric-0.2.0/empyric/collection/controllers.py` & `empyric-0.2.3/empyric/collection/controllers.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,48 +4,45 @@
 
 
 class OmegaCN7500(Instrument):
     """
     Omega model CN7500 PID temperature controller
     """
 
-    name = 'OmegaCN7500'
+    name = "OmegaCN7500"
 
     supported_adapters = (
-        (ModbusSerial, {'slave_mode': 'rtu',
-                  'baud_rate': 38400,
-                  'parity': 'N',
-                  'delay': 0.2}),
+        (
+            ModbusSerial,
+            {"slave_mode": "rtu", "baud_rate": 38400, "parity": "N", "delay": 0.2},
+        ),
     )
 
     knobs = (
-        'output',
-        'setpoint',
-        'proportional band',
-        'integration time',
-        'derivative time'
+        "output",
+        "setpoint",
+        "proportional band",
+        "integration time",
+        "derivative time",
     )
 
-    meters = (
-        'temperature',
-        'power'
-    )
+    meters = ("temperature", "power")
 
     @setter
     def set_output(self, state: Toggle):
         if state == ON:
             # turn on output & start PID control
             self.backend.write_bit(0x814, 1)
         elif state == OFF:
             # turn off output & stop PID control
             self.backend.write_bit(0x814, 0)
 
     @setter
     def set_setpoint(self, setpoint: Float):
-        self.write(0x1001, int(10*setpoint))
+        self.write(0x1001, int(10 * setpoint))
 
     @getter
     def get_setpoint(self) -> Float:
         return self.read(0x1001) / 10
 
     @setter
     def set_proportional_band(self, P: Integer):
@@ -53,27 +50,27 @@
 
     @getter
     def get_proportional_band(self) -> Integer:
         return self.read(0x1009)
 
     @setter
     def set_integration_time(self, Ti: Integer):
-        self.write(0x100c, Ti)
+        self.write(0x100C, Ti)
 
     @getter
     def get_integration_time(self) -> Integer:
-        return self.read(0x100c)
+        return self.read(0x100C)
 
     @setter
     def set_derivative_time(self, Td: Integer):
-        self.write(0x100b, Td)
+        self.write(0x100B, Td)
 
     @getter
     def get_derivative_time(self) -> Integer:
-        return self.read(0x100b)
+        return self.read(0x100B)
 
     @measurer
     def measure_temperature(self) -> Float:
         return self.read(0x1000) / 10
 
     @measurer
     def measure_power(self) -> Float:
@@ -83,62 +80,54 @@
 class OmegaPlatinum(Instrument):
     """
     Omega Platinum series PID controller
     """
 
     name = "OmegaPlatinum"
 
-    supported_adapters = (
-        (ModbusSerial, {
-            'baud_rate': 19200,
-            'parity': 'O'
-        }),
-    )
+    supported_adapters = ((ModbusSerial, {"baud_rate": 19200, "parity": "O"}),)
 
     knobs = (
-        'setpoint',
-        'autotune',
-        'output',
-        'tc type',
+        "setpoint",
+        "autotune",
+        "output",
+        "tc type",
     )
 
-    meters = (
-        'temperature',
-        'power'
-    )
+    meters = ("temperature", "power")
 
     TC_map = {
-        'K': 1,
-        'J': 0,
-        'T': 2,
-        'E': 3,
-        'N': 4,
-        'R': 6,
-        'S': 7,
-        'B': 8,
-        'C': 9,
+        "K": 1,
+        "J": 0,
+        "T": 2,
+        "E": 3,
+        "N": 4,
+        "R": 6,
+        "S": 7,
+        "B": 8,
+        "C": 9,
     }
 
     inverse_TC_map = {v: k for k, v in TC_map.items()}
 
     @measurer
     def measure_temperature(self) -> Float:
-        return self.read(0x0280, dtype='float')
+        return self.read(0x0280, dtype="float")
 
     @measurer
     def measure_power(self) -> Float:
-        return self.read(0x022A, dtype='float')
+        return self.read(0x022A, dtype="float")
 
     @setter
     def set_setpoint(self, setpoint: Float):
-        self.write(0x02E2, setpoint, dtype='float')
+        self.write(0x02E2, setpoint, dtype="float")
 
     @getter
     def get_setpoint(self) -> Float:
-        return self.read(0x02E2, dtype='float')
+        return self.read(0x02E2, dtype="float")
 
     @setter
     def set_autotune(self, state: Toggle):
         if state == ON:
             self.write(0x0243, 1)
         else:
             self.write(0x0243, 0)
@@ -159,45 +148,36 @@
             return OFF
 
     @setter
     def set_tc_type(self, _type: String):
         try:
             self.write(0x0283, OmegaPlatinum.TC_map[_type.upper()])
         except (KeyError, AttributeError):
-            raise ValueError(f'{self.name}: Invalid thermocouple type {_type}')
+            raise ValueError(f"{self.name}: Invalid thermocouple type {_type}")
 
     @getter
     def get_tc_type(self) -> String:
         try:
             return self.inverse_TC_map[self.read(0x0283)]
         except KeyError:
-            return 'None'
+            return "None"
 
 
 class RedLionPXU(Instrument):
     """
     Red Lion PXU temperature PID controller
     """
 
-    name = 'RedLionPXU'
+    name = "RedLionPXU"
 
-    supported_adapters = (
-        (ModbusSerial, {'buad_rate': 38400}),
-    )
+    supported_adapters = ((ModbusSerial, {"buad_rate": 38400}),)
 
-    knobs = (
-        'output',
-        'setpoint',
-        'autotune'
-    )
+    knobs = ("output", "setpoint", "autotune")
 
-    meters = (
-        'temperature',
-        'power'
-    )
+    meters = ("temperature", "power")
 
     @setter
     def set_output(self, state: Toggle):
         if state == ON:
             # turn on output & start PID control
             self.backend.write_bit(0x11, 1)
         elif state == OFF:
@@ -215,212 +195,193 @@
     @measurer
     def measure_power(self) -> Float:
         return self.read(0x8) / 10
 
     @setter
     def set_autotune(self, state: Toggle):
         if state == ON:
-            self.write(0xf, 1)
+            self.write(0xF, 1)
         elif state == OFF:
-            self.write(0xf, 0)
+            self.write(0xF, 0)
 
 
 class WatlowEZZone(Instrument):
     """
     Watlow EZ-Zone PID process controller
     """
 
-    name = 'WatlowEZZone'
+    name = "WatlowEZZone"
 
-    supported_adapters = (
-        (ModbusSerial, {'baud_rate': 9600}),
-    )
+    supported_adapters = ((ModbusSerial, {"baud_rate": 9600}),)
 
-    knobs = (
-        'setpoint',
-    )
+    knobs = ("setpoint",)
 
-    meters = (
-        'temperature',
-    )
+    meters = ("temperature",)
 
     @measurer
     def measure_temperature(self) -> Float:
         # swapped little-endian byte order (= 3 in minimalmodbus)
-        return self.read(360, dtype='float', byte_order=3)
+        return self.read(360, dtype="float", byte_order=3)
 
     @getter
     def get_setpoint(self) -> Float:
-        return self.read(2160, dtype='float', byte_order=3)
+        return self.read(2160, dtype="float", byte_order=3)
 
     @setter
     def set_setpoint(self, setpoint: Float):
-        return self.write(2160, setpoint, dtype='float', byte_order=3)
+        return self.write(2160, setpoint, dtype="float", byte_order=3)
 
     @getter
     def get_proportional_band(self) -> Float:
-        return self.read(1890, dtype='float', byte_order=3)
+        return self.read(1890, dtype="float", byte_order=3)
 
     @setter
     def set_proportional_band(self, band: Float):
-        return self.write(1890, band, dtype='float', byte_order=3)
+        return self.write(1890, band, dtype="float", byte_order=3)
 
     @getter
     def get_time_integral(self) -> Float:
-        return self.read(1894, dtype='float', byte_order=3)
+        return self.read(1894, dtype="float", byte_order=3)
 
     @setter
     def set_time_integral(self, integral: Float):
-        return self.write(1894, integral, dtype='float', byte_order=3)
+        return self.write(1894, integral, dtype="float", byte_order=3)
 
     @getter
     def get_time_derivative(self) -> Float:
-        return self.read(1896, dtype='float', byte_order=3)
+        return self.read(1896, dtype="float", byte_order=3)
 
     @setter
     def set_time_derivative(self, derivative: Float):
-        return self.write(1896, derivative, dtype='float', byte_order=3)
+        return self.write(1896, derivative, dtype="float", byte_order=3)
 
 
 class MKSGSeries(Instrument):
     """MKS G series mass flow controller"""
 
-    name = 'MKSGSeries'
+    name = "MKSGSeries"
 
     supported_adapters = ((Modbus, {}),)
 
     knobs = (
-        'setpoint',  # flow rate setpoint in SCCM
-        'ramp time'  # ramp time in milliseconds
+        "setpoint",  # flow rate setpoint in SCCM
+        "ramp time",  # ramp time in milliseconds
     )
 
     meters = (
-        'flow rate',  # actual flow rate in SCCM
-        'valve position',  # valve position in percent
-        'temperature'  # temperature in degrees C
+        "flow rate",  # actual flow rate in SCCM
+        "valve position",  # valve position in percent
+        "temperature",  # temperature in degrees C
     )
 
     @setter
     def set_setpoint(self, setpoint: Float):
-        self.write(16, 0xA000, setpoint, _type='32bit_float')
+        self.write(16, 0xA000, setpoint, _type="32bit_float")
 
     @getter
     def get_setpoint(self) -> Float:
-        return self.read(3, 0xA000, count=2, _type='32bit_float')
+        return self.read(3, 0xA000, count=2, _type="32bit_float")
 
     @setter
     def set_ramp_time(self, ramp_time: Float):
-        self.write(16, 0xA002, int(ramp_time), _type='32bit_uint')
+        self.write(16, 0xA002, int(ramp_time), _type="32bit_uint")
 
     @getter
     def get_ramp_time(self) -> Float:
-        return self.read(3, 0xA002, count=2, _type='32bit_uint')
+        return self.read(3, 0xA002, count=2, _type="32bit_uint")
 
     @measurer
     def measure_flow_rate(self) -> Float:
-        return self.read(4, 0x4000, count=2, _type='32bit_float')
+        return self.read(4, 0x4000, count=2, _type="32bit_float")
 
     @measurer
     def measure_valve_position(self) -> Float:
-        return self.read(4, 0x4004, count=2, _type='32bit_float')
+        return self.read(4, 0x4004, count=2, _type="32bit_float")
 
     @measurer
     def measure_temperature(self) -> Float:
-        return self.read(4, 0x4002, count=2, _type='32bit_float')
+        return self.read(4, 0x4002, count=2, _type="32bit_float")
 
 
 class AlicatMFC(Instrument):
     """Alicat mass flow controller"""
 
-    name = 'AlicatMFC'
+    name = "AlicatMFC"
 
-    supported_adapters = (
-        (Modbus, {}),
-    )
+    supported_adapters = ((Modbus, {}),)
 
-    knobs = (
-        'setpoint',  # flow rate setpoint in SCCM
-    )
+    knobs = ("setpoint",)  # flow rate setpoint in SCCM
 
     meters = (
-        'flow rate',  # actual flow rate in SCCM
-        'temperature',  # temperature in degrees C
-        'pressure'  
+        "flow rate",  # actual flow rate in SCCM
+        "temperature",  # temperature in degrees C
+        "pressure"
         # pressure in PSI (absolute, gauge or differential,
         # depending on device configuration)
     )
 
     @setter
     def set_setpoint(self, setpoint: Float):
-        self.write(16, 1009, setpoint, _type='32bit_float')
+        self.write(16, 1009, setpoint, _type="32bit_float")
 
     @getter
     def get_setpoint(self) -> Float:
-        return self.read(3, 1009, count=2, _type='32bit_float')
+        return self.read(3, 1009, count=2, _type="32bit_float")
 
     @measurer
     def measure_flow_rate(self) -> Float:
-        return self.read(4, 1208, count=2, _type='32bit_float')
+        return self.read(4, 1208, count=2, _type="32bit_float")
 
     @measurer
     def measure_temperature(self) -> Float:
-        return self.read(4, 1204, count=2, _type='32bit_float')
+        return self.read(4, 1204, count=2, _type="32bit_float")
 
     @measurer
     def measure_pressure(self) -> Float:
-        return self.read(4, 1202, count=2, _type='32bit_float')
+        return self.read(4, 1202, count=2, _type="32bit_float")
 
 
 class SynaccessNetbooter(Instrument):
-
     supported_adapters = (
-        (Socket, {
-            'write_termination': '\r\n',
-            'read_termination': None
-
-        }),
+        (Socket, {"write_termination": "\r\n", "read_termination": None}),
     )
 
     knobs = (
-        'port 1 toggle',
-        'port 2 toggle',
-        'port 3 toggle',
-        'port 4 toggle',
-        'port 5 toggle',
+        "port 1 toggle",
+        "port 2 toggle",
+        "port 3 toggle",
+        "port 4 toggle",
+        "port 5 toggle",
     )
 
     def _set_port_n_toggle(self, n, state):
-
         if state != ON and state != OFF:
             raise ValueError(
-                f'port toggle state of {self.name} must be '
-                f'either ON or OFF (Toggle type)'
+                f"port toggle state of {self.name} must be "
+                f"either ON or OFF (Toggle type)"
             )
 
         if state == ON:
-            self.write('$A3 %d 1' % n)
+            self.write("$A3 %d 1" % n)
         elif state == OFF:
-            self.write('$A3 %d 0' % n)
+            self.write("$A3 %d 0" % n)
 
     def _get_port_n_toggle(self, n):
-
         # Dump buffer (this device sends out a Telnet handshake upon initial
         # connection and periodically transmits null bytes, possibly as a
         # keep-alive signal)
         self.read(nbytes=np.inf, timeout=0.1, decode=False)
 
         def termination(message):
-            return re.search(b'A0,\d\d\d\d\d', message)
+            return re.search(b"A0,\d\d\d\d\d", message)
 
-        status_message = self.query(
-            '$A5', termination=termination, decode=False
-        )
+        status_message = self.query("$A5", termination=termination, decode=False)
 
         # Port statuses are a sequence of 0s and 1s, starting from the right
-        statuses = re.search(b'A0,\d\d\d\d\d', status_message)[0]
+        statuses = re.search(b"A0,\d\d\d\d\d", status_message)[0]
 
         port_n_toggle = ON if int(statuses.decode()[-n]) == 1 else OFF
 
         return port_n_toggle
 
     @setter
     def set_port_1_toggle(self, state: Toggle):
```

### Comparing `empyric-0.2.0/empyric/collection/generators.py` & `empyric-0.2.3/empyric/collection/generators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,175 +1,156 @@
 # Function/signal generators
 
 from empyric.adapters import Socket
 from empyric.instruments import Instrument, setter, getter, measurer
 from empyric.types import ON, OFF, Toggle, Integer, String, Float, recast
+from typing import Union
 
 
 class SiglentSDG1000(Instrument):
-
     supported_adapters = (
-        (Socket, {
-            'write_termination': '\n',
-            'read_termination': '\n'
-        }),
+        (Socket, {"write_termination": "\n", "read_termination": "\n"}),
     )
 
     knobs = (
-        'channel 1 output',
-        'channel 2 output',
-        'channel 1 load',
-        'channel 2 load',
-        'channel 1 polarity',
-        'channel 2 polarity',
-        'channel 1 waveform',
-        'channel 2 waveform',
-        'channel 1 high level',
-        'channel 2 high level',
-        'channel 1 low level',
-        'channel 2 low level',
-        'channel 1 frequency',
-        'channel 2 frequency',
-        'channel 1 pulse width',
-        'channel 2 pulse width',
-        'channel 1 pulse delay',
-        'channel 2 pulse delay'
-    )
-
-    wave_forms = (
-        'SINE', 'SQUARE', 'RAMP', 'PULSE', 'NOISE', 'ARB', 'DC', 'PRBS', 'IQ'
+        "channel 1 output",
+        "channel 2 output",
+        "channel 1 load",
+        "channel 2 load",
+        "channel 1 polarity",
+        "channel 2 polarity",
+        "channel 1 waveform",
+        "channel 2 waveform",
+        "channel 1 high level",
+        "channel 2 high level",
+        "channel 1 low level",
+        "channel 2 low level",
+        "channel 1 frequency",
+        "channel 2 frequency",
+        "channel 1 pulse width",
+        "channel 2 pulse width",
+        "channel 1 pulse delay",
+        "channel 2 pulse delay",
     )
 
-    def _set_channel_n_output(
-            self, n, output: Toggle, load: String, polarity: String
-    ):
+    wave_forms = ("SINE", "SQUARE", "RAMP", "PULSE", "NOISE", "ARB", "DC", "PRBS", "IQ")
 
-        self.write(f'C{n}:OUTP {output},LOAD,{load},PLRT,{polarity}')
+    def _set_channel_n_output(self, n, output: Toggle, load: String, polarity: String):
+        self.write(f"C{n}:OUTP {output},LOAD,{load},PLRT,{polarity}")
 
     def _get_channel_n_output(self, n) -> Toggle:
+        response = self.query("C%d:OUTP?" % n).split(",")
 
-        response = self.query('C%d:OUTP?' % n).split(',')
-
-        if response[0] == ('C%d:OUTP ON' % n):
+        if response[0] == ("C%d:OUTP ON" % n):
             output = ON
-        elif response[0] == ('C%d:OUTP OFF' % n):
+        elif response[0] == ("C%d:OUTP OFF" % n):
             output = OFF
         else:
             raise ValueError(
-                f'while trying to get output state of {self.name}, '
-                f'got corrupted response {response}'
+                f"while trying to get output state of {self.name}, "
+                f"got corrupted response {response}"
             )
 
         load = response[2]
 
-        if response[4] == 'NOR':
-            polarity = 'normal'
-        elif response[4] == 'INVT':
-            polarity = 'inverted'
+        if response[4] == "NOR":
+            polarity = "normal"
+        elif response[4] == "INVT":
+            polarity = "inverted"
         else:
             raise ValueError(
-                f'while trying to get output state of {self.name}, '
-                f'got corrupted response {response}'
+                f"while trying to get output state of {self.name}, "
+                f"got corrupted response {response}"
             )
 
         return output, load, polarity
 
     def _set_channel_n_waveform(self, n, **kwargs):
-
         waveform_dict = self._get_channel_n_waveform(n)
 
         for key in kwargs:
             if key.upper() not in waveform_dict:
                 raise ValueError(
-                    f'parameter {key} is not valid for waveform type '
+                    f"parameter {key} is not valid for waveform type "
                     f'{kwargs["WVTP"]}'
                 )
 
-        parameter_string = f'C{n}:BSWV ' + ','.join(
-            [f'{key.upper()},{value}' for key, value in kwargs.items()]
+        parameter_string = f"C{n}:BSWV " + ",".join(
+            [f"{key.upper()},{value}" for key, value in kwargs.items()]
         )
 
         self.write(parameter_string)
 
     def _get_channel_n_waveform(self, n):
+        response = self.query(f"C{n}:BSWV?")
 
-        response = self.query(f'C{n}:BSWV?')
-
-        response = response.split(f'C{n}:BSWV ')[1].split(',')
+        response = response.split(f"C{n}:BSWV ")[1].split(",")
 
         keys = response[::2]
         values = response[1::2]
 
         waveform_dict = {key: value for key, value in zip(keys, values)}
 
         return waveform_dict
 
     # Output
     @setter
     def set_channel_1_output(self, output: Toggle):
-
         _, load, polarity = self._get_channel_n_output(1)
 
         self._set_channel_n_output(1, output, load, polarity)
 
-
     @getter
     def get_channel_1_output(self) -> Toggle:
         return self._get_channel_n_output(1)[0]
 
-
     @setter
     def set_channel_2_output(self, output: Toggle):
-
         _, load, polarity = self._get_channel_n_output(2)
 
         self._set_channel_n_output(2, output, load, polarity)
 
     @getter
     def get_channel_2_output(self) -> Toggle:
         return self._get_channel_n_output(2)[0]
 
     # Load
     @setter
     def set_channel_1_load(self, load: String):
-
         output, _, polarity = self._get_channel_n_output(1)
 
         self._set_channel_n_output(1, output, load, polarity)
 
     @getter
     def get_channel_1_load(self) -> String:
         return self._get_channel_n_output(1)[1]
 
     @setter
     def set_channel_2_load(self, load: String):
-
         output, _, polarity = self._get_channel_n_output(2)
 
         self._set_channel_n_output(2, output, load, polarity)
 
     @getter
     def get_channel_2_load(self) -> String:
         return self._get_channel_n_output(2)[1]
 
     # Polarity
     @setter
     def set_channel_1_polarity(self, polarity: String):
-
         output, load, _ = self._get_channel_n_output(1)
 
         self._set_channel_n_output(1, output, load, polarity)
 
     @getter
     def get_channel_1_polarity(self) -> String:
         return self._get_channel_n_output(1)[1]
 
     @setter
     def set_channel_2_polarity(self, polarity: String):
-
         output, load, _ = self._get_channel_n_output(2)
 
         self._set_channel_n_output(2, output, load, polarity)
 
     @getter
     def get_channel_2_polarity(self) -> String:
         return self._get_channel_n_output(2)[1]
@@ -177,131 +158,121 @@
     # Waveform type
     @setter
     def set_channel_1_waveform(self, waveform: String):
         self._set_channel_n_waveform(1, wvtp=waveform)
 
     @getter
     def get_channel_1_waveform(self) -> String:
-        return self._get_channel_n_waveform(1)['WVTP']
+        return self._get_channel_n_waveform(1)["WVTP"]
 
     @setter
     def set_channel_2_waveform(self, waveform: String):
         self._set_channel_n_waveform(2, wvtp=waveform)
 
     @getter
     def get_channel_2_waveform(self) -> String:
-        return self._get_channel_n_waveform(2)['WVTP']
+        return self._get_channel_n_waveform(2)["WVTP"]
 
     # Waveform high level
     @setter
-    def set_channel_1_high_level(self, high_level: [Float, String]):
-        self._set_channel_n_waveform(1, hlev=f'{high_level}')
+    def set_channel_1_high_level(self, high_level: Union[Float, String]):
+        self._set_channel_n_waveform(1, hlev=f"{high_level}")
 
     @getter
     def get_channel_1_high_level(self) -> Float:
+        high_level_str = self._get_channel_n_waveform(1).get("HLEV", "nan")
 
-        high_level_str = self._get_channel_n_waveform(1).get('HLEV', 'nan')
-
-        return float(high_level_str.replace('V', ''))
+        return float(high_level_str.replace("V", ""))
 
     @setter
-    def set_channel_2_high_level(self, high_level: [Float, String]):
-        self._set_channel_n_waveform(2, hlev=f'{high_level}')
+    def set_channel_2_high_level(self, high_level: Union[Float, String]):
+        self._set_channel_n_waveform(2, hlev=f"{high_level}")
 
     @getter
     def get_channel_2_high_level(self) -> Float:
+        high_level_str = self._get_channel_n_waveform(2).get("HLEV", "nan")
 
-        high_level_str = self._get_channel_n_waveform(2).get('HLEV', 'nan')
-
-        return float(high_level_str.replace('V', ''))
+        return float(high_level_str.replace("V", ""))
 
     # Waveform low level
     @setter
-    def set_channel_1_low_level(self, low_level: [Float, String]):
-        self._set_channel_n_waveform(1, llev=f'{low_level}')
+    def set_channel_1_low_level(self, low_level: Union[Float, String]):
+        self._set_channel_n_waveform(1, llev=f"{low_level}")
 
     @getter
     def get_channel_1_low_level(self) -> Float:
+        low_level_str = self._get_channel_n_waveform(1).get("LLEV", "nan")
 
-        low_level_str = self._get_channel_n_waveform(1).get('LLEV', 'nan')
-
-        return float(low_level_str.replace('V', ''))
+        return float(low_level_str.replace("V", ""))
 
     @setter
-    def set_channel_2_low_level(self, low_level: [Float, String]):
-        self._set_channel_n_waveform(2, llev=f'{low_level}')
+    def set_channel_2_low_level(self, low_level: Union[Float, String]):
+        self._set_channel_n_waveform(2, llev=f"{low_level}")
 
     @getter
     def get_channel_2_low_level(self) -> Float:
+        low_level_str = self._get_channel_n_waveform(2).get("LLEV", "nan")
 
-        low_level_str = self._get_channel_n_waveform(2).get('LLEV', 'nan')
-
-        return float(low_level_str.replace('V', ''))
+        return float(low_level_str.replace("V", ""))
 
     # Waveform frequency
     @setter
-    def set_channel_1_frequency(self, frequency: [Float, String]):
-        self._set_channel_n_waveform(1, frq=f'{frequency}')
+    def set_channel_1_frequency(self, frequency: Union[Float, String]):
+        self._set_channel_n_waveform(1, frq=f"{frequency}")
 
     @getter
     def get_channel_1_frequency(self) -> Float:
+        freq_str = self._get_channel_n_waveform(1).get("FRQ", "nan")
 
-        freq_str = self._get_channel_n_waveform(1).get('FRQ', 'nan')
-
-        return float(freq_str.replace('HZ', ''))
+        return float(freq_str.replace("HZ", ""))
 
     @setter
-    def set_channel_2_frequency(self, frequency: [Float, String]):
-        self._set_channel_n_waveform(2, frq=f'{frequency}')
+    def set_channel_2_frequency(self, frequency: Union[Float, String]):
+        self._set_channel_n_waveform(2, frq=f"{frequency}")
 
     @getter
     def get_channel_2_frequency(self) -> Float:
+        freq_str = self._get_channel_n_waveform(2).get("FRQ", "nan")
 
-        freq_str = self._get_channel_n_waveform(2).get('FRQ', 'nan')
-
-        return float(freq_str.replace('HZ', ''))
+        return float(freq_str.replace("HZ", ""))
 
     # Pulse width
     @setter
-    def set_channel_1_pulse_width(self, width: [Float, String]):
-        self._set_channel_n_waveform(1, width=f'{width}')
+    def set_channel_1_pulse_width(self, width: Union[Float, String]):
+        self._set_channel_n_waveform(1, width=f"{width}")
 
     @getter
     def get_channel_1_pulse_width(self) -> Float:
+        width_str = self._get_channel_n_waveform(1).get("WIDTH", "nan")
 
-        width_str = self._get_channel_n_waveform(1).get('WIDTH', 'nan')
-
-        return float(width_str.replace('S', ''))
+        return float(width_str.replace("S", ""))
 
     @setter
-    def set_channel_2_pulse_width(self, width: [Float, String]):
-        self._set_channel_n_waveform(2, width=f'{width}')
+    def set_channel_2_pulse_width(self, width: Union[Float, String]):
+        self._set_channel_n_waveform(2, width=f"{width}")
 
     @getter
     def get_channel_2_pulse_width(self) -> Float:
+        width_str = self._get_channel_n_waveform(2).get("WIDTH", "nan")
 
-        width_str = self._get_channel_n_waveform(2).get('WIDTH', 'nan')
-
-        return float(width_str.replace('S', ''))
+        return float(width_str.replace("S", ""))
 
     # Pulse delay
     @setter
-    def set_channel_1_pulse_delay(self, delay: [Float, String]):
-        self._set_channel_n_waveform(1, dly=f'{delay}')
+    def set_channel_1_pulse_delay(self, delay: Union[Float, String]):
+        self._set_channel_n_waveform(1, dly=f"{delay}")
 
     @getter
     def get_channel_1_pulse_delay(self) -> Float:
+        delay_str = self._get_channel_n_waveform(1).get("DLY", "nan")
 
-        delay_str = self._get_channel_n_waveform(1).get('DLY', 'nan')
-
-        return float(delay_str.replace('S', ''))
+        return float(delay_str.replace("S", ""))
 
     @setter
-    def set_channel_2_pulse_delay(self, delay: [Float, String]):
-        self._set_channel_n_waveform(2, dly=f'{delay}')
+    def set_channel_2_pulse_delay(self, delay: Union[Float, String]):
+        self._set_channel_n_waveform(2, dly=f"{delay}")
 
     @getter
     def get_channel_2_pulse_delay(self) -> Float:
+        delay_str = self._get_channel_n_waveform(2).get("DLY", "nan")
 
-        delay_str = self._get_channel_n_waveform(2).get('DLY', 'nan')
-
-        return float(delay_str.replace('S', ''))
+        return float(delay_str.replace("S", ""))
```

### Comparing `empyric-0.2.0/empyric/collection/humans.py` & `empyric-0.2.3/empyric/collection/humans.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,48 +10,43 @@
     """
     Virtual instrument that queries a human operator via the Python console
 
     The prompt is what the user is asked; the cooldown is the minimum time
     between input requests
     """
 
-    name = 'ConsoleUser'
+    name = "ConsoleUser"
 
-    supported_adapters = (
-        (Adapter, {}),
-    )
+    supported_adapters = ((Adapter, {}),)
 
-    knobs = ('prompt',  # message or query to send to user
-             'cooldown')  # minimum time before sending repeat messages
+    knobs = (
+        "prompt",  # message or query to send to user
+        "cooldown",
+    )  # minimum time before sending repeat messages
 
-    presets = {
-        'cooldown': 0,
-        'prompt': '?'
-    }
+    presets = {"cooldown": 0, "prompt": "?"}
 
-    meters = ('response',)
+    meters = ("response",)
 
-    response = ''
+    response = ""
 
-    last_prompt = ''
-    last_sent = float('-inf')
+    last_prompt = ""
+    last_sent = float("-inf")
 
     @setter
     def set_prompt(self, prompt: String):
         pass
 
     @setter
     def set_cooldown(self, cooldown: Float):
         pass
 
     @measurer
     def measure_response(self) -> String:
-
-        new_prompt = (self.prompt != self.last_prompt)
+        new_prompt = self.prompt != self.last_prompt
 
         if time.time() >= self.last_sent + self.cooldown or new_prompt:
-
             response = input(self.prompt)
 
             self.last_prompt = self.prompt
 
         return response
```

### Comparing `empyric-0.2.0/empyric/collection/instrument.py` & `empyric-0.2.3/empyric/collection/instrument.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,89 +12,124 @@
     If the wrapped method returns a value, this value is assigned to the
     corresponding knob attribute of the instrument. This is convenient for
     cases where the set value maps to another value which is more relevant.
     Otherwise, the value of the method's first argument is assigned to the
     attribute.
 
     :param method: (callable) method to be wrapped
+
     :return: wrapped method
     """
 
-    knob = '_'.join(method.__name__.split('_')[1:])
+    knob = "_".join(method.__name__.split("_")[1:])
 
     type_hints = typing.get_type_hints(method)
-    type_hints.pop('self', None)
-    type_hints.pop('return', None)
+    type_hints.pop("self", None)
+    type_hints.pop("return", None)
 
     if type_hints:
         dtype = type_hints[list(type_hints)[0]]
     else:
         dtype = Type
 
     @wraps(method)
     def wrapped_method(*args, **kwargs):
-
         self = args[0]
         value = args[1]
 
+        while self._busy:
+            time.sleep(0.01)
+
         returned_value = method(*args, **kwargs)
 
         # The knob attribute is set to the returned value of the method, or
         # the value argument if the returned value is None
         if returned_value is not None:
             self.__setattr__(knob, recast(returned_value, to=dtype))
         else:
             self.__setattr__(knob, recast(value, to=dtype))
 
+        self._busy = False
+
     return wrapped_method
 
 
 def getter(method):
     """
     Utility function that wraps all get_[knob] methods and records the
     retrieved knob values.
 
     :param method: (callable) method to be wrapped
+
     :return: wrapped method
     """
 
-    knob = '_'.join(method.__name__.split('_')[1:])
+    knob = "_".join(method.__name__.split("_")[1:])
 
-    dtype = typing.get_type_hints(method).get('return', Type)
+    dtype = typing.get_type_hints(method).get("return", Type)
 
     @wraps(method)
     def wrapped_method(*args, **kwargs):
         self = args[0]
-        value = recast(method(*args, **kwargs), to=dtype)
+
+        while self._busy:
+            time.sleep(0.01)
+
+        try:
+            value = recast(method(*args, **kwargs), to=dtype)
+        except AttributeError as err:
+            # catches most errors caused by the adapter returning None
+            if "NoneType" in str(err):
+                value = None
+            else:
+                raise AttributeError(err)
+
         self.__setattr__(knob, value)
 
+        self._busy = False
+
         return value
 
     return wrapped_method
 
 
 def measurer(method):
     """
     Utility function that wraps all measure_[meter] methods and records the
     measured value.
 
     :param method: (callable) method to be wrapped
+
     :return: wrapped method
     """
 
-    meter = '_'.join(method.__name__.split('_')[1:])
+    meter = "_".join(method.__name__.split("_")[1:])
 
-    dtype = typing.get_type_hints(method).get('return', Type)
+    dtype = typing.get_type_hints(method).get("return", Type)
 
     @wraps(method)
     def wrapped_method(*args, **kwargs):
         self = args[0]
-        value = recast(method(*args, **kwargs), to=dtype)
+
+        while self._busy:
+            time.sleep(0.01)
+
+        try:
+            value = recast(method(*args, **kwargs), to=dtype)
+        except AttributeError as err:
+            # catches most errors caused by the adapter returning None
+            if "NoneType" in str(err):
+                value = None
+            else:
+                raise AttributeError(err)
+
         self.__setattr__(meter, value)
 
+        self._busy = False
+
         return value
 
     return wrapped_method
 
 
 class Instrument:
     """
@@ -116,31 +151,33 @@
     * ``postsets``: dictionary of knob settings (same format as ``presets``)
       to apply when the instrument is deleted.
     * ``meters``: tuple of the names of all meters that can be measured on
       this instrument.
 
     """
 
-    name = 'Instrument'
+    name = "Instrument"
 
-    supported_adapters = (
-        (Adapter, {}),
-    )
+    supported_adapters = ((Adapter, {}),)
 
     knobs = tuple()
 
     presets = {}
 
     postsets = {}
 
     meters = tuple()
 
+    # Flag for blocking concurrent operations; useful for set, get or measure
+    # methods that involve multiple adapter operations that might overlap in
+    # time with those of other set, get or measure calls.
+    _busy = False
+
     def __init__(
-            self, address=None, adapter=None, presets=None, postsets=None,
-            **kwargs
+        self, address=None, adapter=None, presets=None, postsets=None, **kwargs
     ):
         """
 
         :param address: (str/int) address of instrument
         :param adapter: (Adapter) desired adapter to use for communications
         with the instrument
         :param presets: (dict) dictionary of instrument presets of the form
@@ -163,36 +200,40 @@
             for _adapter, settings in self.supported_adapters:
                 settings.update(kwargs)
                 try:
                     self.adapter = _adapter(self, **settings)
                     adapter_connected = True
                     break
                 except BaseException as error:
-                    msg = f'in trying {_adapter.__name__} adapter, ' \
-                          f'got {type(error).__name__}: {error}'
+                    msg = (
+                        f"in trying {_adapter.__name__} adapter, "
+                        f"got {type(error).__name__}: {error}"
+                    )
                     errors.append(msg)
 
             if not adapter_connected:
-                message = f'unable to connect an adapter to ' \
-                          f'instrument {self.name} at address {address}:\n'
+                message = (
+                    f"unable to connect an adapter to "
+                    f"instrument {self.name} at address {address}:\n"
+                )
                 for error in errors:
                     message = message + f"{error}\n"
                 raise ConnectionError(message)
 
         if self.address:
-            self.name = self.name + '@' + str(self.address)
+            self.name = self.name + "@" + str(self.address)
 
         # Get existing knob settings, if possible
         for knob in self.knobs:
-            if hasattr(self, 'get_' + knob.replace(' ', '_')):
+            if hasattr(self, "get_" + knob.replace(" ", "_")):
                 # retrieves the knob value from the instrument
-                self.__getattribute__('get_' + knob.replace(' ', '_'))()
+                self.__getattribute__("get_" + knob.replace(" ", "_"))()
             else:
                 # knob value is unknown until it is set
-                self.__setattr__(knob.replace(' ', '_'), None)
+                self.__setattr__(knob.replace(" ", "_"), None)
 
         # Apply presets
         if presets:
             self.presets = {**self.presets, **presets}
 
         for knob, value in self.presets.items():
             self.set(knob, value)
@@ -244,15 +285,15 @@
 
         :param knob: (string) name of variable to be set
         :param value: (float/string) value of new variable setting
         :return: None
         """
 
         try:
-            set_method = getattr(self, 'set_' + knob.replace(' ', '_'))
+            set_method = getattr(self, "set_" + knob.replace(" ", "_"))
         except AttributeError as err:
             raise AttributeError(f"{knob} cannot be set on {self.name}\n{err}")
 
         set_method(value)
 
     def get(self, knob: str):
         """
@@ -260,30 +301,29 @@
         method for the knob, a command will be sent to the instrument to
         retrieve the actual value of the knob. If it does not have a get method
         for the knob, the last known value, stored as an instance attribute,
         will be return (possibly being ``nan`` if no value has yet been set)
 
         """
 
-        if hasattr(self, 'get_' + knob.replace(' ', '_')):
-            return getattr(self, 'get_' + knob.replace(' ', '_'))()
+        if hasattr(self, "get_" + knob.replace(" ", "_")):
+            return getattr(self, "get_" + knob.replace(" ", "_"))()
         else:
-            return getattr(self, knob.replace(' ', '_'))
+            return getattr(self, knob.replace(" ", "_"))
 
     def measure(self, meter: str):
         """
         Measure the value of a variable associated with this instrument
 
         :param meter: (string) name of the variable to be measured
         :return: (float/string) measured value of the variable
         """
 
         try:
-            measure_method = self.__getattribute__(
-                'measure_' + meter.replace(' ', '_'))
+            measure_method = self.__getattribute__("measure_" + meter.replace(" ", "_"))
         except AttributeError:
             raise AttributeError(f"{meter} cannot be measured on {self.name}")
 
         measurement = measure_method()
 
         return measurement
```

### Comparing `empyric-0.2.0/empyric/collection/io.py` & `empyric-0.2.3/empyric/collection/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,107 +11,103 @@
 
     For socket communication, the default port is 9500. If the IP address is
     unknown, you can use the Boost.IO Driver software to find it.
 
     ASCII Protocol must be used.
     """
 
-    supported_adapters = (
-        (Socket, {}),
-    )
+    supported_adapters = ((Socket, {}),)
 
     knobs = (
-        'analog_out0',
-        'analog_out1',
-        'analog_out2',
-        'analog_out3',
+        "analog_out0",
+        "analog_out1",
+        "analog_out2",
+        "analog_out3",
     )
 
     @setter
     def set_analog_out0(self, value: Float):
-        self.query('#010%f' % float(value), validator=self._set_validator)
+        self.query("#010%f" % float(value), validator=self._set_validator)
 
     @getter
     def get_analog_out0(self) -> Float:
-        response = self.query('$0160', validator=self._get_validator)
+        response = self.query("$0160", validator=self._get_validator)
         return recast(response[3:])
 
     @setter
     def set_analog_out1(self, value: Float):
-        self.query('#011%f' % float(value), validator=self._set_validator)
+        self.query("#011%f" % float(value), validator=self._set_validator)
 
     @getter
     def get_analog_out1(self) -> Float:
-        response = self.query('$0161', validator=self._get_validator)
+        response = self.query("$0161", validator=self._get_validator)
         return recast(response[3:])
 
     @setter
     def set_analog_out2(self, value: Float):
-        self.query('#012%f' % float(value), validator=self._set_validator)
+        self.query("#012%f" % float(value), validator=self._set_validator)
 
     @getter
     def get_analog_out2(self) -> Float:
-        response = self.query('$0162', validator=self._get_validator)
+        response = self.query("$0162", validator=self._get_validator)
         return recast(response[3:])
 
     @setter
     def set_analog_out3(self, value: Float):
-        self.query('#013%f' % float(value), validator=self._set_validator)
+        self.query("#013%f" % float(value), validator=self._set_validator)
 
     @getter
     def get_analog_out3(self) -> Float:
-        response = self.query('$0163', validator=self._get_validator)
+        response = self.query("$0163", validator=self._get_validator)
         return recast(response[3:])
 
     @staticmethod
     def _get_validator(response):
-        return re.match('!01\+\d\d\.\d\d\d', response)
+        return re.match("!01\+\d\d\.\d\d\d", response)
 
     @staticmethod
     def _set_validator(response):
-        return response.strip() == '>'
+        return response.strip() == ">"
 
 
 class BrainboxesED549(Instrument):
     """
     Brainboxes 4 channel analog input (0-10 V / 0-20mA) gateway.
 
     For socket communication, the default port is 9500. If the IP address is
     unknown, you can use the Boost.IO Driver software to find it.
 
     ASCII Protocol must be used.
     """
 
-    supported_adapters = (
-        (Socket, {}),
-    )
+    supported_adapters = ((Socket, {}),)
 
     meters = (
-        'analog_in0',
-        'analog_in1',
-        'analog_in2',
-        'analog_in3',
+        "analog_in0",
+        "analog_in1",
+        "analog_in2",
+        "analog_in3",
     )
 
     @measurer
     def measure_analog_in0(self) -> Float:
-        response = self.query('#010', validator=self._validator)
+        response = self.query("#010", validator=self._validator)
         return response[1:]
 
     @measurer
     def measure_analog_in1(self) -> Float:
-        response = self.query('#011', validator=self._validator)
+        response = self.query("#011", validator=self._validator)
         return response[1:]
 
     @measurer
     def measure_analog_in2(self) -> Float:
-        response = self.query('#012', validator=self._validator)
+        response = self.query("#012", validator=self._validator)
         return response[1:]
 
     @measurer
     def measure_analog_in3(self) -> Float:
-        response = self.query('#013', validator=self._validator)
+        response = self.query("#013", validator=self._validator)
         return response[1:]
 
     @staticmethod
     def _validator(response):
-        return re.match('>\+?\-?\d\d\.\d\d\d', response)
+        return re.match(">\+?\-?\d\d\.\d\d\d", response)
```

### Comparing `empyric-0.2.0/empyric/collection/multimeters.py` & `empyric-0.2.3/empyric/collection/multimeters.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,106 +10,107 @@
     Keithley 2110 digital multimeter instrument
     """
 
     name = "Keithley2110"
 
     supported_adapters = ((USB, {}),)
 
-    knobs = ('voltage range', 'current range')
+    knobs = ("voltage range", "current range")
 
-    meters = ('voltage', 'current', 'temperature')
+    meters = ("voltage", "current", "temperature")
 
     _mode = None
 
     @property
     def mode(self):
         return self._mode
 
     @mode.setter
     def mode(self, mode):
-        if mode == 'voltage':
+        if mode == "voltage":
             self.write('FUNC "VOLT"')
-            self._mode = 'voltage'
-        if mode == 'current':
+            self._mode = "voltage"
+        if mode == "current":
             self.write('FUNC "CURR"')
-            self._mode = 'current'
-        if mode == 'temperature':
+            self._mode = "current"
+        if mode == "temperature":
             self.write('FUNC "TCO"')
-            self._mode = 'temperature'
+            self._mode = "temperature"
 
     @setter
     def set_voltage_range(self, voltage_range: Float):
-
         allowed_voltage_ranges = (0, 0.1, 1.0, 10.0, 100.0, 1000.0)
 
         if voltage_range in allowed_voltage_ranges[1:]:
-            self.write('VOLT:RANG %.2e' % voltage_range)
+            self.write("VOLT:RANG %.2e" % voltage_range)
         elif isinstance(voltage_range, numbers.Number):
-
             # Find nearest encapsulating voltage range
             try:
-                nearest = np.argwhere(voltage_range <= np.array(
-                    allowed_voltage_ranges)).flatten()[0]
+                nearest = np.argwhere(
+                    voltage_range <= np.array(allowed_voltage_ranges)
+                ).flatten()[0]
             except IndexError:
                 nearest = -1
 
             self.set_voltage_range(allowed_voltage_ranges[nearest])
 
-            Warning('Given voltage range not an option, '
-                    f'setting to {allowed_voltage_ranges[nearest]} V instead')
+            Warning(
+                "Given voltage range not an option, "
+                f"setting to {allowed_voltage_ranges[nearest]} V instead"
+            )
 
         elif voltage_range == 0.0:
-            self.write('VOLT:RANG:AUTO')
+            self.write("VOLT:RANG:AUTO")
         else:
-            raise ValueError(
-                f'voltage range choice {voltage_range} not permitted!')
+            raise ValueError(f"voltage range choice {voltage_range} not permitted!")
 
     @setter
     def set_current_range(self, current_range: Float):
-
-        allowed_current_ranges = (0.0, .01, 0.1, 1.0, 3.0, 10.0)
+        allowed_current_ranges = (0.0, 0.01, 0.1, 1.0, 3.0, 10.0)
 
         if current_range in allowed_current_ranges:
-            self.write('CURR:RANG %.2e' % current_range)
+            self.write("CURR:RANG %.2e" % current_range)
         elif isinstance(current_range, numbers.Number):
             # Find nearest encapsulating current range
             try:
-                nearest = np.argwhere(current_range <= np.array(
-                    allowed_current_ranges)).flatten()[0]
+                nearest = np.argwhere(
+                    current_range <= np.array(allowed_current_ranges)
+                ).flatten()[0]
             except IndexError:
                 nearest = -1
 
             self.set_current_range(allowed_current_ranges[nearest])
 
-            Warning('Given current range not an option, '
-                    f'setting to {allowed_current_ranges[nearest]} A instead')
+            Warning(
+                "Given current range not an option, "
+                f"setting to {allowed_current_ranges[nearest]} A instead"
+            )
 
         elif current_range == 0.0:
-            self.write('CURR:RANG:AUTO')
+            self.write("CURR:RANG:AUTO")
         else:
-            raise ValueError(
-                f'current range choice {current_range} not permitted!')
+            raise ValueError(f"current range choice {current_range} not permitted!")
 
     @measurer
     def measure_voltage(self) -> Float:
-        if self.mode != 'voltage':
-            self.mode = 'voltage'
-        return float(self.query('READ?'))
+        if self.mode != "voltage":
+            self.mode = "voltage"
+        return float(self.query("READ?"))
 
     @measurer
     def measure_current(self) -> Float:
-        if self.mode != 'current':
-            self.mode = 'current'
-        return float(self.query('READ?'))
+        if self.mode != "current":
+            self.mode = "current"
+        return float(self.query("READ?"))
 
     @measurer
     def measure_temperature(self) -> Float:
-        if self.mode != 'temperature':
-            self.mode = 'temperature'
-        return float(self.query('READ?'))
+        if self.mode != "temperature":
+            self.mode = "temperature"
+        return float(self.query("READ?"))
 
 
 class Keithley6500(Instrument):
     """
     Multimeter with 6.5 digits and high speed scanning and digitizing
     capabilities.
 
@@ -120,324 +121,293 @@
 
     The `range` knob has separate values for the basic measurements (meter =
     'voltage' or 'current') and the digitized measurements (meter = 'fast
     voltages' or 'fast currents'). Be sure to set the desired range after
     switching meter types.
     """
 
-    name = 'Keithley6500'
+    name = "Keithley6500"
 
     supported_adapters = (
-        (Socket, {
-            'write_termination': '\n',
-            'read_termination': '\n',
-            'timeout': 0.5}
-         ),
+        (Socket, {"write_termination": "\n", "read_termination": "\n", "timeout": 0.5}),
     )
 
-    knobs = (
-        'meter',
-        'nplc',
-        'range',
-        'sample count',
-        'sample rate',
-        'trigger_source'
-    )
+    knobs = ("meter", "nplc", "range", "sample count", "sample rate", "trigger_source")
 
-    meters = (
-        'voltage',
-        'current',
-        'fast voltages',
-        'fast currents'
-    )
+    meters = ("voltage", "current", "fast voltages", "fast currents")
 
-    _trig_src = 'trigger.EVENT_DISPLAY'
+    _trig_src = "trigger.EVENT_DISPLAY"
     meter = None
 
     @setter
     def set_meter(self, meter: String):
-
-        if meter.lower() == 'voltage':
-            self.write(f'dmm.measure.func = dmm.FUNC_DC_VOLTAGE')
-        elif meter.lower() == 'current':
-            self.write(f'dmm.measure.func = dmm.FUNC_DC_CURRENT')
-        elif meter.lower() == 'fast voltages':
-            self.write(f'dmm.digitize.func = dmm.FUNC_DIGITIZE_VOLTAGE')
-        elif meter.lower() == 'fast currents':
-            self.write(f'dmm.digitize.func = dmm.FUNC_DIGITIZE_CURRENT')
+        if meter.lower() == "voltage":
+            self.write(f"dmm.measure.func = dmm.FUNC_DC_VOLTAGE")
+        elif meter.lower() == "current":
+            self.write(f"dmm.measure.func = dmm.FUNC_DC_CURRENT")
+        elif meter.lower() == "fast voltages":
+            self.write(f"dmm.digitize.func = dmm.FUNC_DIGITIZE_VOLTAGE")
+        elif meter.lower() == "fast currents":
+            self.write(f"dmm.digitize.func = dmm.FUNC_DIGITIZE_CURRENT")
         else:
-            raise print(f'Warning: invalid meter {meter} for Keithley6500')
+            raise print(f"Warning: invalid meter {meter} for Keithley6500")
             return self.get_meter()
 
         return meter.lower()
 
     @getter
     def get_meter(self) -> String:
-
         def validator(response):
-            return re.match('dmm.FUNC', response)
+            return re.match("dmm.FUNC", response)
 
-        meter = self.query('print(dmm.measure.func)', validator=validator)
+        meter = self.query("print(dmm.measure.func)", validator=validator)
 
-        if 'dmm.FUNC_NONE' in meter:
-            meter = self.query('print(dmm.digitize.func)')
+        if "dmm.FUNC_NONE" in meter:
+            meter = self.query("print(dmm.digitize.func)")
 
-            if 'dmm.FUNC_NONE' in meter:
-                raise ValueError(f'meter is undefined for {self.name}')
+            if "dmm.FUNC_NONE" in meter:
+                raise ValueError(f"meter is undefined for {self.name}")
 
         meter_dict = {
-            'dmm.FUNC_DC_CURRENT': 'current',
-            'dmm.FUNC_DC_VOLTAGE': 'voltage',
-            'dmm.FUNC_DIGITIZE_CURRENT': 'fast currents',
-            'dmm.FUNC_DIGITIZE_VOLTAGE': 'fast voltages'
+            "dmm.FUNC_DC_CURRENT": "current",
+            "dmm.FUNC_DC_VOLTAGE": "voltage",
+            "dmm.FUNC_DIGITIZE_CURRENT": "fast currents",
+            "dmm.FUNC_DIGITIZE_VOLTAGE": "fast voltages",
         }
 
         if meter in meter_dict:
             return meter_dict[meter]
         else:
-            return ''
+            return ""
 
     @setter
     def set_sample_count(self, count: Integer):
-
-        if 'fast' in self.meter:
-            self.write(f'dmm.digitize.count = {count}')
+        if "fast" in self.meter:  # pylint: disable=unsupported-membership-test
+            self.write(f"dmm.digitize.count = {count}")
         else:
             return 1
 
     @getter
     def get_sample_count(self) -> Integer:
+        if "fast" in self.meter:  # pylint: disable=unsupported-membership-test
+            response = self.query("print(dmm.digitize.count)")
 
-        if 'fast' in self.meter:
-            response = self.query('print(dmm.digitize.count)')
-
-            if 'nil' in response:
+            if "nil" in response:
                 return 0
             else:
                 return int(response)
         else:
             return 1
 
     @setter
     def set_sample_rate(self, rate: Integer):
-
-        if 'fast' in self.meter:
-            self.write(f'dmm.digitize.samplerate = {rate}')
+        if "fast" in self.meter:  # pylint: disable=unsupported-membership-test
+            self.write(f"dmm.digitize.samplerate = {rate}")
         else:
             return 0
 
     @getter
     def get_sample_rate(self) -> Integer:
+        if "fast" in self.meter:  # pylint: disable=unsupported-membership-test
+            response = self.query("print(dmm.digitize.samplerate)")
 
-        if 'fast' in self.meter:
-
-            response = self.query(f'print(dmm.digitize.samplerate)')
-
-            if 'nil' in response:
+            if "nil" in response:
                 return 0
             else:
                 return int(response)
         else:
             return 0
 
     @setter
     def set_nplc(self, nplc: Integer):
-
-        if self.meter in ['voltage', 'current']:
-            self.write(f'dmm.measure.nplc = {nplc}')
+        if self.meter in ["voltage", "current"]:
+            self.write(f"dmm.measure.nplc = {nplc}")
         else:
             return 0
 
     @getter
     def get_nplc(self) -> Integer:
-
-        if self.meter in ['voltage', 'current']:
-            return int(self.query('print(dmm.measure.nplc)'))
+        if self.meter in ["voltage", "current"]:
+            return int(self.query("print(dmm.measure.nplc)"))
         else:
             return 0
 
     @setter
     def set_range(self, _range: Float):
-
         meter = self.get_meter()
 
-        if meter in ['voltage', 'current']:
+        if meter in ["voltage", "current"]:
             if _range == 0.0:
-                self.write('dmm.measure.autorange = dmm.ON')
+                self.write("dmm.measure.autorange = dmm.ON")
             else:
-                self.write(f'dmm.measure.range = {_range}')
-        elif meter in ['fast voltages', 'fast currents']:
-            self.write('dmm.digitize.range = %.3e' % _range)
+                self.write(f"dmm.measure.range = {_range}")
+        elif meter in ["fast voltages", "fast currents"]:
+            self.write("dmm.digitize.range = %.3e" % _range)
         else:
             return self.get_range()
 
-
     @getter
     def get_range(self) -> Float:
-
         meter = self.get_meter()
 
-        if meter in ['voltage', 'current']:
-            if self.query('print(dmm.measure.autorange)') == 'dmm.ON':
+        if meter in ["voltage", "current"]:
+            if self.query("print(dmm.measure.autorange)") == "dmm.ON":
                 return 0.0
             else:
-                return float(self.query('print(dmm.measure.range)'))
+                return float(self.query("print(dmm.measure.range)"))
 
-        elif meter in ['fast voltages', 'fast currents']:
-            return float(self.query('print(dmm.digitize.range)'))
+        elif meter in ["fast voltages", "fast currents"]:
+            return float(self.query("print(dmm.digitize.range)"))
 
     @setter
     def set_trigger_source(self, trigger_source: String):
-
         valid_sources = {
-            'front panel': 'trigger.EVENT_DISPLAY',
-            'front': 'trigger.EVENT_DISPLAY',
-            'external in': 'trigger.EVENT_EXTERNAL',
-            'ext': 'trigger.EVENT_EXTERNAL'
+            "front panel": "trigger.EVENT_DISPLAY",
+            "front": "trigger.EVENT_DISPLAY",
+            "external in": "trigger.EVENT_EXTERNAL",
+            "ext": "trigger.EVENT_EXTERNAL",
         }
 
         if trigger_source.lower() in valid_sources:
             self._trig_src = valid_sources[trigger_source.lower()]
         else:
-            raise ValueError(f'invalid trigger source for {self.name}')
+            raise ValueError(f"invalid trigger source for {self.name}")
 
     @getter
     def get_trigger_source(self) -> String:
-
         trigger_sources = {
-            'trigger.EVENT_DISPLAY': 'front panel',
-            'trigger.EVENT_EXTERNAL': 'external in'
+            "trigger.EVENT_DISPLAY": "front panel",
+            "trigger.EVENT_EXTERNAL": "external in",
         }
 
         return trigger_sources[self._trig_src]
 
     @measurer
     def measure_current(self) -> Float:
+        if self.meter != "current":
+            self.set_meter("current")
 
-        if self.meter != 'current':
-            self.set_meter('current')
-
-        return recast(self.query('print(dmm.measure.read())'))
+        return recast(self.query("print(dmm.measure.read())"))
 
     @measurer
     def measure_voltage(self) -> Float:
+        if self.meter != "voltage":
+            self.set_meter("voltage")
 
-        if self.meter != 'voltage':
-            self.set_meter('voltage')
-
-        return recast(self.query('print(dmm.measure.read())'))
+        return recast(self.query("print(dmm.measure.read())"))
 
     def _execute_fast_measurements(self):
-
-        if 'fast' not in self.meter:
+        if "fast" not in self.meter:  # pylint: disable=unsupported-membership-test
             return
 
         trigger_src = {
-            'front panel': 'trigger.EVENT_DISPLAY',
-            'external in': 'trigger.EVENT_EXTERNAL'
+            "front panel": "trigger.EVENT_DISPLAY",
+            "external in": "trigger.EVENT_EXTERNAL",
         }[self.get_trigger_source()]
 
         self.write(
-            'trigger.model.setblock(1, trigger.BLOCK_BUFFER_CLEAR, '
-            'defbuffer1)\n'
-            'trigger.model.setblock(2, trigger.BLOCK_WAIT, '
-            f'{trigger_src})\n'
-            'trigger.model.setblock(3, trigger.BLOCK_DELAY_CONSTANT, 0)\n'
-            'trigger.model.setblock(4, trigger.BLOCK_MEASURE_DIGITIZE, '
-            'defbuffer1, dmm.digitize.count)\n'
-            'trigger.model.initiate()\n'
+            "trigger.model.setblock(1, trigger.BLOCK_BUFFER_CLEAR, "
+            "defbuffer1)\n"
+            "trigger.model.setblock(2, trigger.BLOCK_WAIT, "
+            f"{trigger_src})\n"
+            "trigger.model.setblock(3, trigger.BLOCK_DELAY_CONSTANT, 0)\n"
+            "trigger.model.setblock(4, trigger.BLOCK_MEASURE_DIGITIZE, "
+            "defbuffer1, dmm.digitize.count)\n"
+            "trigger.model.initiate()\n"
         )
 
         running = True
 
         running_states = [
-            'trigger.STATE_BUILDING',
-            'trigger.STATE_RUNNING',
-            'trigger.STATE_PAUSED',
-            'trigger.STATE_WAITING'
+            "trigger.STATE_BUILDING",
+            "trigger.STATE_RUNNING",
+            "trigger.STATE_PAUSED",
+            "trigger.STATE_WAITING",
         ]
 
         failed_states = [
-            'trigger.STATE_ABORTING',
-            'trigger.STATE_ABORTED',
-            'trigger.STATE_FAILED'
+            "trigger.STATE_ABORTING",
+            "trigger.STATE_ABORTED",
+            "trigger.STATE_FAILED",
         ]
 
-        state = ''
+        state = ""
 
         while running:
+            self.write("state, state, block_num = trigger.model.state()")
 
-            self.write('state, state, block_num = trigger.model.state()')
-
-            state = self.query('print(state)')
+            state = self.query("print(state)")
 
             running = state in running_states
 
             time.sleep(0.25)
 
         if state in failed_states:
-            raise RuntimeError(
-                f'fast measurement failed; trigger state is "{state}"'
-            )
+            raise RuntimeError(f'fast measurement failed; trigger state is "{state}"')
 
         readings = self.query(
-            'printbuffer(1, defbuffer1.n, defbuffer1.readings)',
-            nbytes=np.inf
+            "printbuffer(1, defbuffer1.n, defbuffer1.readings)", nbytes=np.inf
         )
 
-        return np.array(
-            [np.float64(reading) for reading in readings.split(', ')]
-        )
+        return np.array([np.float64(reading) for reading in readings.split(", ")])
 
     @measurer
     def measure_fast_voltages(self) -> Array:
-
-        if self.meter != 'fast voltages':
-            self.set_meter('fast voltages')
+        if self.meter != "fast voltages":
+            self.set_meter("fast voltages")
 
         fast_voltages = self._execute_fast_measurements()
 
         return fast_voltages
 
     @measurer
     def measure_fast_currents(self) -> Array:
-
-        if self.meter != 'fast currents':
-            self.set_meter('fast currents')
+        if self.meter != "fast currents":
+            self.set_meter("fast currents")
 
         fast_currents = self._execute_fast_measurements()
 
         return fast_currents
 
 
 class LabJackU6(Instrument):
     """
     LabJack U6 Multi-function DAQ
     """
 
-    name = 'LabJackU6'
+    name = "LabJackU6"
 
     supported_adapters = (
         # custom setup below until I can get serial or modbus comms to work
         (Adapter, {}),
     )
 
-    knobs = ('DAC0 ', 'DAC1',)
+    knobs = (
+        "DAC0 ",
+        "DAC1",
+    )
 
     meters = (
-        'AIN0', 'AIN1', 'AIN2', 'AIN3', 'device temperature',
-        'temperature 0', 'temperature 1', 'temperature 2', 'temperature 3'
+        "AIN0",
+        "AIN1",
+        "AIN2",
+        "AIN3",
+        "device temperature",
+        "temperature 0",
+        "temperature 1",
+        "temperature 2",
+        "temperature 3",
     )
 
     def __init__(self, *args, **kwargs):
-        u6 = importlib.import_module('u6')
+        u6 = importlib.import_module("u6")
         self.backend = u6.U6()
 
-        if len(args) == 0 and 'address' not in kwargs:
-            kwargs['address'] = str(self.backend.serialNumber)
+        if len(args) == 0 and "address" not in kwargs:
+            kwargs["address"] = str(self.backend.serialNumber)
 
         Instrument.__init__(self, *args, **kwargs)
 
     def write(self, register, value):
         self.backend.writeRegister(register, value)
 
     def read(self, register):
@@ -500,39 +470,47 @@
     """
     LabJack T7/T7-Pro DAQ
 
     Only reading the default 14 inputs as voltages is currently supported, but
     this may eventually be expanded.
     """
 
-    name = 'LabJackT7'
+    name = "LabJackT7"
 
-    supported_adapters = (
-        (Modbus, {}),
-    )
+    supported_adapters = ((Modbus, {}),)
 
-    knobs = (
-        'DIO0', 'DIO1', 'DIO2', 'DIO3', 'DIO4', 'DIO5', 'DIO6', 'DIO7'
-    )
+    knobs = ("DIO0", "DIO1", "DIO2", "DIO3", "DIO4", "DIO5", "DIO6", "DIO7")
 
     meters = (
-        'AIN0', 'AIN1', 'AIN2', 'AIN3', 'AIN4', 'AIN5', 'AIN6',
-        'AIN7', 'AIN8', 'AIN9', 'AIN10', 'AIN11', 'AIN12', 'AIN13',
-        'AIN all',
-        'device temperature'
+        "AIN0",
+        "AIN1",
+        "AIN2",
+        "AIN3",
+        "AIN4",
+        "AIN5",
+        "AIN6",
+        "AIN7",
+        "AIN8",
+        "AIN9",
+        "AIN10",
+        "AIN11",
+        "AIN12",
+        "AIN13",
+        "AIN all",
+        "device temperature",
     )
 
     def _set_DION(self, n, value: Integer):
-        self.write(16, 2000 + n, value, _type='16bit_uint')
+        self.write(16, 2000 + n, value, _type="16bit_uint")
 
     def _get_DION(self, n) -> Integer:
-        return self.read(3, 2000 + n, count=1, _type='16bit_uint')
+        return self.read(3, 2000 + n, count=1, _type="16bit_uint")
 
     def _measure_AIN(self, n) -> Float:
-        return self.read(3, 2*n, count=2, _type='32bit_float')
+        return self.read(3, 2 * n, count=2, _type="32bit_float")
 
     @setter
     def set_DIO0(self, value: Integer):
         self._set_DION(0, value)
 
     @getter
     def get_DIO0(self) -> Integer:
@@ -649,13 +627,13 @@
     @measurer
     def measure_AIN13(self) -> Float:
         return self._measure_AIN(13)
 
     @measurer
     def measure_AIN_all(self) -> Array:
         """Reads all 14 analog inputs in a single call"""
-        return self.read(4, 0, count=2*14, _type='32bit_float')
+        return self.read(4, 0, count=2 * 14, _type="32bit_float")
 
     @measurer
     def measure_device_temperature(self) -> Float:
         """Device temperature in C"""
-        return self.read(4, 60052, count=2, _type='32bit_float') - 273.15
+        return self.read(4, 60052, count=2, _type="32bit_float") - 273.15
```

### Comparing `empyric-0.2.0/empyric/collection/scopes.py` & `empyric-0.2.3/empyric/collection/scopes.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,103 +9,100 @@
     """
     Tektronix oscillscope of the TDS200, TDS1000/2000, TDS1000B/2000B,
     TPS2000 series
 
     NOT TESTED
     """
 
-    name = 'TekScope'
+    name = "TekScope"
 
-    supported_adapters = (
-        (USB, {'timeout': 10}),  # acquisitions can take a long time
-    )
+    supported_adapters = ((USB, {"timeout": 10}),)  # acquisitions can take a long time
 
     knobs = (
-        'horz scale',
-        'horz position',
-        'ch1 scale',
-        'ch1 position',
-        'ch2 scale',
-        'ch2 position',
-        'ch3 scale',
-        'ch3 position',
-        'ch4 scale',
-        'ch4 position',
-        'trigger level',
+        "horz scale",
+        "horz position",
+        "ch1 scale",
+        "ch1 position",
+        "ch2 scale",
+        "ch2 position",
+        "ch3 scale",
+        "ch3 position",
+        "ch4 scale",
+        "ch4 position",
+        "trigger level",
     )
 
     meters = (
-        'channel 1',
-        'channel 2',
-        'channel 3',
-        'channel 4',
+        "channel 1",
+        "channel 2",
+        "channel 3",
+        "channel 4",
     )
 
     @setter
     def set_horz_scale(self, scale: Float):
-        self.write('HOR:SCA %.3e' % scale)
+        self.write("HOR:SCA %.3e" % scale)
 
     @setter
     def set_horz_position(self, position: Float):
-        self.write('HOR:POS %.3e' % position)
+        self.write("HOR:POS %.3e" % position)
 
     @setter
     def set_ch1_scale(self, scale: Float):
-        self.write('CH1:SCA %.3e' % scale)
+        self.write("CH1:SCA %.3e" % scale)
 
     @setter
     def set_ch2_scale(self, scale: Float):
-        self.write('CH1:SCA %.3e' % scale)
+        self.write("CH1:SCA %.3e" % scale)
 
     @setter
     def set_ch3_scale(self, scale: Float):
-        self.write('CH1:SCA %.3e' % scale)
+        self.write("CH1:SCA %.3e" % scale)
 
     @setter
     def set_ch4_scale(self, scale: Float):
-        self.write('CH1:SCA %.3e' % scale)
+        self.write("CH1:SCA %.3e" % scale)
 
     @setter
     def set_ch1_position(self, position: Float):
-        self.write('CH1:POS %.3e' % position)
+        self.write("CH1:POS %.3e" % position)
 
     @setter
     def set_ch2_position(self, position: Float):
-        self.write('CH1:POS %.3e' % position)
+        self.write("CH1:POS %.3e" % position)
 
     @setter
     def set_ch3_position(self, position: Float):
-        self.write('CH1:POS %.3e' % position)
+        self.write("CH1:POS %.3e" % position)
 
     @setter
     def set_ch4_position(self, position: Float):
-        self.write('CH1:POS %.3e' % position)
+        self.write("CH1:POS %.3e" % position)
 
     @setter
     def set_trigger_level(self, level: Float):
-        self.write('TRIG:MAI:LEV %.3e' % level)
+        self.write("TRIG:MAI:LEV %.3e" % level)
 
     def _measure_channel(self, channel):
+        self.write("DAT:ENC ASCI")  # ensure ASCII encoding of data
+        self.write("DAT:SOU CH%d" % channel)  # switch to channel 1
 
-        self.write('DAT:ENC ASCI') # ensure ASCII encoding of data
-        self.write('DAT:SOU CH%d' % channel)  # switch to channel 1
+        scale_factor = float(self.query("WFMPRE:YMULT?"))
+        zero = float(self.query("WFMPRE:YZERO?"))
+        offset = float(self.query("WFMPRE:YOFF?"))
 
-        scale_factor = float(self.query('WFMPRE:YMULT?'))
-        zero = float(self.query('WFMPRE:YZERO?'))
-        offset = float(self.query('WFMPRE:YOFF?'))
+        self.write("ACQ:STATE RUN")  # acquire the waveform
 
-        self.write('ACQ:STATE RUN') # acquire the waveform
-
-        while int(self.query('BUSY?')):
+        while int(self.query("BUSY?")):
             time.sleep(1)  # wait for acquisition to complete
 
-        str_data = self.query('CURVE?').split(' ')[1].split(',')
-        return np.array([
-            (float(datum) - offset)*scale_factor + zero for datum in str_data
-        ])
+        str_data = self.query("CURVE?").split(" ")[1].split(",")
+        return np.array(
+            [(float(datum) - offset) * scale_factor + zero for datum in str_data]
+        )
 
     @measurer
     def measure_channel_1(self) -> Array:
         return self._measure_channel(1)
 
     @measurer
     def measure_channel_2(self) -> Array:
@@ -124,129 +121,145 @@
     """
     Multicomp Pro PC Oscilloscope.
 
     NOT TESTED
     """
 
     supported_adapters = (
-        (USB, {'delay': 1}),
+        (USB, {"delay": 1}),
         # acquisitions can take a long time
     )
     """Supported adapters and options."""
 
     knobs = (
-        'horz scale',
-        'horz position',
-        'scale ch1',
-        'position ch1',
-        'scale ch2',
-        'position ch2',
-        'sweep mode',
-        'trigger level',
-        'trigger source',
-        'sweep mode',
-        'resolution',
-        'acquire',
-        'state'
+        "horz scale",
+        "horz position",
+        "scale ch1",
+        "position ch1",
+        "scale ch2",
+        "position ch2",
+        "sweep mode",
+        "trigger level",
+        "trigger source",
+        "sweep mode",
+        "resolution",
+        "acquire",
+        "state",
     )
 
     meters = (
-        'channel 1',
-        'channel 2',
+        "channel 1",
+        "channel 2",
     )
 
     presets = {
-        'resolution': '100000',
-        'sweep mode': 'SINGLE',
-        'trigger source': 1,
+        "resolution": "100000",
+        "sweep mode": "SINGLE",
+        "trigger source": 1,
     }
 
     _time_scales = {
-        2e-9: '2.0ns', 5e-9: '5.0ns', 10e-9: '10ns',
-        20e-9: '20ns', 50e-9: '50ns', 100e-9: '100ns',
-        200e-9: '200ns', 500e-9: '500ns', 1e-6: '1.0us',
-        2e-6: '2.0us', 5e-6: '5.0us', 10e-6: '10us',
-        20e-6: '20us', 50e-6: '50us', 100e-6: '100us',
-        200e-6: '200us', 500e-6: '500us', 1e-3: '1.0ms',
-        2e-3: '2.0ms', 5e-3: '5.0ms', 10e-3: '10ms',
-        20e-3: '20ms', 50e-3: '50ms', 100e-3: '100ms',
-        200e-3: '200ms', 500e-3: '500ms', 1: '1.0s',
-        2: '2.0s', 5: '5.0s', 10: '10s',
-        20: '20s', 50: '50s', 100: '100s'
+        2e-9: "2.0ns",
+        5e-9: "5.0ns",
+        10e-9: "10ns",
+        20e-9: "20ns",
+        50e-9: "50ns",
+        100e-9: "100ns",
+        200e-9: "200ns",
+        500e-9: "500ns",
+        1e-6: "1.0us",
+        2e-6: "2.0us",
+        5e-6: "5.0us",
+        10e-6: "10us",
+        20e-6: "20us",
+        50e-6: "50us",
+        100e-6: "100us",
+        200e-6: "200us",
+        500e-6: "500us",
+        1e-3: "1.0ms",
+        2e-3: "2.0ms",
+        5e-3: "5.0ms",
+        10e-3: "10ms",
+        20e-3: "20ms",
+        50e-3: "50ms",
+        100e-3: "100ms",
+        200e-3: "200ms",
+        500e-3: "500ms",
+        1: "1.0s",
+        2: "2.0s",
+        5: "5.0s",
+        10: "10s",
+        20: "20s",
+        50: "50s",
+        100: "100s",
     }
 
     _volt_scales = {
-        2e-3: '2mv', 5e-3: '5mv', 10e-3: '10mv',
-        20e-3: '20mv', 50e-3: '50mv', 100e-3: '100mv',
-        200e-3: '200mv', 500e-3: '500mv', 1.0: '1v',
-        2.0: '2v', 5.0: '5v'
+        2e-3: "2mv",
+        5e-3: "5mv",
+        10e-3: "10mv",
+        20e-3: "20mv",
+        50e-3: "50mv",
+        100e-3: "100mv",
+        200e-3: "200mv",
+        500e-3: "500mv",
+        1.0: "1v",
+        2.0: "2v",
+        5.0: "5v",
     }
 
-    _volt_div_table = {
-        0: 1e-3,
-        9: 1.0
-    }
+    _volt_div_table = {0: 1e-3, 9: 1.0}
 
-    _resolutions = {
-        1e3: '1K',
-        1e4: '10K',
-        1e5: '100K',
-        1e6: '1M',
-        1e7: '10M'
-    }
+    _resolutions = {1e3: "1K", 1e4: "10K", 1e5: "100K", 1e6: "1M", 1e7: "10M"}
 
-    _sweep_modes = ['AUTO', 'NORMAL', 'NORM', 'SINGLE', 'SING']
+    _sweep_modes = ["AUTO", "NORMAL", "NORM", "SINGLE", "SING"]
 
     _acquiring = False
 
     @setter
     def set_horz_scale(self, scale):
-
         new_time_scale = find_nearest(list(self._time_scales.keys()), scale)
 
-        self.write(':HORI:SCAL ' + self._time_scales[new_time_scale])
+        self.write(":HORI:SCAL " + self._time_scales[new_time_scale])
 
     @getter
     def get_horz_scale(self):
-
         time_scales_rev = {val: key for key, val in self._time_scales.items()}
 
-        time_scale_str = self.query(':HORI:SCAL?')[:-2]
+        time_scale_str = self.query(":HORI:SCAL?")[:-2]
 
         return time_scales_rev[time_scale_str]
 
     @setter
     def set_horz_position(self, offset):
-        self.write(':HORI:OFFS ' + str(offset))
+        self.write(":HORI:OFFS " + str(offset))
 
     @getter
     def get_horz_position(self):
-        return float(self.query(':HORI:OFFS?')[:-2])
+        return float(self.query(":HORI:OFFS?")[:-2])
 
     def _set_scale_ch(self, channel, scale):
-
         new_volt_scale = find_nearest(list(self._volt_scales.keys()), scale)
 
         scale_str = self._volt_scales[new_volt_scale]
 
-        self.write((':CH%d:SCAL ' % channel) + scale_str)
+        self.write((":CH%d:SCAL " % channel) + scale_str)
 
     def _get_scale_ch(self, channel):
+        volt_scale_str = self.query(":CH%d:SCAL?" % channel)[:-2]
 
-        volt_scale_str = self.query(':CH%d:SCAL?' % channel)[:-2]
-
-        if 'mv' in volt_scale_str.lower():
+        if "mv" in volt_scale_str.lower():
             return 1e-3 * float(volt_scale_str[:-2])
-        elif 'v' in volt_scale_str.lower():
+        elif "v" in volt_scale_str.lower():
             return float(volt_scale_str[:-1])
         else:
-            return float('nan')
+            return float("nan")
 
     def _set_position_ch(self, channel, position):
-        self.write((':CH%d:OFFS ' % channel) + str(position))
+        self.write((":CH%d:OFFS " % channel) + str(position))
 
     @setter
     def set_scale_ch(self, scale, channel=None):
         self._set_scale_ch(channel, scale)
 
     @getter
     def get_scale_ch(self, channel=None):
@@ -254,350 +267,344 @@
 
     @setter
     def set_position_ch(self, position, channel=None):
         self._set_position_ch(channel, position)
 
     @getter
     def get_position_ch(self, channel=None):
-        return float(self.query(':CH%d:OFFS?' % channel)[:-2])
+        return float(self.query(":CH%d:OFFS?" % channel)[:-2])
 
     @setter
     def set_sweep_mode(self, mode):
-
         if mode.upper() not in self._sweep_modes:
             raise ValueError(
                 f"Invalid sweep mode! "
                 f"Sweep mode must be one of: {', '.join(self._sweep_modes)}"
             )
 
-        self.write(':TRIG:SING:SWE ' + mode.upper())
+        self.write(":TRIG:SING:SWE " + mode.upper())
 
     @getter
     def get_sweep_mode(self):
-        return self.query(':TRIG:SING:SWE?')[:-2].upper()
+        return self.query(":TRIG:SING:SWE?")[:-2].upper()
 
     @setter
     def set_trigger_source(self, source):
-        self.write(':TRIG:SING:EDGE:SOUR CH%d' % int(source))
+        self.write(":TRIG:SING:EDGE:SOUR CH%d" % int(source))
 
     @getter
     def get_trigger_source(self):
-        source = self.query(':TRIG:SING:EDGE:SOUR?')[:-2]
+        source = self.query(":TRIG:SING:EDGE:SOUR?")[:-2]
 
-        if source == 'CH1':
+        if source == "CH1":
             return 1
-        elif source == 'CH2':
+        elif source == "CH2":
             return 2
 
     @setter
     def set_trigger_level(self, level_volts):
-
         trigger_source = self.get_trigger_source()
 
         scale = self._get_scale_ch(trigger_source)
 
         level_div = str(level_volts / scale)
 
-        self.write(':TRIG:SING:EDGE:LEV ' + level_div)
+        self.write(":TRIG:SING:EDGE:LEV " + level_div)
 
     @getter
     def get_trigger_level(self):
-
         trigger_source = self.get_trigger_source()
 
         scale = self._get_scale_ch(trigger_source)
 
-        return float(self.query(':TRIG:SING:EDGE:LEV?')[:-2]) * scale
+        return float(self.query(":TRIG:SING:EDGE:LEV?")[:-2]) * scale
 
     @measurer
     def measure_trigger_status(self):
-        return self.query(':TRIG:STATUS?')[:-2]
+        return self.query(":TRIG:STATUS?")[:-2]
 
     @setter
     def set_resolution(self, resolution):
-
         if resolution not in self._resolutions:
             raise ValueError(
                 f"Invalid memory depth! "
                 f"Memory depth must be one of: {', '.join(self._resolutions)}"
             )
 
-        self.write(':ACQ:DEPMEM ' + self._resolutions[resolution])
+        self.write(":ACQ:DEPMEM " + self._resolutions[resolution])
 
     @getter
     def get_resolution(self):
-
         res_rev = {val: key for key, val in self._resolutions.items()}
 
-        return res_rev[self.query(':ACQ:DEPMEM?')[:-2]]
+        return res_rev[self.query(":ACQ:DEPMEM?")[:-2]]
 
     @setter
     def set_state(self, state):
-        if state.upper() in ['RUN', 'STOP']:
-            self.write(f':{state.upper()}')
+        if state.upper() in ["RUN", "STOP"]:
+            self.write(f":{state.upper()}")
 
     @setter
     def set_acquire(self, _):
-
         self._acquiring = True
 
-        self.set_sweep_mode('SINGLE')
+        self.set_sweep_mode("SINGLE")
 
         trig_status = self.measure_trigger_status()
 
-        if trig_status == 'TRIG':
+        if trig_status == "TRIG":
             # measurement has been triggered
             pass
         else:
             # sweep needs to be reset
             time.sleep(0.1)
             self.set_acquire(1)
 
     def _read_preamble(self, channel):
-
         info_dict = {}
 
-        preamble = self.query(':WAV:PRE?', binary=True)
+        preamble = self.query(":WAV:PRE?", binary=True)
 
         header, info = preamble[:11], preamble[11:]
 
-        if header != b'#9000000000':  # indicates empty data buffer
-
+        if header != b"#9000000000":  # indicates empty data buffer
             try:
                 # First 8 bytes is an integer signature, used for verification
                 ver_int = 651058244139746640
-                verified = struct.unpack('<q', info[:8])[0] == ver_int
+                verified = struct.unpack("<q", info[:8])[0] == ver_int
 
                 if verified:
                     if channel == 1:
                         scale = self._volt_div_table[
-                            struct.unpack('<h', info[260:262])[0]
+                            struct.unpack("<h", info[260:262])[0]
                         ]
-                        zero = struct.unpack('<f', info[268:272])[0]
+                        zero = struct.unpack("<f", info[268:272])[0]
                     else:
                         scale = self._volt_div_table[
-                            struct.unpack('<h', info[262:264])[0]
+                            struct.unpack("<h", info[262:264])[0]
                         ]
-                        zero = struct.unpack('<f', info[272:276])[0]
+                        zero = struct.unpack("<f", info[272:276])[0]
 
-                    sample_rate = struct.unpack('<f', info[316:320])[0] * 1e6
+                    sample_rate = struct.unpack("<f", info[316:320])[0] * 1e6
                     # Hz
 
-                    info_dict['scale'] = scale
-                    info_dict['zero'] = zero
-                    info_dict['sample rate'] = sample_rate
+                    info_dict["scale"] = scale
+                    info_dict["zero"] = zero
+                    info_dict["sample rate"] = sample_rate
                 else:
                     print(
-                        f'Warning: {self.name} received unverified '
-                        f'signature when reading from channel {channel}'
+                        f"Warning: {self.name} received unverified "
+                        f"signature when reading from channel {channel}"
                     )
 
             except struct.error:
                 print(
-                    f'Warning: {self.name} received truncated preamble when '
-                    f'reading from channel {channel}'
+                    f"Warning: {self.name} received truncated preamble when "
+                    f"reading from channel {channel}"
                 )
 
-        self._sample_rate = info['sample rate']
+        self._sample_rate = info["sample rate"]
 
         return info_dict
 
     def _read_data(self, channel):
-
         info = self._read_preamble(channel)
 
         if info:
-            scale = info['scale']
-            zero = info['zero']
+            scale = info["scale"]
+            zero = info["zero"]
         else:
             return None
 
         # Only 256k data points can be read at a time
         resolution = int(
-            self.get_resolution().replace('K', '000').replace('M', '000000')
+            self.get_resolution().replace("K", "000").replace("M", "000000")
         )
 
         if resolution < 256000:  # can get all data in one pass
+            self.write(":WAV:RANG 0, %d" % resolution)
 
-            self.write(':WAV:RANG 0, %d' % resolution)
-
-            raw_response = self.query(':WAV:FETC?', binary=True)
+            raw_response = self.query(":WAV:FETC?", binary=True)
 
             header, byte_data = raw_response[:11], raw_response[11:]
 
             data_len = int(header[2:]) // 2
 
             voltages = scale * (
-                np.array(
-                    struct.unpack(f'<{data_len}h', byte_data), dtype=float
-                ) / 6400 - zero
+                np.array(struct.unpack(f"<{data_len}h", byte_data), dtype=float) / 6400
+                - zero
             )
 
         else:  # need to read data in chunks; max chunk size is 256k
-
             offset, size = 0, 200000
 
             voltages = np.empty(resolution)
 
             while offset + size <= resolution:
+                self.write(":WAV:RANG %d, %d" % (offset, size))
 
-                self.write(':WAV:RANG %d, %d' % (offset, size))
-
-                raw_response = self.query(':WAV:FETC?', binary=True)
+                raw_response = self.query(":WAV:FETC?", binary=True)
 
                 header, byte_data = raw_response[:11], raw_response[11:]
 
                 data_len = int(header[2:]) // 2
 
-                voltages[offset:offset + size] = scale * (
-                    np.array(
-                        struct.unpack(f'<{data_len}h', byte_data),
-                        dtype=float
-                    ) / 6400 - zero
+                voltages[offset : offset + size] = scale * (
+                    np.array(struct.unpack(f"<{data_len}h", byte_data), dtype=float)
+                    / 6400
+                    - zero
                 )
 
                 offset += size
 
         if len(voltages) != resolution:
             print(
-                f'Warning: {self.name} received truncated data '
-                f'for channel {channel}; discarding'
+                f"Warning: {self.name} received truncated data "
+                f"for channel {channel}; discarding"
             )
             return None
 
         return voltages
 
     @measurer
     def measure_channel_1(self):
-
         if not self._acquiring:
             self.set_acquire(True)
 
         self._acquiring = False
 
-        self.write(':WAV:BEG CH1')
+        self.write(":WAV:BEG CH1")
 
         data = self._read_data(1)
 
-        self.write(':WAV:END CH1')
+        self.write(":WAV:END CH1")
 
         return data[1]
 
     @measurer
     def measure_channel_2(self):
-
         if not self._acquiring:
             self.set_acquire(True)
 
         self._acquiring = False
 
-        self.write(':WAV:BEG CH2')
+        self.write(":WAV:BEG CH2")
 
         data = self._read_data(2)
 
-        self.write(':WAV:END CH2')
+        self.write(":WAV:END CH2")
 
         return data[1]
 
 
 class SiglentSDS1000(Instrument):
     """
     Siglent SDS1000 series digital oscilloscope
     """
 
-    name = 'SiglentSDS1000'
+    name = "SiglentSDS1000"
 
     supported_adapters = (
-        (Socket, {
-            'write_termination': '\n',
-            'read_termination': '\n'
-        }),
+        (Socket, {"write_termination": "\n", "read_termination": "\n"}),
     )
 
     knobs = (
-        'horz scale',
-        'horz position',
-        'ch1 scale',
-        'ch1 position',
-        'ch2 scale',
-        'ch2 position',
-        'ch3 scale',
-        'ch3 position',
-        'ch4 scale',
-        'ch4 position',
-        'trigger source',
-        'trigger level',
-        'acquire mode',
-        'memory size',
-        'averages'
+        "horz scale",
+        "horz position",
+        "ch1 scale",
+        "ch1 position",
+        "ch2 scale",
+        "ch2 position",
+        "ch3 scale",
+        "ch3 position",
+        "ch4 scale",
+        "ch4 position",
+        "trigger source",
+        "trigger level",
+        "acquire mode",
+        "memory size",
+        "averages",
     )
 
-    meters = (
-        'ch1 waveform',
-        'ch2 waveform',
-        'ch3 waveform',
-        'ch4 waveform'
-    )
+    meters = ("ch1 waveform", "ch2 waveform", "ch3 waveform", "ch4 waveform")
 
     horz_scales = [
-        1e-9, 2e-9, 5e-9, 10e-9, 20e-9, 50e-9, 100e-9, 200e-9, 500e-9,
-        1e-6, 2e-6, 5e-6, 10e-6, 20e-6, 50e-6, 100e-6, 200e-6, 500e-6,
-        1e-3, 2e-3, 5e-3, 10e-3, 20e-3, 50e-3, 100e-3, 200e-3, 500e-3,
-        1.0, 2.0, 5.0, 10.0, 20.0, 50.0, 100.0  # seconds
+        1e-9,
+        2e-9,
+        5e-9,
+        10e-9,
+        20e-9,
+        50e-9,
+        100e-9,
+        200e-9,
+        500e-9,
+        1e-6,
+        2e-6,
+        5e-6,
+        10e-6,
+        20e-6,
+        50e-6,
+        100e-6,
+        200e-6,
+        500e-6,
+        1e-3,
+        2e-3,
+        5e-3,
+        10e-3,
+        20e-3,
+        50e-3,
+        100e-3,
+        200e-3,
+        500e-3,
+        1.0,
+        2.0,
+        5.0,
+        10.0,
+        20.0,
+        50.0,
+        100.0,  # seconds
     ]
 
     _trg_src = None
 
     # Time axis control
     @setter
     def set_horz_scale(self, scale: Float):
+        nearest_scale = find_nearest(self.horz_scales, scale, overestimate=True)
 
-        nearest_scale = find_nearest(
-            self.horz_scales, scale,
-            overestimate=True
-        )
-
-        self.write(f'TDIV {nearest_scale}S')
+        self.write(f"TDIV {nearest_scale}S")
 
         return nearest_scale
 
     @getter
     def get_horz_scale(self) -> Float:
-
-        return float(self.query('TDIV?').split('TDIV ')[-1][:-1])
-
+        return float(self.query("TDIV?").split("TDIV ")[-1][:-1])
 
     @setter
     def set_horz_position(self, position: Float):
-
-        self.write(f'TRDL {position}S')
+        self.write(f"TRDL {position}S")
 
     @getter
     def get_horz_position(self) -> Float:
-
-        return float(self.query('TRDL?').split('TRDL ')[-1][:-1])
+        return float(self.query("TRDL?").split("TRDL ")[-1][:-1])
 
     # Channel control base functions
     def _set_chn_scale(self, n, scale):
-
-        self.write('C%d:VDIV %.3eV' % (n, float(scale)))
+        self.write("C%d:VDIV %.3eV" % (n, float(scale)))
 
     def _get_chn_scale(self, n):
-
-        response = self.query('C%d:VDIV?' % n).split('C%d:VDIV ' % n)[-1][:-1]
+        response = self.query("C%d:VDIV?" % n).split("C%d:VDIV " % n)[-1][:-1]
 
         return float(response)
 
     def _set_chn_position(self, n, position):
-
-        self.write('C%d:OFST %.3eV' % (n, float(position)))
+        self.write("C%d:OFST %.3eV" % (n, float(position)))
 
     def _get_chn_position(self, n):
-
-        response = self.query('C%d:OFST?' % n).split('C%d:OFST ' % n)[-1][:-1]
+        response = self.query("C%d:OFST?" % n).split("C%d:OFST " % n)[-1][:-1]
 
         return float(response)
 
     # Channel 1 control
     @setter
     def set_ch1_scale(self, scale: Float):
         self._set_chn_scale(1, scale)
@@ -664,123 +671,110 @@
     @getter
     def get_ch4_position(self) -> Float:
         return self._get_chn_position(4)
 
     # Trigger control
     @setter
     def set_trigger_level(self, level: Float):
-
         trg_src = self.get_trigger_source()
 
-        self.write(f'C{trg_src}:TRLV {level}V')
+        self.write(f"C{trg_src}:TRLV {level}V")
 
     @getter
     def get_trigger_level(self) -> Float:
-
         trg_src = self.get_trigger_source()
 
-        return float(self.query(f'C{trg_src}:TRLV?').split('TRLV ')[-1][:-1])
+        return float(self.query(f"C{trg_src}:TRLV?").split("TRLV ")[-1][:-1])
 
     @setter
     def set_trigger_source(self, source: Integer):
-
-        self.write(f'TRSE EDGE,SR,C{int(source)},OFF')
+        self.write(f"TRSE EDGE,SR,C{int(source)},OFF")
 
     @getter
     def get_trigger_source(self) -> Integer:
-
-        return int(self.query('TRSE?').split('SR,C')[-1][0])
+        return int(self.query("TRSE?").split("SR,C")[-1][0])
 
     @setter
     def set_acquire_mode(self, mode: String):
-
-        if mode.upper() in ['SAMPLING', 'PEAK_DETECT', 'HIGH_RES']:
-            self.write(f'ACQW {mode.upper()}')
-        elif mode.upper() == 'AVERAGE':
-
-            if not hasattr(self, 'averages'):
+        if mode.upper() in ["SAMPLING", "PEAK_DETECT", "HIGH_RES"]:
+            self.write(f"ACQW {mode.upper()}")
+        elif mode.upper() == "AVERAGE":
+            if not hasattr(self, "averages"):
                 self.set_averages(4)
 
-            self.write(f'ACQW AVERAGE,{int(self.averages)}')
+            self.write(f"ACQW AVERAGE,{int(self.averages)}")
 
         else:
             return None
 
     @getter
     def get_acquire_mode(self) -> String:
+        response = self.query("ACQW?").split("ACQW ")[-1]
 
-        response = self.query('ACQW?').split('ACQW ')[-1]
-
-        if 'AVERAGE' in response:
-            return 'AVERAGE'
+        if "AVERAGE" in response:
+            return "AVERAGE"
         else:
             return response
 
     @setter
     def set_memory_size(self, size: Integer):
-
-        self.write(f'MSIZ {int(size)}')
+        self.write(f"MSIZ {int(size)}")
 
         return self.get_memory_size()
 
     @getter
     def get_memory_size(self) -> Integer:
+        response = self.query("MSIZ?").split("MSIZ ")[-1]
 
-        response = self.query('MSIZ?').split('MSIZ ')[-1]
-
-        if 'K' in response:
-            response = float(response.replace('K', 'e3'))
-        elif 'M' in response:
-            response = float(response.replace('M', 'e6'))
+        if "K" in response:
+            response = float(response.replace("K", "e3"))
+        elif "M" in response:
+            response = float(response.replace("M", "e6"))
 
         return int(response)
 
-
     @setter
     def set_averages(self, averages: Integer):
-
         valid = [4] + [2**i for i in range(4, 11)]
 
         averages = find_nearest(valid, averages)
 
-        self.write(f'AVGA {averages}')
+        self.write(f"AVGA {averages}")
 
     @getter
     def get_averages(self) -> Integer:
-        return int(self.query('AVGA?').split('AVGA ')[-1])
+        return int(self.query("AVGA?").split("AVGA ")[-1])
 
     # Channel measurements
     def _measure_chn_waveform(self, n):
-
         # Set trigger mode to NORMAL
-        if 'NORM' not in self.query('TRMD?'):
-            self.write('TRMD NORM')
+        if "NORM" not in self.query("TRMD?"):
+            self.write("TRMD NORM")
 
         # Wait for trigger
         triggered = False
         wait_time = 0.0
         while not triggered and wait_time < 30.0:
-            status = self.query('INR?')
-            triggered = status == 'INR 8193'
+            status = self.query("INR?")
+            triggered = status == "INR 8193"
             wait_time += 0.25
             time.sleep(0.25)
 
         if not triggered:
             return None
 
         # Enable channel if needed
-        channel_enabled = 'ON' in self.query('C%d:TRA?' % n)
+        channel_enabled = "ON" in self.query("C%d:TRA?" % n)
         if not channel_enabled:
-            self.write('C%d:TRA ON' % n)
+            self.write("C%d:TRA ON" % n)
             time.sleep(3)
 
-        self.write('WFSU SP,0,NP,0,FP,0')  # setup to get all data points
+        self.write("WFSU SP,0,NP,0,FP,0")  # setup to get all data points
 
         def is_terminated(message):
-
             try:
                 size = int(message[13:22])
             except ValueError:
                 return False
 
             data_length = len(message[22:-2])
 
@@ -798,51 +792,49 @@
 
             if response is None:
                 return False
             elif len(response) == 0:
                 return False
 
             header = response[:13]
-            if header != (b'C%d:WF DAT2,#9' % n):
+            if header != (b"C%d:WF DAT2,#9" % n):
                 return False
 
             size = response[13:22]
             try:
                 size = int(size)
             except ValueError:
                 return False
 
             data = response[22:-2]
             if len(data) != size:
                 return False
 
             termination = response[-2:]
-            if termination != b'\n\n':
+            if termination != b"\n\n":
                 return False
 
             return True
 
-        response = self.query(
-            'C%d:WF? DAT2' % n, decode=False, validator=validator
-        )
+        response = self.query("C%d:WF? DAT2" % n, decode=False, validator=validator)
 
-        self.adapter.read_termination = '\n'  # restore normal read termination
+        self.adapter.read_termination = "\n"  # restore normal read termination
 
-        self.write('TRMD NORM')  # set to single trigger mode
+        self.write("TRMD NORM")  # set to single trigger mode
 
         header, size, waveform = response[:13], response[13:22], response[22:-2]
         size = int(size)
 
         # convert bytes to integers
-        waveform = np.array(struct.unpack('b'*size, waveform), dtype=np.float64)
+        waveform = np.array(struct.unpack("b" * size, waveform), dtype=np.float64)
 
         scale = self._get_chn_scale(n)
         pos = self._get_chn_position(n)
 
-        waveform = (scale/25.0)*waveform - pos
+        waveform = (scale / 25.0) * waveform - pos
 
         return waveform
 
     @measurer
     def measure_ch1_waveform(self) -> Array:
         return self._measure_chn_waveform(1)
 
@@ -856,10 +848,8 @@
 
     @measurer
     def measure_ch4_waveform(self) -> Array:
         return self._measure_chn_waveform(4)
 
     @measurer
     def measure_sample_rate(self) -> Float:
-        return float(self.query('SARA?')[5:-4])
-
-
+        return float(self.query("SARA?")[5:-4])
```

### Comparing `empyric-0.2.0/empyric/collection/sourcemeters.py` & `empyric-0.2.3/empyric/collection/sourcemeters.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,982 +11,913 @@
 
 
 class Keithley2400(Instrument):
     """
     Keithley 2400 Sourcemeter, a 20 W power supply and picoammeter
     """
 
-    name = 'Keithley2400'
+    name = "Keithley2400"
 
-    supported_adapters = (
-        (GPIB, {'delay': 0.1, 'timeout': 0.5}),
-    )
+    supported_adapters = ((GPIB, {"delay": 0.1, "timeout": 0.5}),)
 
     # Available knobs
     knobs = (
-        'voltage',
-        'fast voltages',
-        'current',
-        'voltage range',
-        'voltage limit',
-        'current range',
-        'current limit',
-        'nplc',
-        'delay',
-        'output',
-        'source',
-        'meter',
-        'remote sense',
-        'source delay'
+        "voltage",
+        "fast voltages",
+        "current",
+        "voltage range",
+        "voltage limit",
+        "current range",
+        "current limit",
+        "nplc",
+        "delay",
+        "output",
+        "source",
+        "meter",
+        "remote sense",
+        "source delay",
     )
 
     presets = {
-        'source': 'voltage',
-        'meter': 'current',
-        'voltage': 0,
-        'output': 'ON',
-        'source_delay': 0,
+        "source": "voltage",
+        "meter": "current",
+        "voltage": 0,
+        "output": "ON",
+        "source_delay": 0,
     }
 
-    postsets = {
-        'voltage': 0,
-        'output': 'OFF'
-    }
+    postsets = {"voltage": 0, "output": "OFF"}
 
     # Available meters
-    meters = (
-        'voltage',
-        'current',
-        'fast currents'
-    )
+    meters = ("voltage", "current", "fast currents")
 
     fast_voltages = []
 
     #: allowed current range settings; zero indicate auto-range
-    current_ranges = (0.0, 1.e-6, 10.e-6, 100.e-6, 1.e-3, 10.e-3, 100.e-3, 1.)
+    current_ranges = (0.0, 1.0e-6, 10.0e-6, 100.0e-6, 1.0e-3, 10.0e-3, 100.0e-3, 1.0)
 
     #: allowed voltage range settings; zero indicates auto-range
-    voltage_ranges = (0.0, 0.2, 2., 20., 200.)
+    voltage_ranges = (0.0, 0.2, 2.0, 20.0, 200.0)
 
     #: over-voltage protection level settings
-    ovp_levels = (20., 40., 60., 80., 100., 120., 140., 160., 210.)
+    ovp_levels = (20.0, 40.0, 60.0, 80.0, 100.0, 120.0, 140.0, 160.0, 210.0)
 
     @setter
     def set_source(self, variable: String):
-
-        if variable not in ['voltage', 'current']:
+        if variable not in ["voltage", "current"]:
             raise ValueError('Source must be either "current" or "voltage"')
 
-        self.write(':SOUR:CLE:AUTO OFF')  # disable auto output-off
+        self.write(":SOUR:CLE:AUTO OFF")  # disable auto output-off
 
-        self.write(':SENS:FUNC:CONC OFF')  # disable concurrent measurements
+        self.write(":SENS:FUNC:CONC OFF")  # disable concurrent measurements
 
         # Disabling concurrent measurements sets instrument to measure voltage
         self.set_meter(self.meter)
 
-        self.set_output('OFF')
+        self.set_output("OFF")
 
-        if variable == 'voltage':
-            self.write(':SOUR:FUNC VOLT')
+        if variable == "voltage":
+            self.write(":SOUR:FUNC VOLT")
             self.current = None
 
-        if variable == 'current':
-            self.write(':SOUR:FUNC CURR')
+        if variable == "current":
+            self.write(":SOUR:FUNC CURR")
             self.voltage = None
 
     @getter
     def get_source(self) -> String:
-
-        if self.query('SOUR:FUNC?').strip() == 'VOLT':
-            return 'voltage'
+        if self.query("SOUR:FUNC?").strip() == "VOLT":
+            return "voltage"
         else:
-            return 'current'
+            return "current"
 
     @setter
     def set_meter(self, variable: String):
-
-        if variable not in ['voltage', 'current']:
+        if variable not in ["voltage", "current"]:
             raise ValueError('Source must be either "current" or "voltage"')
 
-        if variable == 'voltage':
+        if variable == "voltage":
             self.write(':SENS:FUNC "VOLT"')
-            self.write(':FORM:ELEM VOLT')
+            self.write(":FORM:ELEM VOLT")
 
-        if variable == 'current':
+        if variable == "current":
             self.write(':SENS:FUNC "CURR"')
-            self.write(':FORM:ELEM CURR')
+            self.write(":FORM:ELEM CURR")
 
-        self.write(':TRIG:COUN 1')
+        self.write(":TRIG:COUN 1")
 
     @getter
     def get_meter(self) -> String:
-        if self.query(':SENS:FUNC?').strip() == 'VOLT:DC':
-            return 'voltage'
+        if self.query(":SENS:FUNC?").strip() == "VOLT:DC":
+            return "voltage"
         else:
-            return 'current'
-
+            return "current"
 
     @setter
     def set_remote_sense(self, state: Toggle):
-
         self.set_output(OFF)
 
         if state.on:
-            self.write(':SYST:RSEN ON')
+            self.write(":SYST:RSEN ON")
         else:
-            self.write(':SYST:RSEN OFF')
+            self.write(":SYST:RSEN OFF")
 
     @getter
     def get_remote_sense(self) -> Toggle:
-
-        state = Toggle(self.query(':SYST:RSEN?').strip())
+        state = Toggle(self.query(":SYST:RSEN?").strip())
 
         return ON if state.on else OFF
 
     @setter
     def set_output(self, output: Toggle):
-
         if output:
-            self.write(':OUTP ON')
+            self.write(":OUTP ON")
         elif not output:
-            self.write(':OUTP OFF')
+            self.write(":OUTP OFF")
 
-            if not int(self.query(':OUTP?').strip()) == 0:
-                raise RuntimeWarning(
-                    f'unable to turn off output of {self.name}'
-                )
+            if not int(self.query(":OUTP?").strip()) == 0:
+                raise RuntimeWarning(f"unable to turn off output of {self.name}")
 
         else:
-            raise ValueError(f'Output setting {output} not recognized!')
+            raise ValueError(f"Output setting {output} not recognized!")
 
     @getter
     def get_output(self) -> Toggle:
-        return Toggle(self.query('OUTP?').strip())
+        return Toggle(self.query("OUTP?").strip())
 
     @measurer
     def measure_voltage(self) -> Float:
-
-        if self.meter != 'voltage':
-            self.set_meter('voltage')
+        if self.meter != "voltage":
+            self.set_meter("voltage")
 
         if not self.output:
             self.set_output(ON)
 
         def validator(response):
-            match = re.match('.\d\.\d+E.\d\d', response)
+            match = re.match(".\d\.\d+E.\d\d", response)
             return bool(match)
 
-        return float(self.query(':READ?', validator=validator))
+        return float(self.query(":READ?", validator=validator))
 
     @measurer
     def measure_current(self) -> Float:
-
-        if self.meter != 'current':
-            self.set_meter('current')
+        if self.meter != "current":
+            self.set_meter("current")
 
         if not self.output:
             self.set_output(ON)
 
         def validator(response):
-            match = re.match('.\d\.\d+E.\d\d', response)
+            match = re.match(".\d\.\d+E.\d\d", response)
             return bool(match)
 
-        return float(self.query(':READ?', validator=validator))
+        return float(self.query(":READ?", validator=validator))
 
     @setter
     def set_voltage(self, voltage: Float):
-
-        if self.source != 'voltage':
-            Warning(f'Switching source mode to voltage!')
-            self.set_source('voltage')
+        if self.source != "voltage":
+            Warning(f"Switching source mode to voltage!")
+            self.set_source("voltage")
 
         if not self.output:
             self.set_output(ON)
 
-        self.write(':SOUR:VOLT:LEV %.2E' % voltage)
+        self.write(":SOUR:VOLT:LEV %.2E" % voltage)
 
     @getter
     def get_voltage(self) -> Float:
-
-        return float(self.query(':SOUR:VOLT:LEV?'))
+        return float(self.query(":SOUR:VOLT:LEV?"))
 
     @setter
     def set_current(self, current: Float):
-
-        if self.source != 'current':
-            Warning(f'Switching source mode to current!')
-            self.set_source('current')
+        if self.source != "current":
+            Warning(f"Switching source mode to current!")
+            self.set_source("current")
 
         if not self.output:
-            self.set_output('ON')
+            self.set_output("ON")
 
-        self.write(':SOUR:CURR:LEV %.2E' % current)
+        self.write(":SOUR:CURR:LEV %.2E" % current)
 
     @getter
     def get_current(self) -> Float:
-
-        return float(self.query(':SOUR:CURR:LEV?').strip())
+        return float(self.query(":SOUR:CURR:LEV?").strip())
 
     @setter
     def set_voltage_range(self, voltage_range: Float):
-
         if voltage_range in self.voltage_ranges:
-            if self.source == 'voltage':
-                self.write(':SOUR:VOLT:RANGE %.2E' % voltage_range)
+            if self.source == "voltage":
+                self.write(":SOUR:VOLT:RANGE %.2E" % voltage_range)
             else:
                 if voltage_range == 0.0:
-                    self.write(':SENS:VOLT:RANGE: AUTO ON')
+                    self.write(":SENS:VOLT:RANGE: AUTO ON")
                 else:
-                    self.write(':SENS:VOLT:RANGE %.2E' % voltage_range)
+                    self.write(":SENS:VOLT:RANGE %.2E" % voltage_range)
         else:
-            first_line = f'Given voltage range {voltage_range} ' \
-                         f'is not a valid value for {self.name}\n'
-            second_line = f'Valid values are {self.voltage_ranges}'
+            first_line = (
+                f"Given voltage range {voltage_range} "
+                f"is not a valid value for {self.name}\n"
+            )
+            second_line = f"Valid values are {self.voltage_ranges}"
             raise ValueError(first_line + second_line)
 
     @getter
     def get_voltage_range(self) -> Float:
-
-        if not hasattr(self, 'source'):
+        if not hasattr(self, "source"):
             self.get_source()
 
-        if self.source == 'voltage':
-
-            if Toggle(self.query(':SOUR:VOLT:RANGE:AUTO?').strip()):
+        if self.source == "voltage":
+            if Toggle(self.query(":SOUR:VOLT:RANGE:AUTO?").strip()):
                 return 0.0
             else:
-                return float(self.query(':SOUR:VOLT:RANG?').strip())
+                return float(self.query(":SOUR:VOLT:RANG?").strip())
 
         else:
-            if Toggle(self.query(':SENS:VOLT:RANGE:AUTO?').strip()):
+            if Toggle(self.query(":SENS:VOLT:RANGE:AUTO?").strip()):
                 return 0.0
             else:
-                return float(self.query(':SENS:VOLT:RANG?').strip())
+                return float(self.query(":SENS:VOLT:RANG?").strip())
 
     @setter
     def set_voltage_limit(self, voltage_limit: Float):
-
-        if not hasattr(self, 'source'):
+        if not hasattr(self, "source"):
             self.get_source()
 
-        if self.source == 'voltage':
+        if self.source == "voltage":
             if voltage_limit in self.ovp_levels:
-                self.write(':SOUR:VOLT:PROT %d' % int(voltage_limit))
+                self.write(":SOUR:VOLT:PROT %d" % int(voltage_limit))
             else:
-                first_line = f'{self.name} is sourcing voltage, but given ' \
-                             f'voltage limit {voltage_limit} ' \
-                             f'is not a valid value\n'
-                second_line = f'Valid values are {self.ovp_levels}'
+                first_line = (
+                    f"{self.name} is sourcing voltage, but given "
+                    f"voltage limit {voltage_limit} "
+                    f"is not a valid value\n"
+                )
+                second_line = f"Valid values are {self.ovp_levels}"
                 raise ValueError(first_line + second_line)
         else:
-            self.write(':SENS:VOLT:PROT %.2E' % voltage_limit)
+            self.write(":SENS:VOLT:PROT %.2E" % voltage_limit)
 
     @getter
     def get_voltage_limit(self) -> Float:
-
-        if not hasattr(self, 'source'):
+        if not hasattr(self, "source"):
             self.get_source()
 
-        if self.source == 'voltage':
-            return float(self.query(':SOUR:VOLT:PROT?').strip())
+        if self.source == "voltage":
+            return float(self.query(":SOUR:VOLT:PROT?").strip())
         else:
-            return float(self.query(':SENS:VOLT:PROT?').strip())
+            return float(self.query(":SENS:VOLT:PROT?").strip())
 
     @setter
     def set_current_range(self, current_range: Float):
-
         if current_range in self.current_ranges:
-            if self.source == 'current':
-                self.write(':SOUR:CURR:RANGE %.2E' % current_range)
+            if self.source == "current":
+                self.write(":SOUR:CURR:RANGE %.2E" % current_range)
             else:
                 if current_range == 0.0:
-                    self.write(':SENS:CURR:RANGE AUTO')
+                    self.write(":SENS:CURR:RANGE AUTO")
                 else:
-                    self.write(':SENS:CURR:RANGE %.2E' % current_range)
+                    self.write(":SENS:CURR:RANGE %.2E" % current_range)
         else:
-            first_line = f'Given current range {current_range} ' \
-                         f'is not a valid value for {self.name}\n'
-            second_line = f'Valid values are {self.current_ranges}'
+            first_line = (
+                f"Given current range {current_range} "
+                f"is not a valid value for {self.name}\n"
+            )
+            second_line = f"Valid values are {self.current_ranges}"
             raise ValueError(first_line + second_line)
 
     @getter
     def get_current_range(self) -> Float:
-
-        if not hasattr(self, 'source'):
+        if not hasattr(self, "source"):
             self.get_source()
 
-        if self.source == 'current':
-
-            if Toggle(self.query(':SOUR:CURR:RANGE:AUTO?').strip()):
+        if self.source == "current":
+            if Toggle(self.query(":SOUR:CURR:RANGE:AUTO?").strip()):
                 return 0.0
             else:
-                return float(self.query(':SOUR:CURR:RANG?').strip())
+                return float(self.query(":SOUR:CURR:RANG?").strip())
 
         else:
-            if Toggle(self.query(':SENS:CURR:RANGE:AUTO?').strip()):
+            if Toggle(self.query(":SENS:CURR:RANGE:AUTO?").strip()):
                 return 0.0
             else:
-                return float(self.query(':SENS:CURR:RANG?').strip())
+                return float(self.query(":SENS:CURR:RANG?").strip())
 
     @setter
     def set_current_limit(self, current_limit: Float):
-        self.write(':SENS:CURR:PROT %.2E' % current_limit)
+        self.write(":SENS:CURR:PROT %.2E" % current_limit)
 
     @getter
     def get_current_limit(self) -> Float:
-
-        if self.source == 'current':
-            return float(self.query(':SOUR:CURR:PROT?'.strip()))
+        if self.source == "current":
+            return float(self.query(":SOUR:CURR:PROT?".strip()))
         else:
-            return float(self.query(':SENS:CURR:PROT?').strip())
+            return float(self.query(":SENS:CURR:PROT?").strip())
 
     @setter
     def set_nplc(self, nplc: Float):
-
-        if self.meter == 'current':
-            self.write(':SENS:CURR:NPLC %.2E' % nplc)
-        elif self.meter == 'voltage':
-            self.write(':SENS:VOLT:NPLC %.2E' % nplc)
+        if self.meter == "current":
+            self.write(":SENS:CURR:NPLC %.2E" % nplc)
+        elif self.meter == "voltage":
+            self.write(":SENS:VOLT:NPLC %.2E" % nplc)
 
     @getter
     def get_nplc(self) -> Float:
-
-        if not hasattr(self, 'meter'):
+        if not hasattr(self, "meter"):
             self.get_meter()
 
-        if self.meter == 'current':
-            return float(self.query(':SENS:CURR:NPLC?'))
-        elif self.meter == 'voltage':
-            return float(self.query(':SENS:VOLT:NPLC?'))
+        if self.meter == "current":
+            return float(self.query(":SENS:CURR:NPLC?"))
+        elif self.meter == "voltage":
+            return float(self.query(":SENS:VOLT:NPLC?"))
 
     @setter
     def set_delay(self, delay: Float):
         self.adapter.delay = delay
 
     @getter
     def get_delay(self) -> Float:
         return self.adapter.delay
 
     @setter
     def set_fast_voltages(self, voltages: [Array, String]):
-
         # import fast voltages, if specified as a path
         if type(voltages) == str:
-
-            is_csv = '.csv' in voltages.lower()
+            is_csv = ".csv" in voltages.lower()
             is_file = os.path.isfile(voltages)
 
             if not is_csv or not is_file:
                 raise ValueError(
-                    f'invalid fast voltages path for {self.name}; '
-                    'a 1D numerical array or valid path to CSV file must be '
-                    'provided.'
+                    f"invalid fast voltages path for {self.name}; "
+                    "a 1D numerical array or valid path to CSV file must be "
+                    "provided."
                 )
 
             voltage_data = pd.read_csv(voltages)
 
             columns = voltage_data.columns
 
             # Look for matching column name
             named = np.intersect1d(
-                ['Voltage', 'Fast Voltage', 'Voltages', 'Fast Voltages'],
-                columns
+                ["Voltage", "Fast Voltage", "Voltages", "Fast Voltages"], columns
             )
 
             if named:
                 voltages = voltage_data[named[0]].values
             else:
                 # If no matching column name, take the first column
                 voltages = voltage_data[columns[0]].values
 
         if np.ndim(voltages) == 1:
             return np.array(voltages, dtype=float)  # --> self.fast_voltages
         else:
-            raise ValueError(f'invalid fast voltages: {voltages}')
+            raise ValueError(f"invalid fast voltages: {voltages}")
 
     @measurer
     def measure_fast_currents(self) -> Array:
+        self._busy = True
 
         list_length = len(self.fast_voltages)
 
         if list_length == 0:
-            raise ValueError(
-                f'fast voltages for {self.name} have not been set'
-            )
+            raise ValueError(f"fast voltages for {self.name} have not been set")
         elif list_length <= 100:
             sub_lists = []
         else:  # instrument can only store 100 voltages
             sub_lists = [
-                self.fast_voltages[i * 100:(i + 1) * 100]
+                self.fast_voltages[i * 100 : (i + 1) * 100]
                 for i in range(list_length // 100)
             ]
 
         if list_length % 100 > 0:
-            sub_lists.append(self.fast_voltages[-(list_length % 100):])
+            sub_lists.append(self.fast_voltages[-(list_length % 100) :])
 
-        self.set_meter('current')
+        self.set_meter("current")
 
         current_list = []
 
-        normal_timeout = self.adapter.timeout
-        self.adapter.timeout = None  # the response times can be long
-
-        self.set_source('voltage')
-        self.set_meter('current')
-        self.set_output('ON')
-        self.write(':SOUR:VOLT:MODE LIST')
+        self.set_source("voltage")
+        self.set_meter("current")
+        self.set_output("ON")
+        self.write(":SOUR:VOLT:MODE LIST")
 
         for voltage_list in sub_lists:
-            voltage_str = ', '.join(
-                ['%.4E' % voltage for voltage in voltage_list]
-            )
+            voltage_str = ", ".join(["%.4E" % voltage for voltage in voltage_list])
 
-            self.write(':SOUR:LIST:VOLT ' + voltage_str)
-            self.write(':TRIG:COUN %d' % len(voltage_list))
+            self.write(":SOUR:LIST:VOLT " + voltage_str)
+            self.write(":TRIG:COUN %d" % len(voltage_list))
 
-            raw_response = self.query(':READ?').strip()
-            current_list += [
-                float(current_str) for current_str in raw_response.split(',')
-            ]
+            raw_response = self.query(":READ?", timeout=60)
 
-        self.adapter.timeout = normal_timeout  # put it back
+            if raw_response is not None:
+                raw_response = raw_response.strip()
 
-        self.write(':SOUR:VOLT:MODE FIX')
-        self.write(':TRIG:COUN 1')
+                current_list += [
+                    float(current_str) for current_str in raw_response.split(",")
+                ]
+
+            else:
+                # truncated data; nullify measurement
+                current_list = [np.nan for _ in self.fast_voltages]
+                break
+
+        self.write(":SOUR:VOLT:MODE FIX")
+        self.write(":TRIG:COUN 1")
+
+        self._busy = False
 
         return np.array(current_list)
 
     @setter
     def set_source_delay(self, delay: Float):
-        self.write(':SOUR:DEL %.4E' % delay)
+        self.write(":SOUR:DEL %.4E" % delay)
 
     @getter
     def get_source_delay(self) -> Float:
-        return self.query(':SOUR:DEL?').strip()
+        response = self.query(":SOUR:DEL?")
+
+        if response is not None:
+            return response.strip()
 
 
 class Keithley2460(Instrument):
     """
     Keithley 2460 Sourcemeter, a 100 W power supply and picoammeter
     """
 
-    name = 'Keithley2460'
+    name = "Keithley2460"
 
-    supported_adapters = (
-        (GPIB, {}),
-    )
+    supported_adapters = ((GPIB, {}),)
 
     # Available knobs
     knobs = (
-        'voltage',
-        'fast voltages',
-        'current',
-        'voltage range',
-        'voltage limit',
-        'current range',
-        'current limit',
-        'nplc',
-        'delay',
-        'output',
-        'source',
-        'meter',
-        'remote sense',
-        'source delay'
+        "voltage",
+        "fast voltages",
+        "current",
+        "voltage range",
+        "voltage limit",
+        "current range",
+        "current limit",
+        "nplc",
+        "delay",
+        "output",
+        "source",
+        "meter",
+        "remote sense",
+        "source delay",
     )
 
     presets = {
-        'source': 'voltage',
-        'meter': 'current',
-        'voltage': 0,
-        'output': 'ON',
-        'nplc': 1,
-        'source delay': 0,
-        'remote sense': 'OFF'
+        "source": "voltage",
+        "meter": "current",
+        "voltage": 0,
+        "output": "ON",
+        "nplc": 1,
+        "source delay": 0,
+        "remote sense": "OFF",
     }
 
-    postsets = {
-        'voltage': 0,
-        'output': 'OFF'
-    }
+    postsets = {"voltage": 0, "output": "OFF"}
 
     # Available meters
-    meters = (
-        'voltage',
-        'current',
-        'fast currents'
-    )
+    meters = ("voltage", "current", "fast currents")
 
     fast_voltages = None
 
     current_ranges = (1e-6, 10e-6, 100e-6, 1e-3, 10e-3, 100e-3, 1, 4, 5, 7)
     voltage_ranges = (0.2, 2, 7, 10, 20, 100)
     ovp_levels = (2, 5, 10, 20, 40, 60, 80, 100, 120, 140, 160, 180)
 
     @setter
     def set_source(self, variable):
-
-        if variable not in ['voltage', 'current']:
+        if variable not in ["voltage", "current"]:
             raise ValueError('Source must be either "current" or "voltage"')
 
-        self.set_output('OFF')
+        self.set_output("OFF")
 
-        if variable == 'voltage':
-            self.write('SOUR:FUNC VOLT')
+        if variable == "voltage":
+            self.write("SOUR:FUNC VOLT")
             self.current = None
 
-        if variable == 'current':
-            self.write('SOUR:FUNC CURR')
+        if variable == "current":
+            self.write("SOUR:FUNC CURR")
             self.voltage = None
 
     @setter
     def set_meter(self, variable):
-
-        if variable == 'voltage':
+        if variable == "voltage":
             self.write('SENS:FUNC "VOLT"')
-            self.write('DISP:VOLT:DIG 5')
-        elif variable == 'current':
+            self.write("DISP:VOLT:DIG 5")
+        elif variable == "current":
             self.write('SENS:FUNC "CURR"')
-            self.write('DISP:CURR:DIG 5')
+            self.write("DISP:CURR:DIG 5")
         else:
             raise ValueError('Source must be either "current" or "voltage"')
 
     @setter
     def set_output(self, output):
-
-        if output in [0, 'OFF', 'off']:
-            self.write(':OUTP OFF')
-        elif output in [1, 'ON', 'on']:
-            self.write(':OUTP ON')
+        if output in [0, "OFF", "off"]:
+            self.write(":OUTP OFF")
+        elif output in [1, "ON", "on"]:
+            self.write(":OUTP ON")
         else:
-            raise ValueError(f'Output setting {output} not recognized!')
+            raise ValueError(f"Output setting {output} not recognized!")
 
     @measurer
     def measure_voltage(self):
+        if self.meter != "voltage":
+            self.set_meter("voltage")
 
-        if self.meter != 'voltage':
-            self.set_meter('voltage')
-
-        if self.output == 'ON':
-            return float(self.query('READ?').strip())
+        if self.output == "ON":
+            return float(self.query("READ?").strip())
         else:
             return np.nan
 
     @measurer
     def measure_current(self):
+        if self.meter != "current":
+            self.set_meter("current")
 
-        if self.meter != 'current':
-            self.set_meter('current')
-
-        if self.output == 'ON':
-            return float(self.query('READ?').strip())
+        if self.output == "ON":
+            return float(self.query("READ?").strip())
         else:
             return 0
 
     @setter
     def set_voltage(self, voltage):
-
-        if self.source != 'voltage':
-            Warning(f'Switching sourcing mode to voltage!')
-            self.set_source('voltage')
+        if self.source != "voltage":
+            Warning(f"Switching sourcing mode to voltage!")
+            self.set_source("voltage")
 
             # turn output on if shut off when the source mode is changed
-            self.set_output('ON')
+            self.set_output("ON")
 
-        self.write('SOUR:VOLT:LEV %.4E' % voltage)
+        self.write("SOUR:VOLT:LEV %.4E" % voltage)
 
     @setter
     def set_current(self, current):
-
-        if self.source != 'current':
-            Warning(f'Switching sourcing mode to current!')
-            self.set_source('current')
+        if self.source != "current":
+            Warning(f"Switching sourcing mode to current!")
+            self.set_source("current")
 
             # turn output on if shut off when the source mode is changed
-            self.set_output('ON')
+            self.set_output("ON")
 
-        self.write('SOUR:CURR:LEV %.4E' % current)
+        self.write("SOUR:CURR:LEV %.4E" % current)
 
     @setter
     def set_voltage_range(self, voltage_range):
-
         if voltage_range in self.voltage_ranges:
-            if self.source == 'voltage':
-                self.write(':SOUR:VOLT:RANGE %.2E' % voltage_range)
+            if self.source == "voltage":
+                self.write(":SOUR:VOLT:RANGE %.2E" % voltage_range)
             else:
-                if voltage_range == 'AUTO':
-                    self.write(':SENS:VOLT:RANGE:AUTO ON')
+                if voltage_range == "AUTO":
+                    self.write(":SENS:VOLT:RANGE:AUTO ON")
                 else:
-                    self.write(':SENS:VOLT:RANGE %.2E' % voltage_range)
+                    self.write(":SENS:VOLT:RANGE %.2E" % voltage_range)
         else:
-            first_line = f'Given voltage range {voltage_range} ' \
-                         f'is not a valid value for {self.name}\n'
-            second_line = f'Valid values are {self.voltage_ranges}'
+            first_line = (
+                f"Given voltage range {voltage_range} "
+                f"is not a valid value for {self.name}\n"
+            )
+            second_line = f"Valid values are {self.voltage_ranges}"
             raise ValueError(first_line + second_line)
 
     @setter
     def set_voltage_limit(self, voltage_limit):
-
-        if self.source == 'voltage':
+        if self.source == "voltage":
             if int(voltage_limit) in self.ovp_levels:
-                self.write(':SOUR:VOLT:PROT PROT%d' % int(voltage_limit))
+                self.write(":SOUR:VOLT:PROT PROT%d" % int(voltage_limit))
             else:
-                first_line = f'{self.name} is sourcing voltage, but given ' \
-                             f'voltage limit {voltage_limit} ' \
-                             f'is not a valid value\n'
-                second_line = f'Valid values are {self.ovp_levels}'
+                first_line = (
+                    f"{self.name} is sourcing voltage, but given "
+                    f"voltage limit {voltage_limit} "
+                    f"is not a valid value\n"
+                )
+                second_line = f"Valid values are {self.ovp_levels}"
                 raise ValueError(first_line + second_line)
         else:
-            self.write(':SOUR:CURR:VLIM %.2E' % voltage_limit)
+            self.write(":SOUR:CURR:VLIM %.2E" % voltage_limit)
 
     @setter
     def set_current_range(self, current_range):
-
         if current_range in self.current_ranges:
-            if self.source == 'current':
-                self.write(':SOUR:CURR:RANGE %.2E' % current_range)
+            if self.source == "current":
+                self.write(":SOUR:CURR:RANGE %.2E" % current_range)
             else:
-                if current_range == 'AUTO':
-                    self.write(':SENS:CURR:RANGE:AUTO ON')
+                if current_range == "AUTO":
+                    self.write(":SENS:CURR:RANGE:AUTO ON")
                 else:
-                    self.write(':SENS:CURR:RANGE %.2E' % current_range)
+                    self.write(":SENS:CURR:RANGE %.2E" % current_range)
         else:
-            first_line = f'Given current range {current_range} ' \
-                         f'is not a valid value for {self.name}\n'
-            second_line = f'Valid values are {self.current_ranges}'
+            first_line = (
+                f"Given current range {current_range} "
+                f"is not a valid value for {self.name}\n"
+            )
+            second_line = f"Valid values are {self.current_ranges}"
             raise ValueError(first_line + second_line)
 
     @setter
     def set_current_limit(self, current_limit):
-        self.write(':SOUR:VOLT:ILIM %.2E' % current_limit)
+        self.write(":SOUR:VOLT:ILIM %.2E" % current_limit)
 
     @setter
     def set_nplc(self, nplc):
-
-        if self.meter == 'current':
-            self.write('CURR:NPLC %.2E' % nplc)
-        elif self.meter == 'voltage':
-            self.write('VOLT:NPLC %.2E' % nplc)
+        if self.meter == "current":
+            self.write("CURR:NPLC %.2E" % nplc)
+        elif self.meter == "voltage":
+            self.write("VOLT:NPLC %.2E" % nplc)
 
     @setter
     def set_delay(self, delay):
         self.adapter.delay = delay
 
     @setter
     def set_fast_voltages(self, voltages):
-
         Keithley2400.set_fast_voltages(self, voltages)
 
     @measurer
     def measure_fast_currents(self):
-
         try:
             self.fast_voltages
         except AttributeError:
-            raise ValueError('Fast IV sweep voltages have not been set!')
+            raise ValueError("Fast IV sweep voltages have not been set!")
 
         if len(self.fast_voltages) == 0:
-            raise ValueError('Fast IV sweep voltages have not been set!')
+            raise ValueError("Fast IV sweep voltages have not been set!")
 
-        path = self.name + '-fast_iv_measurement.csv'
+        path = self.name + "-fast_iv_measurement.csv"
 
         list_length = len(self.fast_voltages)
 
         if list_length >= 100:
             sub_lists = [
-                self.fast_voltages[i * 100:(i + 1) * 100]
+                self.fast_voltages[i * 100 : (i + 1) * 100]
                 for i in range(list_length // 100)
             ]
         else:
             sub_lists = []
 
         if list_length % 100 > 0:
-            sub_lists.append(self.fast_voltages[-(list_length % 100):])
+            sub_lists.append(self.fast_voltages[-(list_length % 100) :])
 
         current_list = []
 
         normal_timeout = self.adapter.timeout
         self.adapter.timeout = None  # the response times can be long
 
         start = datetime.datetime.now()
         for voltage_list in sub_lists:
-            voltage_str = ', '.join(
-                ['%.4E' % voltage for voltage in voltage_list]
-            )
-            self.write('SOUR:LIST:VOLT ' + voltage_str)
-            self.write('SOUR:SWE:VOLT:LIST 1, %.2e' % self.source_delay)
-            self.write('INIT')
-            self.write('*WAI')
+            voltage_str = ", ".join(["%.4E" % voltage for voltage in voltage_list])
+            self.write("SOUR:LIST:VOLT " + voltage_str)
+            self.write("SOUR:SWE:VOLT:LIST 1, %.2e" % self.source_delay)
+            self.write("INIT")
+            self.write("*WAI")
             raw_response = self.query(
                 'TRAC:DATA? 1, %d, "defbuffer1", SOUR, READ' % len(voltage_list)
             ).strip()
 
             current_list += [
-                float(current_str)
-                for current_str in raw_response.split(',')[1::2]
+                float(current_str) for current_str in raw_response.split(",")[1::2]
             ]
 
         self.adapter.timeout = normal_timeout  # put it back
         end = datetime.datetime.now()
 
         return np.array(current_list)
 
     @setter
     def set_source_delay(self, delay):
-
-        if self.source == 'voltage':
-            self.write('SOUR:VOLT:DEL %.4e' % delay)
+        if self.source == "voltage":
+            self.write("SOUR:VOLT:DEL %.4e" % delay)
         else:
-            self.write('SOUR:CURR:DEL %.4e' % delay)
+            self.write("SOUR:CURR:DEL %.4e" % delay)
 
     @setter
     def set_remote_sense(self, state):
-        if bool(state) or state in ['ON', '1']:
-            self.write('VOLT:RSEN ON')
+        if bool(state) or state in ["ON", "1"]:
+            self.write("VOLT:RSEN ON")
         else:
-            self.write('VOLT:RSEN OFF')
+            self.write("VOLT:RSEN OFF")
 
-        self.set_output('ON')
+        self.set_output("ON")
 
     @getter
     def get_remote_sense(self):
-        if int(self.query('VOLT:RSEN?').strip()):
-            return 'ON'
+        if int(self.query("VOLT:RSEN?").strip()):
+            return "ON"
         else:
-            return 'OFF'
+            return "OFF"
 
 
 class Keithley2651A(Instrument):
     """
     Keithley 2651A High Power (200 W) Sourcemeter
     """
 
-    name = 'Keithley2651A'
+    name = "Keithley2651A"
 
-    supported_adapters = (
-        (GPIB, {}),
-    )
+    supported_adapters = ((GPIB, {}),)
 
     # Available knobs
     knobs = (
-        'voltage',
-        'fast voltages',
-        'current',
-        'voltage range',
-        'voltage limit',
-        'current range',
-        'current limit',
-        'nplc',
-        'output',
-        'source',
-        'meter',
-        'source delay'
+        "voltage",
+        "fast voltages",
+        "current",
+        "voltage range",
+        "voltage limit",
+        "current range",
+        "current limit",
+        "nplc",
+        "output",
+        "source",
+        "meter",
+        "source delay",
     )
 
     presets = {
-        'voltage range': 40,
-        'current range': 5,
-        'voltage': 0,
-        'output': 'ON',
-        'nplc': 1,
-        'source': 'voltage',
-        'meter': 'current',
-        'source_delay': 0
+        "voltage range": 40,
+        "current range": 5,
+        "voltage": 0,
+        "output": "ON",
+        "nplc": 1,
+        "source": "voltage",
+        "meter": "current",
+        "source_delay": 0,
     }
 
-    postsets = {
-        'voltage': 0,
-        'output': 'OFF'
-    }
+    postsets = {"voltage": 0, "output": "OFF"}
 
     # Available meters
-    meters = (
-        'voltage',
-        'current',
-        'fast currents'
-    )
+    meters = ("voltage", "current", "fast currents")
 
     fast_voltages = None
 
     @setter
     def set_source(self, variable):
-
-        if variable == 'voltage':
-            self.write('smua.source.func =  smua.OUTPUT_DCVOLTS')
-        elif variable == 'current':
-            self.write('smua.source.func = smua.OUTPUT_DCAMPS')
+        if variable == "voltage":
+            self.write("smua.source.func =  smua.OUTPUT_DCVOLTS")
+        elif variable == "current":
+            self.write("smua.source.func = smua.OUTPUT_DCAMPS")
         else:
             raise ValueError('source must be either "current" or "voltage"')
 
     @setter
     def set_meter(self, variable):
+        self.write("display.screen = display.SMUA")
 
-        self.write('display.screen = display.SMUA')
-
-        if variable == 'current':
-            self.write('display.smua.measure.func = display.MEASURE_DCAMPS')
+        if variable == "current":
+            self.write("display.smua.measure.func = display.MEASURE_DCAMPS")
 
-        if variable == 'voltage':
-            self.write('display.smua.measure.func = display.MEASURE_DCVOLTS')
+        if variable == "voltage":
+            self.write("display.smua.measure.func = display.MEASURE_DCVOLTS")
 
         # This sourcemeter does not require specifying the meter
         # before taking a measurement
 
     @setter
     def set_output(self, output):
-
-        if output in [0, 'OFF', 'off']:
-            self.write('smua.source.output = smua.OUTPUT_OFF')
-        elif output in [1, 'ON', 'on']:
-            self.write('smua.source.output = smua.OUTPUT_ON')
+        if output in [0, "OFF", "off"]:
+            self.write("smua.source.output = smua.OUTPUT_OFF")
+        elif output in [1, "ON", "on"]:
+            self.write("smua.source.output = smua.OUTPUT_ON")
         else:
-            raise ValueError(f'Ouput setting {output} not recognized!')
+            raise ValueError(f"Ouput setting {output} not recognized!")
 
     @measurer
     def measure_voltage(self):
+        if self.meter != "voltage":
+            self.set_meter("voltage")
 
-        if self.meter != 'voltage':
-            self.set_meter('voltage')
-
-        if self.output == 'ON':
-            return float(self.query('print(smua.measure.v())').strip())
+        if self.output == "ON":
+            return float(self.query("print(smua.measure.v())").strip())
         else:
             return np.nan
 
     @measurer
     def measure_current(self):
+        if self.meter != "current":
+            self.set_meter("current")
 
-        if self.meter != 'current':
-            self.set_meter('current')
-
-        if self.output == 'ON':
-            return float(self.query('print(smua.measure.i())').strip())
+        if self.output == "ON":
+            return float(self.query("print(smua.measure.i())").strip())
         else:
             return 0
 
     @measurer
     def set_voltage(self, voltage):
-
-        if self.source != 'voltage':
-            Warning(f'Switching sourcing mode!')
-            self.set_source('voltage')
+        if self.source != "voltage":
+            Warning(f"Switching sourcing mode!")
+            self.set_source("voltage")
 
             # turn output on if shut off when the source mode is changed
-            self.set_output('ON')
+            self.set_output("ON")
 
-        self.write(f'smua.source.levelv = {voltage}')
+        self.write(f"smua.source.levelv = {voltage}")
 
     @setter
     def set_current(self, current):
-
-        if self.source != 'current':
-            Warning(f'Switching sourcing mode!')
-            self.set_source('current')
+        if self.source != "current":
+            Warning(f"Switching sourcing mode!")
+            self.set_source("current")
 
             # turn output on if shut off when the source mode is changed
-            self.set_output('ON')
+            self.set_output("ON")
 
-        self.write(f'smua.source.leveli = {current}')
+        self.write(f"smua.source.leveli = {current}")
 
     @setter
     def set_voltage_range(self, voltage_range):
-
-        if voltage_range == 'auto':
-            self.write('smua.source.autorangev = smua.AUTORANGE_ON')
+        if voltage_range == "auto":
+            self.write("smua.source.autorangev = smua.AUTORANGE_ON")
         else:
-            self.write(f'smua.source.rangev = {voltage_range}')
+            self.write(f"smua.source.rangev = {voltage_range}")
 
     @setter
     def set_voltage_limit(self, voltage_limit):
-        self.write(f'smua.source.limitv = {voltage_limit}')
+        self.write(f"smua.source.limitv = {voltage_limit}")
 
     @setter
     def set_current_range(self, current_range):
-
-        if current_range == 'auto':
-            self.write('smua.source.autorangei = smua.AUTORANGE_ON')
+        if current_range == "auto":
+            self.write("smua.source.autorangei = smua.AUTORANGE_ON")
         else:
-            self.write(f'smua.source.rangei = {current_range}')
+            self.write(f"smua.source.rangei = {current_range}")
 
     @setter
     def set_current_limt(self, current_limit):
-        self.write(f'smua.source.limiti = {current_limit}')
+        self.write(f"smua.source.limiti = {current_limit}")
 
     @setter
     def set_nplc(self, nplc):
-        self.write(f'smua.measure.nplc = {nplc}')
+        self.write(f"smua.measure.nplc = {nplc}")
 
     @setter
     def set_fast_voltages(self, voltages):
         self.fast_voltages = voltages
 
         # import fast voltages, if specified as a path
         if type(self.fast_voltages) == str:  # can be specified as a path
             try:
                 fast_voltage_data = pd.read_csv(self.fast_voltages)
             except FileNotFoundError:
                 # probably in an experiment data directory; try going up a level
                 working_subdir = os.getcwd()
-                os.chdir('..')
+                os.chdir("..")
                 fast_voltage_data = pd.read_csv(self.fast_voltages)
                 os.chdir(working_subdir)
 
             columns = fast_voltage_data.columns
 
             fast_voltages = fast_voltage_data[columns[0]]
 
             self.fast_voltages = fast_voltages.astype(float).values
 
     @measurer
     def measure_fast_currents(self):
-
         try:
             if len(self.fast_voltages) == 0:
-                raise ValueError('Fast IV sweep voltages have not been set!')
+                raise ValueError("Fast IV sweep voltages have not been set!")
         except AttributeError:
-            raise ValueError('Fast IV sweep voltages have not been set!')
+            raise ValueError("Fast IV sweep voltages have not been set!")
 
         voltage_lists = []
         current_list = []
 
         list_length = 100  # maximum number of voltages to sweep at a time
 
         for i in range(len(self.fast_voltages) // list_length):
             voltage_lists.append(
-                self.fast_voltages[i * list_length:(i + 1) * list_length]
+                self.fast_voltages[i * list_length : (i + 1) * list_length]
             )
 
         remainder = len(self.fast_voltages) % list_length
         if remainder:
             voltage_lists.append(self.fast_voltages[-remainder:])
 
         normal_timeout = self.backend.timeout
         self.backend.timeout = 60  # give it up to a minute to do sweep
 
         for voltage_list in voltage_lists:
-            voltage_string = ', '.join(
-                [f'{voltage}' for voltage in voltage_list]
-            )
+            voltage_string = ", ".join([f"{voltage}" for voltage in voltage_list])
 
-            self.write('vlist = {%s}' % voltage_string)
-            self.write(
-                f'SweepVListMeasureI(smua, vlist, 0.01, {len(voltage_list)})'
-            )
+            self.write("vlist = {%s}" % voltage_string)
+            self.write(f"SweepVListMeasureI(smua, vlist, 0.01, {len(voltage_list)})")
             raw_response = self.query(
-                f'printbuffer(1, {len(voltage_list)}, smua.nvbuffer1)'
+                f"printbuffer(1, {len(voltage_list)}, smua.nvbuffer1)"
             ).strip()
             current_list += [
-                float(current_str) for current_str in raw_response.split(',')
+                float(current_str) for current_str in raw_response.split(",")
             ]
 
             # hold last voltage until next sub-sweep
             self.set_voltage(voltage_list[-1])
 
         self.connection.timeout = normal_timeout  # put it back
 
-        self.write('display.screen = display.SMUA')
-        self.write('display.smua.measure.func = display.MEASURE_DCAMPS')
+        self.write("display.screen = display.SMUA")
+        self.write("display.smua.measure.func = display.MEASURE_DCAMPS")
 
         return np.array(current_list)
 
     @setter
     def set_source_delay(self, delay):
-        self.write(f'smua.source.delay = {delay}')
+        self.write(f"smua.source.delay = {delay}")
```

### Comparing `empyric-0.2.0/empyric/collection/spectrometers.py` & `empyric-0.2.3/empyric/collection/spectrometers.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,145 +8,127 @@
 
 class SRSRGA(Instrument):
     """
     SRS Residual Gas Analyzer, a quadrupole mass spectrometer with mass ranges
     from 100 to 300 amu
     """
 
-    name = 'SRS-RGA'
+    name = "SRS-RGA"
 
     supported_adapters = (
-        (
-            Serial,
-            {'baud_rate': 28800, 'timeout': 300, 'read_termination': '\n\r'}
-        ),
+        (Serial, {"baud_rate": 28800, "timeout": 300, "read_termination": "\n\r"}),
     )
 
     knobs = (
-        'initialize'
-        'filament current',
-        'mass',
-        'masses',
-        'mass range',
-        'ppsf',  # partial pressure sensitivity factor
-        'tpsf'  # total pressure sensitivity factor
+        "initialize" "filament current",
+        "mass",
+        "masses",
+        "mass range",
+        "ppsf",  # partial pressure sensitivity factor
+        "tpsf",  # total pressure sensitivity factor
     )
 
-    presets = {
-        'filament current': 1
-    }
-
-    postsets = {
-        'filament current': 0
-    }
-
-    meters = {
-        'filament current',
-        'single',
-        'spectrum',
-        'total pressure'
-    }
+    presets = {"filament current": 1}
 
-    def __init__(self, *args, **kwargs):
+    postsets = {"filament current": 0}
+
+    meters = {"filament current", "single", "spectrum", "total pressure"}
 
+    def __init__(self, *args, **kwargs):
         Instrument.__init__(self, *args, **kwargs)
 
     @setter
     def set_filament_current(self, current: Float):
         # current is in mA
 
         if current >= 3.5:
-            self.query('FL3.5')
+            self.query("FL3.5")
         elif current <= 0:
-            self.query('FL0')
+            self.query("FL0")
         else:
-            self.query('FL'+f'{np.round(current, 2)}')
+            self.query("FL" + f"{np.round(current, 2)}")
 
         time.sleep(5)
 
     @measurer
     def measure_filament_current(self) -> Float:
-        return float(self.query('FL?'))
+        return float(self.query("FL?"))
 
     @setter
     def set_mass(self, mass: Integer):
-        self.write('ML' + f'{mass}')
+        self.write("ML" + f"{mass}")
 
     @getter
     def get_mass(self) -> Integer:
-        return int(self.query('ML?'))
+        return int(self.query("ML?"))
 
     @setter
     def set_masses(self, masses: Array):
         initial_mass, final_mass = masses[0], masses[-1]
 
-        self.write('MI' + f'{int(initial_mass)}')
-        self.write('MF' + f'{int(final_mass)}')
+        self.write("MI" + f"{int(initial_mass)}")
+        self.write("MF" + f"{int(final_mass)}")
 
         self.mass_range = [initial_mass, final_mass]
 
     @getter
     def get_masses(self) -> Array:
-
-        initial_mass = int(self.query('MI?'))
-        final_mass = int(self.query('MF?'))
+        initial_mass = int(self.query("MI?"))
+        final_mass = int(self.query("MF?"))
 
         self.mass_range = [initial_mass, final_mass]
 
         return np.arange(initial_mass, final_mass + 1, dtype=np.int64)
 
     @setter
     def set_mass_range(self, mass_range: Array):
-
         initial_mass, final_mass = mass_range
 
-        self.write('MI' + f'{int(initial_mass)}')
-        self.write('MF' + f'{int(final_mass)}')
+        self.write("MI" + f"{int(initial_mass)}")
+        self.write("MF" + f"{int(final_mass)}")
 
         self.masses = np.arange(initial_mass, final_mass + 1)
 
     @getter
     def get_mass_range(self) -> Array:
-        initial_mass = int(self.query('MI?'))
-        final_mass = int(self.query('MF?'))
+        initial_mass = int(self.query("MI?"))
+        final_mass = int(self.query("MF?"))
 
         self.masses = np.arange(initial_mass, final_mass + 1)
 
         return [initial_mass, final_mass]
 
-
     @setter
     def set_ppsf(self, value: Float):
-        self.write(f'SP{value}')
+        self.write(f"SP{value}")
 
     @getter
     def get_ppsf(self) -> Float:
-        return float(self.query('SP?'))
+        return float(self.query("SP?"))
 
     @setter
     def set_tpsf(self, value: Float):
-        self.write(f'ST{value}')
+        self.write(f"ST{value}")
 
     @getter
     def get_tpsf(self) -> Float:
-        return float(self.query('ST?'))
+        return float(self.query("ST?"))
 
     @measurer
     def measure_spectrum(self) -> Array:
-        response = self.query(
-            'HS1', num_bytes=4*(len(self.masses)+1), decode=False
+        response = self.query("HS1", num_bytes=4 * (len(self.masses) + 1), decode=False)
+        return (
+            np.array(struct.unpack("<" + "i" * (len(self.masses) + 1), response))[:-1]
+            * 1.0e-16
+            / self.ppsf
+            * 1000
         )
-        return np.array(
-            struct.unpack('<'+'i'*(len(self.masses)+1), response)
-        )[:-1] * 1.0e-16 / self.ppsf * 1000
 
     @measurer
     def measure_single(self) -> Float:
-        response = self.query(
-            'MR'+f'{int(self.mass)}', num_bytes=4, decode=False
-        )
-        return struct.unpack('<i', response)[0] * 1.0e-16 / self.ppsf * 1000
+        response = self.query("MR" + f"{int(self.mass)}", num_bytes=4, decode=False)
+        return struct.unpack("<i", response)[0] * 1.0e-16 / self.ppsf * 1000
 
     @measurer
     def measure_total_pressure(self) -> Float:
-        response = self.query('TP?', num_bytes=4, decode=False)
-        return struct.unpack('<i', response)[0] * 1.0e-16 / self.tpsf * 1000
+        response = self.query("TP?", num_bytes=4, decode=False)
+        return struct.unpack("<i", response)[0] * 1.0e-16 / self.tpsf * 1000
```

### Comparing `empyric-0.2.0/empyric/collection/supplies.py` & `empyric-0.2.3/empyric/collection/supplies.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,310 +4,250 @@
 
 
 class Keithley2260B(Instrument):
     """
     Keithley 2260B power supply, usually either 360 W or 720 W
     """
 
-    name = 'Keithley2260B'
+    name = "Keithley2260B"
 
-    supported_adapters = (
-        (Serial, {'baud_rate': 115200, 'write_termination': '\r\n'}),
-    )
+    supported_adapters = ((Serial, {"baud_rate": 115200, "write_termination": "\r\n"}),)
 
-    knobs = (
-        'max voltage',
-        'max current',
-        'output'
-    )
+    knobs = ("max voltage", "max current", "output")
 
     # no presets or postsets for this instrument
 
-    meters = (
-        'voltage',
-        'current'
-    )
+    meters = ("voltage", "current")
 
     @measurer
     def measure_current(self) -> Float:
-
         def validator(response):
-            return bool(re.match('[\+\-]\d+\.\d\d\d', response))
+            return bool(re.match("[\+\-]\d+\.\d\d\d", response))
 
-        return float(self.query('MEAS:CURR?', validator=validator))
+        return float(self.query("MEAS:CURR?", validator=validator))
 
     @measurer
     def measure_voltage(self) -> Float:
-
         def validator(response):
-            return bool(re.match('[\+\-]\d+\.\d\d\d', response))
+            return bool(re.match("[\+\-]\d+\.\d\d\d", response))
 
-        return float(self.query('MEAS:VOLT?', validator=validator))
+        return float(self.query("MEAS:VOLT?", validator=validator))
 
     @setter
     def set_max_voltage(self, voltage: Float):
-        self.write('VOLT %.4f' % voltage)
+        self.write("VOLT %.4f" % voltage)
 
     @setter
     def set_max_current(self, current: Float):
-        self.write('CURR %.4f' % current)
+        self.write("CURR %.4f" % current)
 
     @setter
     def set_output(self, output: Toggle):
-
         if output == ON:
-            self.write('OUTP:STAT:IMM ON')
+            self.write("OUTP:STAT:IMM ON")
         elif output == OFF:
-            self.write('OUTP:STAT:IMM OFF')
+            self.write("OUTP:STAT:IMM OFF")
 
     @getter
     def get_max_current(self) -> Float:
-
         def validator(response):
-            return bool(re.match('[\+\-]\d+\.\d\d\d', response))
+            return bool(re.match("[\+\-]\d+\.\d\d\d", response))
 
-        return float(self.query('CURR?', validator=validator))
+        return float(self.query("CURR?", validator=validator))
 
     @getter
     def get_max_voltage(self) -> Float:
-
         def validator(response):
-            return bool(re.match('[\+\-]\d+\.\d\d\d', response))
+            return bool(re.match("[\+\-]\d+\.\d\d\d", response))
 
-        return float(self.query('VOLT?', validator=validator))
+        return float(self.query("VOLT?", validator=validator))
 
 
 class BK9183B(Instrument):
     """
     B&K Precision Model 9183B (35V & 6A / 70V & 3A) power supply
     """
 
-    name = 'BK9183B'
+    name = "BK9183B"
 
-    supported_adapters = (
-        (Serial, {'baud_rate': 57600}),
-    )
-    
-    knobs = (
-        'max voltage',
-        'max current',
-        'output'
-    )
+    supported_adapters = ((Serial, {"baud_rate": 57600}),)
+
+    knobs = ("max voltage", "max current", "output")
 
     # no presets or postsets for this instrument
 
-    meters = (
-        'voltage',
-        'current'
-    )
+    meters = ("voltage", "current")
 
     @setter
     def set_output(self, output: Toggle):
-
         if output == ON:
-            self.write('OUT ON')
+            self.write("OUT ON")
         elif output == OFF:
-            self.write('OUT OFF')
+            self.write("OUT OFF")
 
     @measurer
     def measure_current(self):
         # sometimes the first measurement is lagged
-        return [float(self.query('MEAS:CURR?')) for i in range(3)][-1]
+        return [float(self.query("MEAS:CURR?")) for i in range(3)][-1]
 
     @measurer
     def measure_voltage(self):
         # sometimes the first measurement is lagged
-        return [float(self.query('MEAS:VOLT?')) for i in range(3)][-1]
+        return [float(self.query("MEAS:VOLT?")) for i in range(3)][-1]
 
     @setter
     def set_max_current(self, current):
-        self.write('SOUR:CURR ' + str(current))
+        self.write("SOUR:CURR " + str(current))
 
     @setter
     def set_max_voltage(self, voltage):
-        self.write('SOUR:VOLT ' + str(voltage))
+        self.write("SOUR:VOLT " + str(voltage))
 
     @getter
     def get_max_current(self):
-        return float(self.query('SOUR:CURR?'))
+        return float(self.query("SOUR:CURR?"))
 
     @getter
     def get_max_voltage(self):
-        return float(self.query('SOUR:VOLT?'))
+        return float(self.query("SOUR:VOLT?"))
 
 
 class UltraflexInductionHeater(Instrument):
     """UltraFlex Ultraheat S2 (or similar) 2 kW induction heater"""
 
     name = "UltraflexInductionHeater"
 
-    supported_adapters = (
-        (Serial, {})
-    )
+    supported_adapters = (Serial, {})
 
-    knobs = (
-        'power',
-        'output',
-        'mode'
-    )
+    knobs = ("power", "output", "mode")
 
     meters = (
-        'voltage',
-        'current',
-        'frequency',
+        "voltage",
+        "current",
+        "frequency",
     )
 
     @measurer
     def measure_current(self):
-        return 0.1 * float(self.query('S3i11K')[3:-3], 16)
+        return 0.1 * float(self.query("S3i11K")[3:-3], 16)
 
     @measurer
     def measure_voltage(self):
-        return float(self.query('S3v04K')[3:-3], 16)
+        return float(self.query("S3v04K")[3:-3], 16)
 
     @measurer
     def measure_frequency(self):
-        return 1e3 * float(self.query('S3f14K')[3:-3], 16)
+        return 1e3 * float(self.query("S3f14K")[3:-3], 16)
 
     @setter
     def set_power(self, percent_of_max):
-
         if percent_of_max < 0 or percent_of_max > 100:
             raise ValueError(
-                'power setting must be a percentage value between 0 and 100'
+                "power setting must be a percentage value between 0 and 100"
             )
 
-        ascii_command = 'S34'
+        ascii_command = "S34"
         ascii_command += hex(int(round(percent_of_max)))[-2:].upper()
         ascii_command += hex(512 - sum(ascii_command.encode()))[-2:].upper()
-        self.query(ascii_command + 'K')
+        self.query(ascii_command + "K")
 
     @getter
     def get_power(self):
-        return float(self.query('S3B38K')[3:5], 16)
+        return float(self.query("S3B38K")[3:5], 16)
 
     @setter
     def set_output(self, output):
-
         if Toggle(output):
-            self.query('S3200E8K')
+            self.query("S3200E8K")
         else:
-            self.query('S3347K')
+            self.query("S3347K")
 
     @setter
     def set_mode(self, mode):
-        if mode.lower() == 'manual':
-            self.query('S3L01CDK')
-        elif mode.lower() == 'remote':
-            self.query('S3L00CEK')
+        if mode.lower() == "manual":
+            self.query("S3L01CDK")
+        elif mode.lower() == "remote":
+            self.query("S3L00CEK")
         else:
-            raise ValueError(f'{self.name}: Unsupported control mode {mode}. '
-                             'Allowed values are "manual" and "remote".')
+            raise ValueError(
+                f"{self.name}: Unsupported control mode {mode}. "
+                'Allowed values are "manual" and "remote".'
+            )
 
 
 class SRSPS300(Instrument):
     """
     Stanford Rsearch Systems PS-300 series high voltage power supply.
     """
 
-    name = 'SRSPS350'
+    name = "SRSPS350"
 
-    supported_adapters = (
-        (GPIB, {}),
-    )
+    supported_adapters = ((GPIB, {}),)
 
-    knobs = (
-        'output',
-        'voltage',
-        'max voltage'
-        'max current',
-        'trip current'
-    )
+    knobs = ("output", "voltage", "max voltage" "max current", "trip current")
 
-    presets = {
-        'output': 'OFF',
-        'voltage': 0,
-        'max current': 5e-3
-    }
-
-    postsets = {
-        'output': 'OFF',
-        'voltage': 0,
-        'max current': 5e-3
-    }
+    presets = {"output": "OFF", "voltage": 0, "max current": 5e-3}
 
-    meters = (
-        'voltage',
-        'current'
-    )
+    postsets = {"output": "OFF", "voltage": 0, "max current": 5e-3}
+
+    meters = ("voltage", "current")
 
     @setter
     def set_output(self, output):
-
         if Toggle(output):
-            self.write('HVON')
+            self.write("HVON")
         else:
-            self.write('HVOF')
+            self.write("HVOF")
 
     @getter
     def get_output(self):
         # last bit of status byte is the output state
 
         def validator(response):
-            return re.match('\d{1}', response)
+            return re.match("\d{1}", response)
 
-        status_bit_7 = int(self.query('*STB? 7', validator=validator))
+        status_bit_7 = int(self.query("*STB? 7", validator=validator))
 
         if status_bit_7 == 1:
-            return 'ON'
+            return "ON"
         else:
-            return 'OFF'
+            return "OFF"
 
     @setter
     def set_voltage(self, voltage):
-
-        self.write('VSET%f' % float(voltage))
+        self.write("VSET%f" % float(voltage))
 
     @getter
     def get_voltage(self):
-
-        return float(self.query('VSET?'))
+        return float(self.query("VSET?"))
 
     @setter
     def set_max_voltage(self, voltage):
-
-        self.write('VLIM%f' % float(voltage))
+        self.write("VLIM%f" % float(voltage))
 
     @getter
     def get_max_voltage(self):
-
-        return float(self.query('VLIM?'))
+        return float(self.query("VLIM?"))
 
     @setter
     def set_max_current(self, current):
-
-        self.write('ILIM%f' % float(current))
+        self.write("ILIM%f" % float(current))
 
     @getter
     def get_max_current(self):
-
-        return float(self.query('ILIM?'))
+        return float(self.query("ILIM?"))
 
     @setter
     def set_trip_current(self, current):
-
-        self.write('ITRP%f' % float(current))
+        self.write("ITRP%f" % float(current))
 
     @getter
     def get_trip_current(self):
-
-        return float(self.query('ITRP?'))
+        return float(self.query("ITRP?"))
 
     @measurer
     def measure_voltage(self):
-
-        return float(self.query('VOUT?'))
+        return float(self.query("VOUT?"))
 
     @measurer
     def measure_current(self):
-
-        return float(self.query('IOUT?'))
+        return float(self.query("IOUT?"))
```

### Comparing `empyric-0.2.0/empyric/collection/thermometers.py` & `empyric-0.2.3/empyric/collection/thermometers.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,78 +7,77 @@
 class Phidget1101(Instrument):
     """
     Phidgets 4x TC reader
     Many instrument methods (setX, getY, etc.) are mapped by the adapter from
     the Phidgets device class
     """
 
-    name = 'Phidget1101'
+    name = "Phidget1101"
 
-    supported_adapters = (
-        (Phidget, {}),
-    )
+    supported_adapters = ((Phidget, {}),)
 
     # Available knobs
-    knobs = ('type',)
+    knobs = ("type",)
 
     # Available meters
-    meters = ('temperature',)
+    meters = ("temperature",)
 
     def __init__(self, *args, **kwargs):
-
         self.device_class = importlib.import_module(
-            'Phidget22.Devices.TemperatureSensor'
+            "Phidget22.Devices.TemperatureSensor"
         ).TemperatureSensor
 
         Instrument.__init__(self, *args, **kwargs)
 
     @setter
     def set_type(self, type_: String):
-
-        types = importlib.import_module('Phidget22.ThermocoupleType')
+        types = importlib.import_module("Phidget22.ThermocoupleType")
 
         type_dict = {
-            'K': types.ThermocoupleType.THERMOCOUPLE_TYPE_K,
-            'J': types.ThermocoupleType.THERMOCOUPLE_TYPE_J,
-            'T': types.ThermocoupleType.THERMOCOUPLE_TYPE_T,
-            'E': types.ThermocoupleType.THERMOCOUPLE_TYPE_E,
+            "K": types.ThermocoupleType.THERMOCOUPLE_TYPE_K,
+            "J": types.ThermocoupleType.THERMOCOUPLE_TYPE_J,
+            "T": types.ThermocoupleType.THERMOCOUPLE_TYPE_T,
+            "E": types.ThermocoupleType.THERMOCOUPLE_TYPE_E,
         }
 
-        self.write('ThermocoupleType', type_dict[type_])
+        self.write("ThermocoupleType", type_dict[type_])
 
     @measurer
     def measure_temperature(self) -> Float:
-        return self.query('Temperature')
+        return self.query("Temperature")
 
 
 class WilliamsonPyrometer(Instrument):
     """
     Williamson Pro Series 2-color pyrometer.
     """
 
     supported_adapters = (
-        (Serial, {
-            'read_termination': b'\n\r',
-            'write_termination': b'\r\n',
-            'baud_rate': 38400
-        }),
+        (
+            Serial,
+            {
+                "read_termination": b"\n\r",
+                "write_termination": b"\r\n",
+                "baud_rate": 38400,
+            },
+        ),
     )
 
     meters = (
-        'temperature',
-        'unfiltered temperature',
-        'signal strength',
+        "temperature",
+        "unfiltered temperature",
+        "signal strength",
     )
 
     @measurer
     def measure_temperature(self) -> Float:
         # temp returned in F, convert to C
-        return (recast(self.query('FT')) - 32) / 1.8
+        return (recast(self.query("FT")) - 32) / 1.8
 
     @measurer
     def measure_unfiltered_temperature(self) -> Float:
         # temp returned in F, convert to C
-        return (recast(self.query('UT')) - 32) / 1.8
+        return (recast(self.query("UT")) - 32) / 1.8
 
     @measurer
     def measure_signal_strength(self) -> Float:
-        return recast(self.query('SS'))
+        return recast(self.query("SS"))
```

### Comparing `empyric-0.2.0/empyric/collection/virtual.py` & `empyric-0.2.3/empyric/collection/virtual.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,67 +9,61 @@
 class Clock(Instrument):
     """
     Virtual clock for time keeping; works like a standard stopwatch
     """
 
     name = "Clock"
 
-    supported_adapters = (
-        (Adapter, {}),
-    )
+    supported_adapters = ((Adapter, {}),)
 
-    knobs = ('state', )
-    meters = ('time', )
+    knobs = ("state",)
+    meters = ("time",)
 
     @property
     def _time(self):
         if self.stop_time:
             elapsed_time = self.stop_time - self.start_time - self.stoppage
         else:
             elapsed_time = time.time() - self.start_time - self.stoppage
 
         return elapsed_time
 
     def __init__(self, *args, **kwargs):
-
         Instrument.__init__(self, *args, **kwargs)
 
         # Initially stopped
-        self.state = 'STOP'
+        self.state = "STOP"
         self.start_time = self.stop_time = time.time()
 
         self.stoppage = 0  # total time during which the clock has been stopped
 
     @setter
     def set_state(self, state: String):
         """
         Set the clock state:
 
         * 'START': setting to this state starts the clock, if it is stopped.
         * 'STOP': setting to this state stops the clock, if it is running.
         * 'RESET': setting to this state resets the clock time to zero.
         """
 
-        if state == 'START':
-
+        if state == "START":
             if self.stop_time:
                 self.stoppage += time.time() - self.stop_time
                 self.stop_time = False
 
-            self.state = 'START'
-
-        elif state == 'STOP':
+            self.state = "START"
 
+        elif state == "STOP":
             if not self.stop_time:
                 self.stop_time = time.time()
 
-            self.state = 'START'
-
-        elif state == 'RESET':
+            self.state = "START"
 
+        elif state == "RESET":
             self.start_time = time.time()
             self.stoppage = 0
 
             if self.stop_time:
                 self.stop_time = self.start_time
 
             return self.state  # return to START or STOP state once reset
@@ -84,24 +78,22 @@
     """
     Virtual instrument with a single knob "input" and single meter "output",
     useful for testing.
 
     The "output" meter simply returns the value of the "input" knob.
     """
 
-    name = 'Echo'
+    name = "Echo"
 
-    supported_adapters = (
-        (Adapter, {}),
-    )
+    supported_adapters = ((Adapter, {}),)
 
-    knobs = ('input',)
-    presets = {'input': 0}
+    knobs = ("input",)
+    presets = {"input": 0}
 
-    meters = ('output',)
+    meters = ("output",)
 
     @setter
     def set_input(self, _input: Float):
         pass
 
     @measurer
     def measure_output(self) -> Float:
@@ -115,24 +107,22 @@
     x_{n+1} = 1 - a * x_n^2 + y_n
 
     y_{n+1} = b * x_n
 
     It has two virtual knobs (a,b) and two virtual meters (x,y)
     """
 
-    name = 'HenonMapper'
+    name = "HenonMapper"
 
-    supported_adapters = (
-        (Adapter, {}),
-    )
+    supported_adapters = ((Adapter, {}),)
 
-    knobs = ('a', 'b')
-    presets = {'a': 1.4, 'b': 0.3}
+    knobs = ("a", "b")
+    presets = {"a": 1.4, "b": 0.3}
 
-    meters = ('x', 'y')
+    meters = ("x", "y")
 
     a = 1.4
     b = 0.3
 
     x, y = 0.63, 0.19  # near the unstable fixed point
 
     @setter
@@ -162,15 +152,15 @@
         Each call triggers a new iteration, with new values set for x and y
         based on the Henon Map. Therefore, each call to ``measure_x`` should
         be followed by a call to ``measure_y``.
 
         :return: (float) current value of x
         """
 
-        x_new = 1.0 - self.a * self.x ** 2 + self.y
+        x_new = 1.0 - self.a * self.x**2 + self.y
         y_new = self.b * self.x
 
         self.x = x_new
         self.y = y_new
 
         return self.x
 
@@ -191,38 +181,25 @@
 
 class PIDController(Instrument):
     """
     Virtual PID controller
 
     """
 
-    name = 'PIDController'
+    name = "PIDController"
 
-    supported_adapters = (
-        (Adapter, {}),
-    )
-
-    knobs = (
-        'setpoint',
-        'proportional gain'
-        'derivative time'
-        'integral time',
-        'input'
-    )
-
-    presets = {
-        'proportional gain': 1,
-        'derivative time': 12,
-        'integral time': 180
-    }
+    supported_adapters = ((Adapter, {}),)
 
-    meters = ('output',)
+    knobs = ("setpoint", "proportional gain" "derivative time" "integral time", "input")
 
-    def __init__(self, *args, **kwargs):
+    presets = {"proportional gain": 1, "derivative time": 12, "integral time": 180}
+
+    meters = ("output",)
 
+    def __init__(self, *args, **kwargs):
         self.setpoint = None
 
         Instrument.__init_(self, *args, **kwargs)
         self.clock = Clock()
 
         self.times = np.array([])
         self.setpoints = np.array([])
@@ -265,45 +242,39 @@
     def measure_output(self) -> Float:
         """Get the controller output"""
         if self.setpoint is None:
             # Don't output anything unless the setpoint is defined
             return None
 
         if len(self.outputs) < len(self.inputs):  # if input has been updated
-
             # Proportional term
             error = self.setpoint - self.input
 
             # Integral and derivative terms
             if len(self.times) > 1:
-
                 interval = np.argwhere(
                     self.times >= self.times[-1] - self.integral_time
                 ).flatten()
 
                 dt = np.diff(self.times[interval])
                 errors = (self.setpoints - self.inputs)[interval[1:]]
 
-                integral = np.sum(dt*errors)
+                integral = np.sum(dt * errors)
 
-                derivative = -(
-                        self.inputs[-1] - self.inputs[-2]
-                ) / (
-                        self.times[-1] - self.times[-2]
+                derivative = -(self.inputs[-1] - self.inputs[-2]) / (
+                    self.times[-1] - self.times[-2]
                 )
             else:
                 integral = 0
                 derivative = 0
 
             tD = self.derivative_time
             tI = self.integral_time
 
-            output = self.proportional_gain*(
-                    error + tD*derivative + integral/tI
-            )
+            output = self.proportional_gain * (error + tD * derivative + integral / tI)
 
             self.outputs.append(output)
 
             return output
         else:
             return self.outputs[-1]
 
@@ -315,32 +286,27 @@
     Dynamics of the process value is determined by the mean, step and affinity
     knobs. The mean is the mean value of the process in steady state, the step
     is the size of the step that the process can take in either direction upon
     each measurement of the process value, and the affinity is the tendancy of
     the process value to return to its mean value at each step.
     """
 
-    name = 'RandomWalk'
+    name = "RandomWalk"
 
-    supported_adapters = (
-        (Adapter, {}),
-    )
+    supported_adapters = ((Adapter, {}),)
 
-    knobs = ('mean',
-             'step',
-             'affinity')
+    knobs = ("mean", "step", "affinity")
 
-    meters = ('value',)
+    meters = ("value",)
 
     def __init__(self, *args, **kwargs):
+        Instrument.__init__(self, *args, **kwargs)
 
-        Instrument.__init__(self,*args, **kwargs)
-
-        self.mean = 0.
-        self.step = 1.
+        self.mean = 0.0
+        self.step = 1.0
         self.affinity = 0.01
         self.value = self.mean
 
     @setter
     def set_mean(self, mean: Float):
         pass
 
@@ -350,85 +316,72 @@
 
     @setter
     def set_drift(self, drift: Float):
         pass
 
     @measurer
     def measure_value(self) -> Float:
-
-        self.value += np.random.choice(
-            [-self.step, self.step]
-        ) + self.affinity*(self.mean - self.value)
+        self.value += np.random.choice([-self.step, self.step]) + self.affinity * (
+            self.mean - self.value
+        )
 
         return self.value
 
 
 class SimpleProcess(Instrument):
     """
     Virtual process that mimics the behavior of a heating process
     """
 
-    name = 'SimpleProcess'
+    name = "SimpleProcess"
 
-    supported_adapters = (
-        (Adapter, {}),
-    )
-
-    knobs = ('setpoint',
-             'noise level',
-             'response time')
-
-    presets = {
-        'setpoint': 0.0,
-        'noise level': 0.1,
-        'response time': 10.0
-    }
+    supported_adapters = ((Adapter, {}),)
 
-    meters = ('value',)
+    knobs = ("setpoint", "noise level", "response time")
 
-    def __init__(self, *args, **kwargs):
+    presets = {"setpoint": 0.0, "noise level": 0.1, "response time": 10.0}
+
+    meters = ("value",)
 
+    def __init__(self, *args, **kwargs):
         Instrument.__init__(self, *args, **kwargs)
 
         self._clock = Clock()
-        self._clock.set_state('START')
+        self._clock.set_state("START")
         self._time = self._clock.measure_time()
 
     @setter
     def set_setpoint(self, setpoint: Float):
-        if hasattr(self, '_time'):
+        if hasattr(self, "_time"):
             self.measure_value()
-            self._clock.set_state('RESET')
+            self._clock.set_state("RESET")
         else:
             self._value = setpoint
 
     @setter
     def set_noise_level(self, noise_level: Float):
         pass
 
     @setter
     def set_response_time(self, response_time: Float):
         pass
 
     @measurer
     def measure_value(self) -> Float:
-
         last_value = self._value
         t = self._clock.measure_time()  # time since last setpoint change
-        self._value = self.setpoint + (
-                last_value - self.setpoint
-        )*np.exp(-t / self.response_time)
+        self._value = self.setpoint + (last_value - self.setpoint) * np.exp(
+            -t / self.response_time
+        )
 
-        return self._value + self.noise_level*(2*np.random.rand() - 1)
+        return self._value + self.noise_level * (2 * np.random.rand() - 1)
 
 
 class ModbusClient(Instrument):
     """
     Counterpart to the ModbusServer routine. Communicates with a ModbusServer
     instance in other experiments to control variables.
     """
 
-    name = 'DataClient'
+    name = "DataClient"
 
-    supported_adapters = (
-        (Modbus, {}),
-    )
+    supported_adapters = ((Modbus, {}),)
```

### Comparing `empyric-0.2.0/empyric/experiment.py` & `empyric-0.2.3/empyric/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,153 +29,147 @@
     """
     An iterable class which represents an experiment; iterates through any
     assigned routines,and retrieves and stores the values of all experiment
     variables.
     """
 
     # Possible statuses of an experiment
-    READY = 'Ready'  # Experiment is waiting to start
-    RUNNING = 'Running'  # Experiment is running
-    HOLDING = 'Holding'  # Routines are stopped, but measurements are ongoing
-    STOPPED = 'Stopped'  # Both routines and measurements are stopped
-    TERMINATED = 'Terminated'
+    READY = "Ready"  # Experiment is waiting to start
+    RUNNING = "Running"  # Experiment is running
+    HOLDING = "Holding"  # Routines are stopped, but measurements are ongoing
+    STOPPED = "Stopped"  # Both routines and measurements are stopped
+    TERMINATED = "Terminated"
 
     # Experiment has either finished or has been terminated by the user
 
     @property
     def status(self):
         return self._status
 
     @status.setter
     def status(self, status):
-        prior_base_status = self._status.split(':')[0]
-        new_base_status = status.split(':')[0]
+        prior_base_status = self._status.split(":")[0]
+        new_base_status = status.split(":")[0]
 
         # Only allow change if the status is unlocked,
         # or if the base status is the same
         if not self.status_locked or new_base_status == prior_base_status:
             self._status = status
 
     @property
     def ready(self):
-        return 'Ready' in self.status
+        return "Ready" in self.status
 
     @property
     def running(self):
-        return 'Running' in self.status
+        return "Running" in self.status
 
     @property
     def holding(self):
-        return 'Holding' in self.status
+        return "Holding" in self.status
 
     @property
     def stopped(self):
-        return 'Stopped' in self.status
+        return "Stopped" in self.status
 
     @property
     def terminated(self):
-        return 'Terminated' in self.status
+        return "Terminated" in self.status
 
     def __init__(self, variables, routines=None, end=None):
-
         self.variables = variables
         # dict of the form {..., name: variable, ...}
 
         # Used to block evaluation of expressions
         # until their dependee variables are evaluated
         self.eval_events = {name: threading.Event() for name in variables}
 
         if routines:
             self.routines = routines
             # dictionary of the form {..., name: (variable_name, routine), ...}
         else:
             self.routines = {}
 
         if end:
-            if end.lower() == 'with routines':
+            if end.lower() == "with routines":
                 self.end = max([routine.end for routine in routines.values()])
             else:
                 self.end = end
         else:
             self.end = np.inf
 
         self.clock = Clock()
         self.clock.start()
 
-        self.timestamp = datetime.datetime.now().strftime('%Y%m%d-%H%M%S')
+        self.timestamp = datetime.datetime.now().strftime("%Y%m%d-%H%M%S")
 
-        self.data = pd.DataFrame(columns=['Time'] + list(variables.keys()))
+        self.data = pd.DataFrame(columns=["Time"] + list(variables.keys()))
 
         self.state = pd.Series({column: None for column in self.data.columns})
-        self.state['Time'] = 0
+        self.state["Time"] = 0
 
         self._status = Experiment.READY
         self.status_locked = True
         # can only be unlocked by the start, hold, stop and terminate methods
 
         self.saved = []  # list of saved data entries
 
     def __next__(self):
-
         # Start the clock on first call
         if self.state.name is None:  # first step of the experiment
             self.start()
-            self.status = Experiment.RUNNING + ': initializing...'
+            self.status = Experiment.RUNNING + ": initializing..."
 
         # Update time
-        self.state['Time'] = self.clock.time
+        self.state["Time"] = self.clock.time
         self.state.name = datetime.datetime.now()
 
         # If experiment is stopped, just return the knob & parameter values,
         # and nullify meter & expression values
         if self.stopped:
-
             threads = {}
             for name, variable in self.variables.items():
-
                 is_knob = isinstance(variable, _variables.Knob)
                 is_parameter = isinstance(variable, _variables.Parameter)
 
                 if is_knob or is_parameter:
                     threads[name] = threading.Thread(
                         target=self._update_variable, args=(name,)
                     )
                     threads[name].start()
                 else:
                     self.state[name] = None
 
             # Wait for all variable update threads to finish
             for name, thread in threads.items():
-                self.status = Experiment.RUNNING + f': retrieving {name}'
+                self.status = Experiment.RUNNING + f": retrieving {name}"
                 thread.join()
 
             return self.state
 
         # If the experiment is running, apply new settings to knobs
         # according to the routines (if there are any)
         if self.running:
-
             # Update each routine in its own thread
             threads = {}
             for name, routine in self.routines.items():
                 threads[name] = threading.Thread(
                     target=self._update_routine, args=(name,)
                 )
                 threads[name].start()
 
             # Wait for all routine threads to finish
             for name, thread in threads.items():
-                self.status = Experiment.RUNNING + f': executing {name}'
+                self.status = Experiment.RUNNING + f": executing {name}"
                 thread.join()
 
             self.status = Experiment.RUNNING
 
         # Get all variable values if experiment is running or holding
         if self.running or self.holding:
-
             for event in self.eval_events.values():
                 event.clear()
 
             # Run each measure / get operation in its own thread
             threads = {}
             for name in self.variables:
                 threads[name] = threading.Thread(
@@ -183,15 +177,15 @@
                 )
                 threads[name].start()
 
             base_status = self.status
 
             # Wait for all threads to finish
             for name, thread in threads.items():
-                self.status = base_status + f': retrieving {name}'
+                self.status = base_status + f": retrieving {name}"
                 thread.join()
 
             self.status = base_status
 
             # Append new state to experiment data set
             self.data.loc[self.state.name] = self.state
 
@@ -207,31 +201,30 @@
     def __iter__(self):
         return self
 
     def _update_variable(self, name):
         """Retrieve and store a variable value"""
 
         try:
-
             if isinstance(self.variables[name], _variables.Expression):
                 for dependee in self.variables[name].definitions:
                     event = self.eval_events[dependee]
                     event.wait()  # wait for dependee to be evaluated
 
             value = self.variables[name].value
 
             self.eval_events[name].set()
             # unblock threads evaluating dependents
 
             if np.size(value) > 1:  # store array data as CSV files
                 dataframe = pd.DataFrame(
                     {name: value}, index=[self.state.name] * len(value)
                 )
-                path = name.replace(' ', '_') + '_'
-                path += self.state.name.strftime('%Y%m%d-%H%M%S') + '.csv'
+                path = name.replace(" ", "_") + "_"
+                path += self.state.name.strftime("%Y%m%d-%H%M%S") + ".csv"
                 dataframe.to_csv(path)
                 self.state[name] = path
             else:
                 self.state[name] = value
         except BaseException as err:
             self.terminate()
             raise err
@@ -251,32 +244,32 @@
 
         :param directory: (path) (optional) directory to save data to,
                           if different from working directory
         :return: None
         """
 
         base_status = self.status
-        self.status = base_status + ': saving data'
+        self.status = base_status + ": saving data"
 
         path = f"data_{self.timestamp}.csv"
 
         if directory:
             path = os.path.join(directory, path)
 
         if not os.path.exists(path):
             # if this is a new file, write column headers
-            with open(path, 'a') as data_file:
-                data_file.write(',' + ','.join(self.data.columns) + '\n')
+            with open(path, "a") as data_file:
+                data_file.write("," + ",".join(self.data.columns) + "\n")
 
         unsaved = np.setdiff1d(self.data.index, self.saved)
 
-        with open(path, 'a') as data_file:
+        with open(path, "a") as data_file:
             for line in unsaved:
-                line_data = ','.join(map(str, list(self.data.loc[line])))
-                data_file.write(str(line) + ',' + line_data + '\n')
+                line_data = ",".join(map(str, list(self.data.loc[line])))
+                data_file.write(str(line) + "," + line_data + "\n")
 
         self.saved = self.saved + list(unsaved)
 
         self.status = base_status
 
     def start(self):
         """
@@ -298,29 +291,29 @@
         :return: None
         """
         self.clock.stop()
 
         self.status_locked = False
         self.status = Experiment.HOLDING
         if reason:
-            self.status = self.status + ': ' + reason
+            self.status = self.status + ": " + reason
         self.status_locked = True
 
     def stop(self, reason=None):
         """
         Stop the experiment: clock stops, routines stop, measurements stop
 
         :return: None
         """
         self.clock.stop()
 
         self.status_locked = False
         self.status = Experiment.STOPPED
         if reason:
-            self.status = self.status + ': ' + reason
+            self.status = self.status + ": " + reason
         self.status_locked = True
 
     def terminate(self, reason=None):
         """
         Terminate the experiment: clock, routines and measurements stop,
         data is saved and StopIteration is raised
 
@@ -328,23 +321,23 @@
         """
         self.stop()
         self.save()
 
         self.status_locked = False
         self.status = Experiment.TERMINATED
         if reason:
-            self.status = self.status + ': ' + reason
+            self.status = self.status + ": " + reason
         self.status_locked = True
 
         # End routines
         for routine in self.routines.values():
             routine.terminate()
 
     def __repr__(self):
-        return 'Experiment'
+        return "Experiment"
 
 
 class Alarm:
     """
     Triggers if a condition among variables is met and indicates the response
     protocol
     """
@@ -353,22 +346,22 @@
         self.trigger_variable = _variables.Expression(
             expression=condition, definitions=variables
         )
 
         if protocol:
             self.protocol = protocol
         else:
-            self.protocol = 'none'
+            self.protocol = "none"
 
     @property
     def triggered(self):
         return self.trigger_variable.value is True
 
     def __repr__(self):
-        return 'Alarm'
+        return "Alarm"
 
 
 class Manager:
     """
     Utility class which sets up and manages experiments, based on runcards.
     When initallized, it uses the given runcard to construct an experiment and
     run it in a separate thread. The Manager also handles alarms as specified
@@ -384,65 +377,58 @@
         if runcard:
             self.runcard = runcard
         else:
             # Have user locate runcard, if none given
             root = tk.Tk()
             root.withdraw()
             self.runcard = askopenfilename(
-                parent=root, title='Select Runcard',
-                filetypes=[('YAML files', '*.yaml')]
+                parent=root,
+                title="Select Runcard",
+                filetypes=[("YAML files", "*.yaml")],
             )
 
-            if self.runcard == '':
-                raise ValueError('a valid runcard was not selected!')
+            if self.runcard == "":
+                raise ValueError("a valid runcard was not selected!")
 
         if isinstance(self.runcard, str):
             if os.path.exists(self.runcard):
                 dirname = os.path.dirname(self.runcard)
-                if dirname != '':
+                if dirname != "":
                     os.chdir(os.path.dirname(self.runcard))
                     # go to runcard directory to put data in same location
 
                 yaml = YAML()
-                with open(self.runcard, 'rb') as runcard_file:
+                with open(self.runcard, "rb") as runcard_file:
                     self.runcard = yaml.load(runcard_file)  # load the runcard
             else:
-                raise FileNotFoundError(
-                    f'invalid runcard path "{self.runcard}"'
-                )
+                raise FileNotFoundError(f'invalid runcard path "{self.runcard}"')
         elif isinstance(self.runcard, dict):
             pass
         else:
             raise TypeError(
-                f'runcard given to Manager must be a path to a YAML file '
-                f'or a dictionary, not {type(self.runcard)}!'
+                f"runcard given to Manager must be a path to a YAML file "
+                f"or a dictionary, not {type(self.runcard)}!"
             )
 
         converted_runcard = convert_runcard(self.runcard)
 
-        self.description = converted_runcard['Description']
-        self.settings = converted_runcard['Settings']
-        self.instruments = converted_runcard['Instruments']
-        self.alarms = converted_runcard['Alarms']
-        self.plotter = converted_runcard.get('Plotter', None)
+        self.description = converted_runcard["Description"]
+        self.settings = converted_runcard["Settings"]
+        self.instruments = converted_runcard["Instruments"]
+        self.alarms = converted_runcard["Alarms"]
+        self.plotter = converted_runcard.get("Plotter", None)
 
-        self.experiment = converted_runcard['Experiment']
+        self.experiment = converted_runcard["Experiment"]
 
         # Unpack settings
-        self.followup = self.settings.get('follow-up', None)
-        self.step_interval = convert_time(
-            self.settings.get('step interval', 0.1)
-        )
-        self.save_interval = convert_time(
-            self.settings.get('save interval', 60)
-        )
-        self.plot_interval = convert_time(
-            self.settings.get('plot interval', 0.1)
-        )
-        self.end = convert_time(self.settings.get('end', np.inf))
+        self.followup = self.settings.get("follow-up", None)
+        self.step_interval = convert_time(self.settings.get("step interval", 0.1))
+        self.save_interval = convert_time(self.settings.get("save interval", 60))
+        self.plot_interval = convert_time(self.settings.get("plot interval", 0.1))
+        self.end = convert_time(self.settings.get("end", np.inf))
 
         self.experiment.end = self.end
 
         self.last_save = 0
 
         self.awaiting_alarms = {}  # dictionary of alarms that are triggered
 
@@ -458,185 +444,182 @@
 
         top_dir = os.getcwd()
 
         if directory:
             os.chdir(directory)
 
         # Create a new directory for data storage
-        experiment_name = self.runcard['Description'].get('name', 'Experiment')
-        working_dir = experiment_name + '-' + self.experiment.timestamp
+        experiment_name = self.runcard["Description"].get("name", "Experiment")
+        working_dir = experiment_name + "-" + self.experiment.timestamp
         os.mkdir(working_dir)
         os.chdir(working_dir)
 
         # Save executed runcard alongside data for record keeping
         yaml = YAML()
 
         timestamped_path = f"{experiment_name}_{self.experiment.timestamp}.yaml"
-        with open(timestamped_path, 'w') as runcard_file:
+        with open(timestamped_path, "w") as runcard_file:
             yaml.dump(self.runcard, runcard_file)
 
         # Run experiment loop in separate thread
         experiment_thread = threading.Thread(target=self._run)
         experiment_thread.start()
 
         # Set up the GUI for user interaction
-        self.gui = _graphics.ExperimentGUI(self.experiment,
-                                           alarms=self.alarms,
-                                           instruments=self.instruments,
-                                           title=self.description.get(
-                                               'name', 'Experiment'
-                                           ),
-                                           plotter=self.plotter,
-                                           save_interval=self.save_interval,
-                                           plot_interval=self.plot_interval)
+        self.gui = _graphics.ExperimentGUI(
+            self.experiment,
+            alarms=self.alarms,
+            instruments=self.instruments,
+            title=self.description.get("name", "Experiment"),
+            plotter=self.plotter,
+            save_interval=self.save_interval,
+            plot_interval=self.plot_interval,
+        )
 
         self.gui.run()
 
         experiment_thread.join()
 
         # Disconnect instruments
         for instrument in self.instruments.values():
             instrument.disconnect()
 
         os.chdir(top_dir)  # return to the parent directory
 
         # Cancel follow-up if experiment terminated by user
-        if self.experiment.terminated and 'user' in self.experiment.status:
+        if self.experiment.terminated and "user" in self.experiment.status:
             self.followup = None
 
         # Execute the follow-up experiment if there is one
         if self.followup:
-            if 'yaml' in self.followup:
+            if "yaml" in self.followup:
                 self.__init__(self.followup)
                 self.run(directory=directory)
-            elif 'repeat' in self.followup:
+            elif "repeat" in self.followup:
                 self.__init__(self.runcard)
                 self.run(directory=directory)
 
     def _run(self):
         # Run in a separate thread
 
         for state in self.experiment:
-
             step_start = time.time()
 
             # Save experimental data periodically
             next_save = self.last_save + self.save_interval
             if self.experiment.clock.time >= next_save:
                 save_thread = threading.Thread(target=self.experiment.save)
                 save_thread.start()
                 self.last_save = self.experiment.clock.time
 
             # Check if any alarms are triggered and handle them
             for name, alarm in self.alarms.items():
                 if alarm.triggered:
-
                     # Add to dictionary of triggered alarms, if newly triggered
                     if name not in self.awaiting_alarms:
                         self.awaiting_alarms[name] = {
-                            'time': self.experiment.data['Time'].iloc[-1],
-                            'status': self.experiment.status,
+                            "time": self.experiment.data["Time"].iloc[-1],
+                            "status": self.experiment.status,
                         }
 
-                    if 'none' in alarm.protocol:
+                    if "none" in alarm.protocol:
                         # do nothing (GUI will indicate that alarm is triggered)
                         break
-                    if 'hold' in alarm.protocol:
+                    if "hold" in alarm.protocol:
                         # stop routines but keep measuring until alarm is clear
                         self.experiment.hold(reason=name)
                         break
-                    elif 'stop' in alarm.protocol:
+                    elif "stop" in alarm.protocol:
                         # stop routines and measurements until alarm is clear
                         self.experiment.stop(reason=name)
                         break
-                    elif 'terminate' in alarm.protocol:
+                    elif "terminate" in alarm.protocol:
                         # terminate the experiment
                         self.experiment.terminate(reason=name)
                         break
-                    elif 'yaml' in alarm.protocol:
+                    elif "yaml" in alarm.protocol:
                         # terminate the experiment and run another
                         self.experiment.terminate(reason=name)
                         self.followup = alarm.protocol
                         break
-                    elif 'check' in alarm.protocol:
+                    elif "check" in alarm.protocol:
                         # stop routines and measurements until user resumes
                         self.experiment.stop(reason=name)
                         break
                     else:
                         # terminate the experiment
                         self.experiment.terminate(reason=name)
                         break
 
                 elif name in self.awaiting_alarms:
                     # Alarm was previously triggered but is now clear
 
-                    if 'check' not in alarm.protocol:
+                    if "check" not in alarm.protocol:
                         # alarm is not waiting for user to check
 
                         info = self.awaiting_alarms.pop(name)
                         # remove from dictionary of triggered alarms
-                        prior_status = info['status']
+                        prior_status = info["status"]
 
                         if len(self.awaiting_alarms) == 0:
                             # there are no more triggered alarms
                             # return to state of experiment prior to trigger
-                            if 'Running' in prior_status:
+                            if "Running" in prior_status:
                                 self.experiment.start()
-                            if 'Holding' in prior_status:
-                                self.experiment.hold(reason=name + ' cleared')
-                            if 'Stopped' in prior_status:
-                                self.experiment.stop(reason=name + ' cleared')
+                            if "Holding" in prior_status:
+                                self.experiment.hold(reason=name + " cleared")
+                            if "Stopped" in prior_status:
+                                self.experiment.stop(reason=name + " cleared")
 
             step_end = time.time()
 
             remaining_time = self.step_interval - (step_end - step_start)
 
             if remaining_time > 0:
                 time.sleep(remaining_time)
 
     def __repr__(self):
-        return 'Manager'
+        return "Manager"
 
 
 class RuncardError(BaseException):
     pass
 
 
 def validate_runcard(runcard):
     is_dict = isinstance(runcard, dict)
     is_ordereddict = isinstance(runcard, collections.OrderedDict)
 
     if is_dict or is_ordereddict:
-
         # Create temporary runcard YAML file for PyKwalify to validate
         yaml = YAML()
 
-        runcard_path = f'tmp_runcard_{time.time()}.yaml'
+        runcard_path = f"tmp_runcard_{time.time()}.yaml"
 
-        with open(runcard_path, 'w') as runcard_file:
+        with open(runcard_path, "w") as runcard_file:
             yaml.dump(runcard, runcard_file)
 
         validate_runcard(runcard_path)
 
         # Wait until temporary file has write access, then delete
         while not os.access(runcard_path, os.W_OK):
             time.sleep(0.1)
 
         os.remove(runcard_path)
 
         return True
 
     elif type(runcard) is not str:
-        raise ValueError('runcard must be either dict or str.')
+        raise ValueError("runcard must be either dict or str.")
 
     validator = YamlValidator(
         source_file=runcard,
         schema_files=[
             os.path.join(pathlib.Path(__file__).parent, "runcard_schema.yaml")
-        ]
+        ],
     )
 
     try:
         validator.validate(raise_exception=True)
     except pykwalify.errors.SchemaError as err:
         raise RuncardError(err)
 
@@ -660,180 +643,177 @@
       ``Alarm`` objects.
     * The Plots section is converted into a corresponding ``Plotter`` instance.
     """
 
     # if runcard argument is a path to a YAML file, load into a dictionary
     if type(runcard) == str:
         yaml = YAML()
-        with open(runcard, 'rb') as runcard_file:
+        with open(runcard, "rb") as runcard_file:
             runcard = yaml.load(runcard_file)
 
     # Validate runcard format and contents
     validate_runcard(runcard)
 
     converted_runcard = runcard.copy()
 
     # Load any custom components
     custom_routines = {}
     custom_instruments = {}
 
-    if 'custom.py' in os.listdir():
+    if "custom.py" in os.listdir():
         sys.path.insert(1, os.getcwd())
-        custom = importlib.import_module('custom')
+        custom = importlib.import_module("custom")
 
         for name, thing in custom.__dict__.items():
             if type(thing) == type:
                 if issubclass(thing, _routines.Routine):
                     custom_routines[name] = thing
                 if issubclass(thing, _instruments.Instrument):
                     custom_instruments[name] = thing
 
     # Instruments section
     available_instruments = {**_instruments.supported, **custom_instruments}
 
     instruments = {}
-    for name, specs in runcard.get('Instruments', {}).items():
-
+    for name, specs in runcard.get("Instruments", {}).items():
         specs = specs.copy()
-        _type = specs.pop('type')
-        address = specs.get('address', None)
+        _type = specs.pop("type")
+        address = specs.get("address", None)
 
         # Grab any keyword arguments for the adapter
         adapter_kwargs = {}
         for kwarg in _adapters.kwargs:
-            if kwarg.replace('_', ' ') in specs:
-                adapter_kwargs[kwarg] = specs.pop(kwarg.replace('_', ' '))
+            if kwarg.replace("_", " ") in specs:
+                adapter_kwargs[kwarg] = specs.pop(kwarg.replace("_", " "))
 
         # Any remaining keywords are instrument presets
         presets = {
-            key: recast(value) for key, value
-            in specs.get('presets', {}).items()
+            key: recast(value) for key, value in specs.get("presets", {}).items()
         }
         postsets = {
-            key: recast(value) for key, value
-            in specs.get('postsets', {}).items()
+            key: recast(value) for key, value in specs.get("postsets", {}).items()
         }
 
         instrument_class = available_instruments[_type]
         instruments[name] = instrument_class(
-            address=address, presets=presets, postsets=postsets,
-            **adapter_kwargs
+            address=address, presets=presets, postsets=postsets, **adapter_kwargs
         )
         instruments[name].name = name
 
-    converted_runcard['Instruments'] = instruments
+    converted_runcard["Instruments"] = instruments
 
     # Variables section
     variables = {}
-    for name, specs in runcard['Variables'].items():
-        if 'meter' in specs:
-            instrument = converted_runcard['Instruments'][specs['instrument']]
-            gate = specs.get('gate', None)
+    for name, specs in runcard["Variables"].items():
+        if "meter" in specs:
+            instrument = converted_runcard["Instruments"][specs["instrument"]]
+            gate = specs.get("gate", None)
             gate = variables[gate] if gate else None
             variables[name] = _variables.Meter(
-                meter=specs['meter'], instrument=instrument, gate=gate
+                meter=specs["meter"], instrument=instrument, gate=gate
             )
-        elif 'knob' in specs:
-            instrument = converted_runcard['Instruments'][specs['instrument']]
+        elif "knob" in specs:
+            instrument = converted_runcard["Instruments"][specs["instrument"]]
             variables[name] = _variables.Knob(
-                knob=specs['knob'], instrument=instrument,
-                lower_limit=specs.get('lower limit', None),
-                upper_limit=specs.get('upper limit', None)
+                knob=specs["knob"],
+                instrument=instrument,
+                lower_limit=specs.get("lower limit", None),
+                upper_limit=specs.get("upper limit", None),
             )
-        elif 'expression' in specs:
-            expression = specs['expression']
+        elif "expression" in specs:
+            expression = specs["expression"]
             definitions = {}
 
-            for symbol, var_name in specs['definitions'].items():
+            for symbol, var_name in specs["definitions"].items():
                 expression = expression.replace(symbol, var_name)
 
                 try:
                     definitions[var_name] = variables[var_name]
                 except KeyError as undefined:
                     raise KeyError(
                         f"variable {undefined} is not defined for expression "
                         f"'{name}'"
                     )
 
             variables[name] = _variables.Expression(
                 expression=expression, definitions=definitions
             )
-        elif 'server' in specs:
-            server = specs['server']
-            alias = specs.get('alias', name)
-            protocol = specs.get('protocol', None)
-            settable = specs.get('settable', False)
+        elif "server" in specs:
+            server = specs["server"]
+            alias = specs.get("alias", name)
+            protocol = specs.get("protocol", None)
+            settable = specs.get("settable", False)
 
             variables[name] = _variables.Remote(
                 server=server, alias=alias, protocol=protocol, settable=settable
             )
 
-        elif 'parameter' in specs:
-            variables[name] = _variables.Parameter(parameter=specs['parameter'])
+        elif "parameter" in specs:
+            variables[name] = _variables.Parameter(parameter=specs["parameter"])
 
     # Routines section
     available_routines = {**_routines.supported, **custom_routines}
 
     routines = {}
-    if 'Routines' in runcard:
-        for name, specs in runcard['Routines'].items():
+    if "Routines" in runcard:
+        for name, specs in runcard["Routines"].items():
             specs = specs.copy()  # avoids modifying the runcard
-            _type = specs.pop('type')
+            _type = specs.pop("type")
 
-            specs = {
-                key.replace(' ', '_'): value for key, value in specs.items()
-            }
+            specs = {key.replace(" ", "_"): value for key, value in specs.items()}
 
             # Convert list of knobs into dictionary
-            knobs = np.array([specs.get('knobs', [])]).flatten()
+            knobs = np.array([specs.get("knobs", [])]).flatten()
             if knobs.size > 0:
                 for knob in knobs:
                     if knob not in variables:
                         raise KeyError(
-                            f'knob {knob} specified for routine {name} '
-                            'is not in Variables!'
+                            f"knob {knob} specified for routine {name} "
+                            "is not in Variables!"
                         )
 
-                specs['knobs'] = {name: variables[name] for name in knobs}
+                specs["knobs"] = {name: variables[name] for name in knobs}
 
             routines[name] = available_routines[_type](**specs)
 
-    converted_runcard['Experiment'] = Experiment(variables, routines=routines)
+    converted_runcard["Experiment"] = Experiment(variables, routines=routines)
 
     # Alarms section
     alarms = {}
-    if 'Alarms' in runcard:
-        for name, specs in runcard['Alarms'].items():
+    if "Alarms" in runcard:
+        for name, specs in runcard["Alarms"].items():
+            alarm_variables = specs.copy().get("variables", {})
+            condition = specs.copy()["condition"]
 
-            alarm_variables = specs.copy().get('variables', {})
-            condition = specs.copy()['condition']
-
-            for variable in specs.get('variables', {}):
+            for variable in specs.get("variables", {}):
                 if variable not in variables:
                     raise KeyError(
-                        f'variable {variable} specified for alarm {name} '
-                        f'is not in Variables!'
+                        f"variable {variable} specified for alarm {name} "
+                        f"is not in Variables!"
                     )
 
-            alphabet = 'abcdefghijklmnopqrstuvwxyz'
+            alphabet = "abcdefghijklmnopqrstuvwxyz"
             for var_name, variable in variables.items():
-
                 # Variables can be called by name in the condition
                 if var_name in condition:
-                    temp_name = ''.join(
+                    temp_name = "".join(
                         [
-                            alphabet[np.random.randint(0, len(alphabet))]
+                            alphabet[
+                                np.random.randint(0, len(alphabet))
+                            ]  # pylint: disable=invalid-sequence-index
                             for i in range(3)
                         ]
                     )
                     while temp_name in alarm_variables:
                         # make sure temp_name is not repeated
-                        temp_name = ''.join(
+                        temp_name = "".join(
                             [
-                                alphabet[np.random.randint(0, len(alphabet))]
+                                alphabet[
+                                    np.random.randint(0, len(alphabet))
+                                ]  # pylint: disable=invalid-sequence-index
                                 for i in range(3)
                             ]
                         )
 
                     alarm_variables.update({temp_name: variable})
                     condition = condition.replace(var_name, temp_name)
 
@@ -841,25 +821,23 @@
                 for symbol, alarm_variable_name in alarm_variables.items():
                     if alarm_variable_name == var_name:
                         alarm_variables[symbol] = variable
 
             alarms.update(
                 {
                     name: Alarm(
-                        condition,
-                        alarm_variables,
-                        protocol=specs.get('protocol', None)
+                        condition, alarm_variables, protocol=specs.get("protocol", None)
                     )
                 }
             )
 
-    converted_runcard['Alarms'] = alarms
+    converted_runcard["Alarms"] = alarms
 
     # Plots section
-    if 'Plots' in runcard:
-        converted_runcard['Plotter'] = _graphics.Plotter(
-            converted_runcard['Experiment'].data, settings=runcard['Plots']
+    if "Plots" in runcard:
+        converted_runcard["Plotter"] = _graphics.Plotter(
+            converted_runcard["Experiment"].data, settings=runcard["Plots"]
         )
     else:
-        converted_runcard['Plotter'] = None
+        converted_runcard["Plotter"] = None
 
     return converted_runcard
```

### Comparing `empyric-0.2.0/empyric/graphics.py` & `empyric-0.2.3/empyric/graphics.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import tkinter as tk
 import pandas as pd
 import pandas.errors
 
 from empyric.types import recast, Type, Float
 from empyric.routines import SocketServer, ModbusServer
 
-if sys.platform == 'darwin':
+if sys.platform == "darwin":
     import matplotlib
 
-    matplotlib.use('TkAgg')  # works better on macOS
+    matplotlib.use("TkAgg")  # works better on macOS
 
 import matplotlib.pyplot as plt
 from matplotlib.cm import ScalarMappable
 import matplotlib.dates as mdates
 
 from pandas.plotting import register_matplotlib_converters
 
@@ -63,106 +63,101 @@
         self.full_data = self.numericize(data)
 
         self.plotted = []
 
         if settings:
             self.settings = settings
         else:
-            self.settings = {'Plot': {'x': 'Time', 'y': data.columns}}
+            self.settings = {"Plot": {"x": "Time", "y": data.columns}}
 
         self.plots = {}
         for plot_name in settings:
             self.plots[plot_name] = plt.subplots(
                 constrained_layout=True, figsize=(5, 4)
             )
 
     def save(self, plot_name=None, save_as=None):
         """Save the plots to PNG files in the working directory"""
 
         if plot_name:
             fig, ax = self.plots[plot_name]
             if save_as:
-                fig.savefig(save_as + '.png')
+                fig.savefig(save_as + ".png")
             else:
-                fig.savefig(plot_name + '.png')
+                fig.savefig(plot_name + ".png")
         else:
             for name, plot in self.plots.items():
                 fig, ax = plot
-                fig.savefig(name + '.png')
+                fig.savefig(name + ".png")
 
     def close(self, plot_name=None):
         """
         If the plot_name keyword argument is specified, close the corresponding
         plot. Otherwise, close all plots.
         """
 
         self.save()
 
         if plot_name:
             fig, _ = self.plots[plot_name]
             plt.close(fig)
         else:
-            plt.close('all')
+            plt.close("all")
 
     def plot(self):
         """Plot all plots"""
 
         # Update full data
         new_indices = np.setdiff1d(self.data.index, self.full_data.index)
         self.full_data = pd.concat(
             [self.full_data, self.numericize(self.data.loc[new_indices])]
         )
 
         # Make the plots, by name and style
 
         for name, settings in self.settings.items():
+            style = settings.get("style", "basic")
 
-            style = settings.get('style', 'basic')
-
-            if style == 'basic':
+            if style == "basic":
                 self._plot_basic(name)
-            elif style == 'averaged':
+            elif style == "averaged":
                 self._plot_basic(name, averaged=True)
-            elif style == 'errorbars':
+            elif style == "errorbars":
                 self._plot_basis(name, errorbars=True)
-            elif style == 'parametric':
+            elif style == "parametric":
                 self._plot_parametric(name)
             else:
-                raise AttributeError(
-                    f"Plotting style '{style}' not recognized!"
-                )
+                raise AttributeError(f"Plotting style '{style}' not recognized!")
 
     def _plot_basic(self, name, averaged=False, errorbars=False):
         """Make a simple plot, (possibly multiple) y vs. x"""
 
         fig, ax = self.plots[name]
 
-        x = self.settings[name].get('x', 'Time')
-        ys = np.array([self.settings[name]['y']]).flatten()
+        x = self.settings[name].get("x", "Time")
+        ys = np.array([self.settings[name]["y"]]).flatten()
 
         not_in_data = np.setdiff1d(np.concatenate([[x], ys]), self.data.columns)
         if not_in_data.size > 0:
             raise AttributeError(
                 f'{", ".join(not_in_data)} specified for plotting, '
-                'but not in variables!'
+                "but not in variables!"
             )
 
         if averaged or errorbars:
-
             grouped_data = self.full_data.groupby(x)
             averaged_data = grouped_data.mean()
             xdata = averaged_data[x]
             ydata = averaged_data[ys]
 
             if errorbars:
                 ystddata = grouped_data.std()[ys]
 
         else:
-
-            if x == 'Time':
+            if x == "Time":
                 xdata = self.full_data.index
             else:
                 xdata = self.full_data[x].astype(float)
 
             ydata = self.full_data[ys].astype(float)
 
         if ax.lines and not errorbars:
@@ -176,203 +171,195 @@
             ax.relim()  # reset plot limits based on data
             ax.autoscale_view()
 
             fig.canvas.draw_idle()
             fig.canvas.start_event_loop(0.01)
 
         else:  # draw a new plot
-
-            plot_kwargs = self.settings[name].get('configure', {})
+            plot_kwargs = self.settings[name].get("configure", {})
             # kwargs for matplotlib
 
             plot_kwargs = {
-                key: np.array([value]).flatten()
-                for key, value in plot_kwargs.items()
+                key: np.array([value]).flatten() for key, value in plot_kwargs.items()
             }
 
             if len(ys) > 1:  # a legend will be made
-                plot_kwargs['label'] = ys
+                plot_kwargs["label"] = ys
 
-            xscale = self.settings[name].get('x scale', 'linear')
-            yscale = self.settings[name].get('y scale', 'linear')
+            xscale = self.settings[name].get("x scale", "linear")
+            yscale = self.settings[name].get("y scale", "linear")
 
-            if x == 'Time':
+            if x == "Time":
                 ax.xaxis.set_major_locator(self.date_locator)
                 ax.xaxis.set_major_formatter(self.date_formatter)
 
             for i, y in enumerate(ys):
-
-                plot_kwargs_i = {
-                    key: value[i] for key, value in plot_kwargs.items()
-                }
+                plot_kwargs_i = {key: value[i] for key, value in plot_kwargs.items()}
 
                 if errorbars:
-                    ax.errorbar(
-                        xdata, ydata[y], yerr=ystddata[y], **plot_kwargs_i
-                    )
+                    ax.errorbar(xdata, ydata[y], yerr=ystddata[y], **plot_kwargs_i)
                 else:
                     ax.plot(xdata, ydata[y], **plot_kwargs_i)
 
-            if x == 'Time':
+            if x == "Time":
                 pass
                 # axis is automatically configured for datetimes; do not modify
-            elif xscale == 'linear':
+            elif xscale == "linear":
                 try:
-                    ax.ticklabel_format(
-                        axis='x', style='sci', scilimits=(-2, 4)
-                    )
+                    ax.ticklabel_format(axis="x", style="sci", scilimits=(-2, 4))
                 except AttributeError:
                     pass
             elif type(xscale) == dict:
                 for scale, options in xscale.items():
                     ax.set_xscale(scale, **options)
             else:
                 ax.set_xscale(xscale)
 
-            if yscale == 'linear':
+            if yscale == "linear":
                 try:
-                    ax.ticklabel_format(
-                        axis='y', style='sci', scilimits=(-2, 4)
-                    )
+                    ax.ticklabel_format(axis="y", style="sci", scilimits=(-2, 4))
                 except AttributeError:
                     pass
             elif type(yscale) == dict:
                 for scale, options in yscale.items():
                     ax.set_yscale(scale, **options)
             else:
                 ax.set_yscale(yscale)
 
             ax.set_title(name)
-            ax.tick_params(labelsize='small')
+            ax.tick_params(labelsize="small")
             ax.grid()
 
             if len(ys) > 1:
                 ax.legend()
 
-            if x != 'Time':
-                ax.set_xlabel(self.settings[name].get('xlabel', x))
-            ax.set_ylabel(self.settings[name].get('ylabel', ys[0]))
+            if x != "Time":
+                ax.set_xlabel(self.settings[name].get("xlabel", x))
+            ax.set_ylabel(self.settings[name].get("ylabel", ys[0]))
 
             plt.pause(0.01)
 
     def _plot_parametric(self, name):
         """Make a parametric plot of x and y against a third parameter"""
 
         fig, ax = self.plots[name]
 
-        x = self.settings[name]['x']
-        y = np.array([self.settings[name]['y']]).flatten()[0]
-        s = self.settings[name].get('s', 'Time')
+        x = self.settings[name]["x"]
+        y = np.array([self.settings[name]["y"]]).flatten()[0]
+        s = self.settings[name].get("s", "Time")
 
         not_in_data = np.setdiff1d([x, y, s], self.data.columns)
         if not_in_data.size > 0:
             raise AttributeError(
                 f'{", ".join(not_in_data)} specified for plotting, '
-                'but not in variables!'
+                "but not in variables!"
             )
 
         xdata = self.full_data[x].values
         ydata = self.full_data[y].values
         sdata = self.full_data[s].values
 
-        if s == 'Time':  # Rescale time if values are large
-            units = 'seconds'
+        if s == "Time":  # Rescale time if values are large
+            units = "seconds"
             if np.max(sdata) > 60:
-                units = 'minutes'
+                units = "minutes"
                 sdata = sdata / 60
                 if np.max(sdata) > 60:
-                    units = 'hours'
+                    units = "hours"
                     sdata = sdata / 60
 
         s_min, s_max = np.min(sdata), np.max(sdata)
         norm = plt.Normalize(vmin=s_min, vmax=s_max)
 
-        colormap = 'viridis'
-        plt.rcParams['image.cmap'] = colormap
-        cmap = plt.get_cmap('viridis')
+        colormap = "viridis"
+        plt.rcParams["image.cmap"] = colormap
+        cmap = plt.get_cmap("viridis")
 
-        plot_kwargs = self.settings[name].get('configure', {})
+        plot_kwargs = self.settings[name].get("configure", {})
         # kwargs for matplotlib
 
-        if not hasattr(fig, 'cbar'):  # draw a new plot
-
+        if not hasattr(fig, "cbar"):  # draw a new plot
             for i in range(len(xdata) - 1):
                 ax.plot(
-                    xdata[i: i + 2], ydata[i: i + 2],
+                    xdata[i : i + 2],
+                    ydata[i : i + 2],
                     color=cmap(norm(sdata[i])),
-                    **plot_kwargs
+                    **plot_kwargs,
                 )
 
             fig.scalarmappable = ScalarMappable(cmap=cmap, norm=norm)
             fig.scalarmappable.set_array(np.linspace(s_min, s_max, 1000))
             fig.cbar = plt.colorbar(fig.scalarmappable, ax=ax)
 
-            xscale = self.settings[name].get('x scale', 'linear')
-            yscale = self.settings[name].get('y scale', 'linear')
+            xscale = self.settings[name].get("x scale", "linear")
+            yscale = self.settings[name].get("y scale", "linear")
 
-            if xscale == 'linear':
-                ax.ticklabel_format(axis='x', style='sci', scilimits=(-2, 4))
+            if xscale == "linear":
+                ax.ticklabel_format(axis="x", style="sci", scilimits=(-2, 4))
             elif type(xscale) == dict:
                 for scale, options in xscale.items():
                     ax.set_xscale(scale, **options)
             else:
                 ax.set_xscale(xscale)
 
-            if yscale == 'linear':
-                ax.ticklabel_format(axis='y', style='sci', scilimits=(-2, 4))
+            if yscale == "linear":
+                ax.ticklabel_format(axis="y", style="sci", scilimits=(-2, 4))
             elif type(yscale) == dict:
                 for scale, options in yscale.items():
                     ax.set_yscale(scale, **options)
             else:
                 ax.set_yscale(yscale)
 
             ax.set_title(name)
             ax.grid(True)
-            ax.tick_params(labelsize='small')
-            ax.set_xlabel(self.settings[name].get('xlabel', x))
-            ax.set_ylabel(self.settings[name].get('ylabel', y))
+            ax.tick_params(labelsize="small")
+            ax.set_xlabel(self.settings[name].get("xlabel", x))
+            ax.set_ylabel(self.settings[name].get("ylabel", y))
 
-            if s == 'Time':
-                fig.cbar.ax.set_ylabel('Time ' + f" ({units})")
+            if s == "Time":
+                fig.cbar.ax.set_ylabel("Time " + f" ({units})")
             else:
                 fig.cbar.ax.set_ylabel(s)
 
-            fig.cbar.ax.tick_params(labelsize='small')
+            fig.cbar.ax.tick_params(labelsize="small")
 
             try:
+                # Optimize plot layout using the figure's layout engine
                 fig.get_layout_engine().execute(fig)
             except AttributeError:  # sometimes happens for reasons
                 pass
+            except ZeroDivisionError:  # sometimes happens for reasons
+                pass
 
             plt.pause(0.01)
 
         else:  # if already plotted, update the plot data and axes
-
             # update color bar
             fig.scalarmappable.set_clim(vmin=s_min, vmax=s_max)
             fig.cbar.update_normal(fig.scalarmappable)
 
             # update_normal method above removes the colorbar's ylabel;
             # redraw it
-            if s == 'Time':
-                fig.cbar.ax.set_ylabel('Time ' + f" ({units})")
+            if s == "Time":
+                fig.cbar.ax.set_ylabel("Time " + f" ({units})")
             else:
                 fig.cbar.ax.set_ylabel(s)
 
             # update colors of existing line segments
             for i, line in enumerate(ax.lines):
                 line.set_color(cmap(norm(sdata[i])))
                 ax.draw_artist(line)
 
             # plot new line segments
             for i in range(len(ax.lines) - 1, len(xdata) - 1):
                 ax.plot(
-                    xdata[i: i + 2], ydata[i: i + 2],
+                    xdata[i : i + 2],
+                    ydata[i : i + 2],
                     color=cmap(norm(sdata[i])),
-                    **plot_kwargs
+                    **plot_kwargs,
                 )
 
             ax.relim()
             ax.autoscale_view()
 
             fig.canvas.draw_idle()
             fig.canvas.start_event_loop(0.01)
@@ -390,41 +377,36 @@
         data_array = data.values
 
         numerical_indices = []
         numerical_array = [[]] * len(labels)
 
         # Iterate through each row and expand any files or lists into columns
         for index, row in zip(indices, data_array):
-
             columns = []
             max_len = 0  # maximum length of columns
             for i, element in enumerate(row):
-
                 if type(element) == str and os.path.isfile(element):
-
                     file_read = False
                     attempt = 0
                     while not file_read:
                         try:
                             expanded_element = list(
                                 pd.read_csv(element)[labels[i]].values
                             )
 
                             file_read = True
                         except pandas.errors.EmptyDataError:
-
                             if attempt > 3:
                                 expanded_element = [np.nan]
                                 break
 
                             attempt += 1
                             plt.pause(1)
 
                 elif np.ndim(element) == 1:
-
                     expanded_element = list(element)
 
                     expanded_element = [
                         value if value is not None else np.nan
                         for value in expanded_element
                     ]
 
@@ -441,17 +423,15 @@
             numerical_indices = numerical_indices + [index] * max_len
             for i, column in enumerate(columns):
                 # fill remainder of column with most recent value
                 new_elements = column + [column[-1]] * (max_len - len(column))
                 numerical_array[i] = numerical_array[i] + new_elements
 
         numerical_data = pd.DataFrame(
-            data=np.array(numerical_array).T,
-            columns=labels,
-            index=numerical_indices
+            data=np.array(numerical_array).T, columns=labels, index=numerical_indices
         )
 
         return numerical_data
 
 
 class ExperimentGUI:
     """
@@ -460,256 +440,261 @@
 
     This GUI allows the user to hold, stop and terminate the experiment. When
     stopped, the user can change the values of knob and parameter variables,
     and also directly interact with instruments through the Dashboard.
     """
 
     def __init__(self, experiment, title=None, **kwargs):
-
         self.experiment = experiment
 
         if title:
             self.title = title
         else:
-            self.title = 'Empyric'
+            self.title = "Empyric"
 
         self.closed = False  # has the GUI been closed?
 
         self.variables = experiment.variables
 
-        self.alarms = kwargs.get('alarms', {})
+        self.alarms = kwargs.get("alarms", {})
 
-        if 'instruments' in kwargs:
-            self.instruments = kwargs['instruments']
+        if "instruments" in kwargs:
+            self.instruments = kwargs["instruments"]
         else:
             # If instruments are not specified,
             # get them from the experiment variables
             self.instruments = {}
             for variable in self.experiment.variables.values():
-                if variable.type in ['meter', 'knob']:
+                if variable.type in ["meter", "knob"]:
                     instrument = variable.instrument
                     if instrument.name not in self.instruments:
                         self.instruments[instrument.name] = instrument
 
-        if ('plots' in kwargs and kwargs['plotter'] is not None) \
-                or ('plotter' in kwargs and kwargs['plotter'] is not None):
-
-            if 'plotter' in kwargs:
-                self.plotter = kwargs['plotter']
+        if ("plots" in kwargs and kwargs["plotter"] is not None) or (
+            "plotter" in kwargs and kwargs["plotter"] is not None
+        ):
+            if "plotter" in kwargs:
+                self.plotter = kwargs["plotter"]
             else:
-                self.plotter = Plotter(experiment.data, kwargs['plots'])
+                self.plotter = Plotter(experiment.data, kwargs["plots"])
 
-            self.plot_interval = kwargs.get('plot_interval', 0)
+            self.plot_interval = kwargs.get("plot_interval", 0)
             # grows if plotting takes longer
 
-            self.last_plot = float('-inf')
+            self.last_plot = float("-inf")
 
             # Set interval for saving plots
-            self.save_interval = kwargs.get('save_interval', 0)
+            self.save_interval = kwargs.get("save_interval", 0)
 
             self.last_save = time.time()
 
         self.root = tk.Tk()
         self.root.lift()
-        self.root.wm_attributes('-topmost', True)  # bring window to front
+        self.root.wm_attributes("-topmost", True)  # bring window to front
         self.root.protocol("WM_DELETE_WINDOW", self.end)
 
         self.root.title(self.title)
         self.root.resizable(False, False)
 
         self.status_frame = tk.Frame(self.root)
         self.status_frame.grid(row=0, column=0, columnspan=2)
 
         i = 0
-        title = kwargs.get('title', 'Experiment')
+        title = kwargs.get("title", "Experiment")
 
-        tk.Label(
-            self.status_frame, text=title, font=("Arial", 14, 'bold')
-        ).grid(row=i, column=1)
+        tk.Label(self.status_frame, text=title, font=("Arial", 14, "bold")).grid(
+            row=i, column=1
+        )
 
         # Status field shows current experiment status
         i += 1
         tk.Label(
-            self.status_frame, text='Status', width=len('Status'), anchor=tk.E
+            self.status_frame, text="Status", width=len("Status"), anchor=tk.E
         ).grid(row=i, column=0, sticky=tk.E)
 
         self.status_label = tk.Label(
-            self.status_frame, text='', width=30, relief=tk.SUNKEN
+            self.status_frame, text="", width=30, relief=tk.SUNKEN
         )
         self.status_label.grid(row=i, column=1, sticky=tk.W, padx=10)
 
         # Table of variables shows most recently measured/set variable values
         self.variable_entries = {}
         self._entry_enter_funcs = {}  # container for enter press event handlers
         self._entry_esc_funcs = {}  # container for esc press event handlers
 
         i += 1
-        tk.Label(
-            self.status_frame, text='', font=("Arial", 14, 'bold')
-        ).grid(row=i, column=0, sticky=tk.E)
+        tk.Label(self.status_frame, text="", font=("Arial", 14, "bold")).grid(
+            row=i, column=0, sticky=tk.E
+        )
 
         i += 1
-        tk.Label(
-            self.status_frame, text='Variables', font=("Arial", 14, 'bold')
-        ).grid(row=i, column=1)
+        tk.Label(self.status_frame, text="Variables", font=("Arial", 14, "bold")).grid(
+            row=i, column=1
+        )
 
         i += 1
         tk.Label(
-            self.status_frame, text='Run Time', width=len('Run Time'),
-            anchor=tk.E
+            self.status_frame, text="Run Time", width=len("Run Time"), anchor=tk.E
         ).grid(row=i, column=0, sticky=tk.E)
 
-        self.variable_entries['Time'] = tk.Entry(
-            self.status_frame, state='readonly', disabledforeground='black',
-            width=30
-        )
-        self.variable_entries['Time'].grid(
-            row=i, column=1, sticky=tk.W, padx=10
+        self.variable_entries["Time"] = tk.Entry(
+            self.status_frame, state="readonly", disabledforeground="black", width=30
         )
+        self.variable_entries["Time"].grid(row=i, column=1, sticky=tk.W, padx=10)
 
         i += 1
         for name in self.variables:
-            tk.Label(
-                self.status_frame, text=name, width=len(name), anchor=tk.E
-            ).grid(row=i, column=0, sticky=tk.E)
+            tk.Label(self.status_frame, text=name, width=len(name), anchor=tk.E).grid(
+                row=i, column=0, sticky=tk.E
+            )
 
             self.variable_entries[name] = tk.Entry(
-                self.status_frame, state='readonly', disabledforeground='black',
-                width=30
-            )
-            self.variable_entries[name].grid(
-                row=i, column=1, sticky=tk.W, padx=10
+                self.status_frame,
+                state="readonly",
+                disabledforeground="black",
+                width=30,
             )
+            self.variable_entries[name].grid(row=i, column=1, sticky=tk.W, padx=10)
 
             if self.variables[name].settable:
                 entry = self.variable_entries[name]
                 variable = self.variables[name]
                 root = self.status_frame
 
-                enter_func = \
-                    lambda event, entry=entry, variable=variable, root=root: \
-                        self._entry_enter(entry, variable, root)
+                enter_func = lambda event, entry=entry, variable=variable, root=root: self._entry_enter(
+                    entry, variable, root
+                )
 
                 self._entry_enter_funcs[name] = enter_func
                 self.variable_entries[name].bind(
-                    '<Return>', self._entry_enter_funcs[name]
+                    "<Return>", self._entry_enter_funcs[name]
                 )
 
-                esc_func = \
-                    lambda event, entry=entry, variable=variable, root=root: \
-                        self._entry_esc(entry, variable, root)
+                esc_func = lambda event, entry=entry, variable=variable, root=root: self._entry_esc(
+                    entry, variable, root
+                )
 
                 self._entry_esc_funcs[name] = esc_func
                 self.variable_entries[name].bind(
-                    '<Escape>', self._entry_esc_funcs[name]
+                    "<Escape>", self._entry_esc_funcs[name]
                 )
 
             i += 1
 
         i += 1
-        tk.Label(
-            self.status_frame, text='', font=("Arial", 14, 'bold')
-        ).grid(row=i, column=0, sticky=tk.E)
+        tk.Label(self.status_frame, text="", font=("Arial", 14, "bold")).grid(
+            row=i, column=0, sticky=tk.E
+        )
 
         # Table of alarm indicators shows the status of any alarms monitored
         self.alarm_status_labels = {}
 
         if len(self.alarms) > 0:
-
             i += 1
-            tk.Label(
-                self.status_frame, text='Alarms', font=("Arial", 14, 'bold')
-            ).grid(row=i, column=1)
+            tk.Label(self.status_frame, text="Alarms", font=("Arial", 14, "bold")).grid(
+                row=i, column=1
+            )
 
             i += 1
             for alarm in self.alarms:
                 tk.Label(
-                    self.status_frame, text=alarm, width=len(alarm),
-                    anchor=tk.E
+                    self.status_frame, text=alarm, width=len(alarm), anchor=tk.E
                 ).grid(row=i, column=0, sticky=tk.E)
 
                 self.alarm_status_labels[alarm] = tk.Label(
-                    self.status_frame, text='Clear', relief=tk.SUNKEN, width=30
+                    self.status_frame, text="Clear", relief=tk.SUNKEN, width=30
                 )
                 self.alarm_status_labels[alarm].grid(
                     row=i, column=1, sticky=tk.W, padx=10
                 )
 
                 i += 1
 
-            tk.Label(
-                self.status_frame, text='', font=("Arial", 14, 'bold')
-            ).grid(row=i, column=0, sticky=tk.E)
+            tk.Label(self.status_frame, text="", font=("Arial", 14, "bold")).grid(
+                row=i, column=0, sticky=tk.E
+            )
 
         # Servers
         self.servers = {
-            name: routine for name, routine in self.experiment.routines.items()
-            if isinstance(routine, SocketServer)
-            or isinstance(routine, ModbusServer)
+            name: routine
+            for name, routine in self.experiment.routines.items()
+            if isinstance(routine, SocketServer) or isinstance(routine, ModbusServer)
         }
 
         if self.servers:
-
             self.server_status_labels = {}
 
             i += 1
             tk.Label(
-                self.status_frame, text='Servers', font=("Arial", 14, 'bold')
+                self.status_frame, text="Servers", font=("Arial", 14, "bold")
             ).grid(row=i, column=1)
 
             i += 1
             for server in self.servers:
-
                 tk.Label(
-                    self.status_frame, text=server, width=len(server),
-                    anchor=tk.E
+                    self.status_frame, text=server, width=len(server), anchor=tk.E
                 ).grid(row=i, column=0, sticky=tk.E)
 
                 ip_address = self.servers[server].ip_address
                 port = self.servers[server].port
 
                 # Make entry so text is selectable
                 self.server_status_labels[server] = tk.Entry(
-                    self.status_frame, disabledforeground='black',
+                    self.status_frame,
+                    disabledforeground="black",
                 )
 
-                self.server_status_labels[server].insert(
-                    0, f'{ip_address}::{port}'
-                )
-                self.server_status_labels[server].config(state='readonly')
+                self.server_status_labels[server].insert(0, f"{ip_address}::{port}")
+                self.server_status_labels[server].config(state="readonly")
 
                 self.server_status_labels[server].grid(
                     row=i, column=1, sticky=tk.W, padx=10
                 )
 
                 i += 1
 
         # Buttons (root is not self.status_frame, so indexing starts at 1)
         i = 1
         self.dash_button = tk.Button(
-            self.root, text='Dashboard', font=("Arial", 14, 'bold'), width=10,
-            command=self.open_dashboard, state=tk.DISABLED
+            self.root,
+            text="Dashboard",
+            font=("Arial", 14, "bold"),
+            width=10,
+            command=self.open_dashboard,
+            state=tk.DISABLED,
         )
         self.dash_button.grid(row=i, column=0, sticky=tk.W)
 
         self.hold_button = tk.Button(
-            self.root, text='Hold', font=("Arial", 14, 'bold'), width=10,
-            command=self.toggle_hold
+            self.root,
+            text="Hold",
+            font=("Arial", 14, "bold"),
+            width=10,
+            command=self.toggle_hold,
         )
         self.hold_button.grid(row=i + 1, column=0, sticky=tk.W)
 
         self.stop_button = tk.Button(
-            self.root, text='Stop', font=("Arial", 14, 'bold'), width=10,
-            command=self.toggle_stop
+            self.root,
+            text="Stop",
+            font=("Arial", 14, "bold"),
+            width=10,
+            command=self.toggle_stop,
         )
         self.stop_button.grid(row=i + 2, column=0, sticky=tk.W)
 
         self.terminate_button = tk.Button(
-            self.root, text='Terminate', font=("Arial", 14, 'bold'), width=10,
-            fg='red', bg='gray87', command=self.end, height=5
+            self.root,
+            text="Terminate",
+            font=("Arial", 14, "bold"),
+            width=10,
+            fg="red",
+            bg="gray87",
+            command=self.end,
+            height=5,
         )
         self.terminate_button.grid(row=i, column=1, sticky=tk.E, rowspan=3)
 
     def run(self):
         """Starts the Tkinter mainloop and the experiment update loop"""
         self.update()
         self.root.mainloop()
@@ -717,123 +702,116 @@
     def update(self):
         """Updates the GUI based on the state of the experiment"""
 
         if self.closed:
             return  # don't update GUI if it no longer exists
 
         # Allow window to fall back once things get started
-        self.root.wm_attributes('-topmost', False)
+        self.root.wm_attributes("-topmost", False)
 
         state = self.experiment.state
 
         # Update all variable entries based on experiment state
         for name, entry in self.variable_entries.items():
-
             # If stopped or holding allow user to edit knobs or parameters
             if self.experiment.stopped or self.experiment.holding:
-                if name != 'Time' and self.variables[name].settable:
+                if name != "Time" and self.variables[name].settable:
                     continue
 
             def write_entry(_entry, text):
                 _entry.config(state=tk.NORMAL)
                 _entry.delete(0, tk.END)
                 _entry.insert(0, text)
                 _entry.config(state=tk.DISABLED)
 
             if state[name] is None:
-                write_entry(entry, 'None')
+                write_entry(entry, "None")
             elif state[name] == np.nan:
-                write_entry(entry, 'NaN')
+                write_entry(entry, "NaN")
             else:
-                if name == 'Time':
-                    write_entry(
-                        entry, str(datetime.timedelta(seconds=state['Time']))
-                    )
+                if name == "Time":
+                    write_entry(entry, str(datetime.timedelta(seconds=state["Time"])))
                 elif isinstance(state[name], Float):
                     # display floating point numbers neatly
                     if state[name] == 0.0:
-                        write_entry(entry, '0.0')
+                        write_entry(entry, "0.0")
                     elif np.abs(np.log10(np.abs(state[name]))) > 3:
-                        write_entry(entry, '%.3e' % state[name])
+                        write_entry(entry, "%.3e" % state[name])
                     else:
-                        write_entry(entry, '%.3f' % state[name])
+                        write_entry(entry, "%.3f" % state[name])
                 else:
                     write_entry(entry, str(state[name]))
 
         self.status_label.config(text=self.experiment.status)
 
         # Check alarms
         for name, label in self.alarm_status_labels.items():
             if self.alarms[name].triggered:
                 protocol = self.alarms[name].protocol
-                if protocol == 'none':
-                    label.config(text='TRIGGERED: NO PROTOCOL', bg='red')
+                if protocol == "none":
+                    label.config(text="TRIGGERED: NO PROTOCOL", bg="red")
                 else:
-                    label.config(
-                        text='TRIGGERED' + f': {protocol.upper()}', bg='red'
-                    )
+                    label.config(text="TRIGGERED" + f": {protocol.upper()}", bg="red")
             else:
-                label.config(text="CLEAR", bg='green')
+                label.config(text="CLEAR", bg="green")
 
         # Update hold, stop and dashboard buttons
         if self.experiment.holding or self.experiment.stopped:
             self.dash_button.config(state=tk.NORMAL)
 
             if self.experiment.holding:
-                self.hold_button.config(text='Resume')
-                self.stop_button.config(text='Stop')
+                self.hold_button.config(text="Resume")
+                self.stop_button.config(text="Stop")
             else:
-                self.hold_button.config(text='Hold')
-                self.stop_button.config(text='Resume')
+                self.hold_button.config(text="Hold")
+                self.stop_button.config(text="Resume")
 
             # Settable variable values can be edited
             for name, entry in self.variable_entries.items():
-                if name != 'Time' and self.variables[name].settable:
+                if name != "Time" and self.variables[name].settable:
                     entry.config(state=tk.NORMAL)
 
         else:  # otherwise, experiment is running
             self.dash_button.config(state=tk.DISABLED)
-            self.hold_button.config(text='Hold')
-            self.stop_button.config(text='Stop')
+            self.hold_button.config(text="Hold")
+            self.stop_button.config(text="Stop")
 
             for entry in self.variable_entries.values():
                 entry.config(state=tk.DISABLED)
 
         # Quit if experiment has ended
         if self.experiment.terminated:
             self.quit()
 
         # Plot data
-        has_plotter = hasattr(self, 'plotter')
+        has_plotter = hasattr(self, "plotter")
         has_data = len(self.experiment.data) > 0
         not_stopped = not self.experiment.stopped
         if has_plotter and has_data and not_stopped:
             if time.time() > self.last_plot + self.plot_interval:
                 start_plot = time.perf_counter()
                 self.plotter.plot()
                 end_plot = time.perf_counter()
                 self.last_plot = time.time()
 
-                self.plot_interval = np.max([
-                    self.plot_interval,
-                    5 * int(end_plot - start_plot)
-                ])  # adjust interval if drawing plots takes significant time
+                self.plot_interval = np.max(
+                    [self.plot_interval, 5 * int(end_plot - start_plot)]
+                )  # adjust interval if drawing plots takes significant time
 
             # Save plots
             saving_needed = time.time() > self.last_save + self.save_interval
             if saving_needed and self.experiment.timestamp:
                 start_save = time.perf_counter()
                 self.plotter.save()
                 end_save = time.perf_counter()
                 self.last_save = time.time()
 
-                self.save_interval = np.max([
-                    self.save_interval,
-                    5 * int(end_save - start_save)
-                ])  # adjust interval if saving plots takes significant time
+                self.save_interval = np.max(
+                    [self.save_interval, 5 * int(end_save - start_save)]
+                )  # adjust interval if saving plots takes significant time
 
         if not self.closed:
             self.root.after(50, self.update)
 
     def open_dashboard(self):
         """
         When the user hits the Dashboard button, open a window which allows
@@ -846,17 +824,17 @@
         self.experiment.stop()
         # stop routines and measurements to avoid communication conflicts
         # while dashboard is open
 
         Dashboard(self.root, self.instruments)
 
         # Return experiment to prior state
-        if 'Holding' in prior_status:
+        if "Holding" in prior_status:
             self.experiment.hold()
-        elif 'Ready' in prior_status or 'Running' in prior_status:
+        elif "Ready" in prior_status or "Running" in prior_status:
             self.experiment.start()
 
     def toggle_hold(self):
         """User pauses/resumes the experiment through the Hold/Resume button."""
 
         if self.experiment.holding:
             self.experiment.start()
@@ -873,20 +851,19 @@
 
     def end(self):
         """
         User terminates the experiment and closes the GUI with the Terminate
         button; cancels any experiment follow-ups.
         """
 
-        self.experiment.terminate(reason='user terminated')
+        self.experiment.terminate(reason="user terminated")
         self.quit()
 
     def quit(self):
-
-        if hasattr(self, 'plotter'):
+        if hasattr(self, "plotter"):
             self.plotter.close()
 
         self.status_label.config(text=self.experiment.TERMINATED)
 
         self.closed = True
         plt.pause(0.1)  # give GUI and plotter enough time to wrap up
         self.root.update()
@@ -895,16 +872,15 @@
         self.root.quit()
 
     @staticmethod
     def _entry_enter(entry, variable, root):
         """Assigns the value to a variable if entered by the user"""
 
         variable.value = recast(
-            entry.get(),
-            to=variable.type if variable.type is not None else Type
+            entry.get(), to=variable.type if variable.type is not None else Type
         )
 
         root.focus()
 
     @staticmethod
     def _entry_esc(entry, variable, root):
         """Restores the value of a variable to an entry if user escapes entry"""
@@ -915,32 +891,31 @@
         try:
             value = float(value)
         except ValueError:
             pass
 
         if type(value) == float:
             if value == 0:
-                entry.insert(0, '0.0')
+                entry.insert(0, "0.0")
             elif np.abs(np.log10(np.abs(value))) > 3:
-                entry.insert(0, '%.3e' % value)
+                entry.insert(0, "%.3e" % value)
             else:
-                entry.insert(0, '%.3f' % value)
+                entry.insert(0, "%.3f" % value)
         else:
             entry.insert(0, str(value))
 
         root.focus()
 
 
 class BasicDialog(tk.Toplevel):
     """
     General purpose dialog window
     """
 
     def __init__(self, parent, title=None):
-
         tk.Toplevel.__init__(self, parent)
         self.transient(parent)
 
         if title:
             self.title(title)
 
         self.parent = parent
@@ -956,16 +931,15 @@
         self.grab_set()
 
         if not self.initial_focus:
             self.initial_focus = self
 
         self.protocol("WM_DELETE_WINDOW", self.ok)
 
-        self.geometry("+%d+%d" % (parent.winfo_rootx() + 50,
-                                  parent.winfo_rooty() + 50))
+        self.geometry("+%d+%d" % (parent.winfo_rootx() + 50, parent.winfo_rooty() + 50))
 
         self.initial_focus.focus_set()
 
         self.wait_window(self)
 
     # construction hooks
 
@@ -977,71 +951,68 @@
 
     def buttonbox(self):
         # add standard button box. override if you don't want the
         # standard buttons
 
         box = tk.Frame(self)
 
-        w = tk.Button(
-            box, text="OK", width=10, command=self.ok, default=tk.ACTIVE
-        )
+        w = tk.Button(box, text="OK", width=10, command=self.ok, default=tk.ACTIVE)
         w.pack(side=tk.LEFT, padx=5, pady=5)
 
         self.bind("<Return>", self.ok)
 
         box.pack()
 
     # standard button semantics
 
     def ok(self, event=None):
-
         if not self.validate():
             self.initial_focus.focus_set()  # put focus back
             return
 
         self.withdraw()
         self.update_idletasks()
 
         self.parent.focus_set()
         self.destroy()
 
     def validate(self):
-
         return 1  # override
 
 
 class Dashboard(BasicDialog):
     """
     Allows the user to configure instruments while running up an experiment
     """
 
     def __init__(self, parent, instruments):
         self.instruments = instruments
 
-        BasicDialog.__init__(self, parent, title='Dashboard')
+        BasicDialog.__init__(self, parent, title="Dashboard")
 
     def body(self, master):
-        tk.Label(
-            master, text='Instruments:', font=('Arial', 14), justify=tk.LEFT
-        ).grid(row=0, column=0, sticky=tk.W)
+        tk.Label(master, text="Instruments:", font=("Arial", 14), justify=tk.LEFT).grid(
+            row=0, column=0, sticky=tk.W
+        )
 
         i = 1
 
         self.instrument_labels = {}
         self.config_buttons = {}
 
         for name, instrument in self.instruments.items():
             instrument_label = tk.Label(master, text=name)
             instrument_label.grid(row=i, column=0)
 
             self.instrument_labels[name] = instrument_label
 
             config_button = tk.Button(
-                master, text='Config/Test',
-                command=lambda instr=instrument: self.config(instr)
+                master,
+                text="Config/Test",
+                command=lambda instr=instrument: self.config(instr),
             )
             config_button.grid(row=i, column=1)
 
             self.config_buttons[name] = config_button
 
             i += 1
 
@@ -1053,114 +1024,106 @@
     """
     Dialog box for setting knobs and checking meters.
     Allows the user to quickly access basic instrument functionality as well as
     configure instrument for an experiment.
     """
 
     def __init__(self, parent, instrument):
-
         self.instrument = instrument
-        BasicDialog.__init__(
-            self, parent, title='Config/Test: ' + instrument.name
-        )
+        BasicDialog.__init__(self, parent, title="Config/Test: " + instrument.name)
 
     def set_knob_entry(self, knob):
         value = self.knob_entries[knob].get()
-        self.instrument.set(knob.replace(' ', '_'), recast(value))
+        self.instrument.set(knob.replace(" ", "_"), recast(value))
 
     def get_knob_entry(self, knob):
-
-        if hasattr(self.instrument, 'get_'+knob.replace(' ', '_')):
+        if hasattr(self.instrument, "get_" + knob.replace(" ", "_")):
             value = self.instrument.get(knob)
         else:
-            value = getattr(self.instrument, knob.replace(' ', '_'))
+            value = getattr(self.instrument, knob.replace(" ", "_"))
 
         self.knob_entries[knob].delete(0, tk.END)
         self.knob_entries[knob].insert(0, str(value))
 
     def update_meter_entry(self, meter):
-
         value = self.instrument.measure(meter)
 
         if np.ndim(value) == 1:  # store array data as CSV files
             dataframe = pd.DataFrame({meter: value})
-            path = self.instrument.name + '-' + meter.replace(' ', '_') + '_'
+            path = self.instrument.name + "-" + meter.replace(" ", "_") + "_"
             now = datetime.datetime.now()
-            path += now.strftime('%Y%m%d-%H%M%S') + '.csv'
+            path += now.strftime("%Y%m%d-%H%M%S") + ".csv"
             dataframe.to_csv(path)
 
             value = path
 
         self.meter_entries[meter].config(state=tk.NORMAL)
         self.meter_entries[meter].delete(0, tk.END)
         self.meter_entries[meter].insert(0, str(value))
-        self.meter_entries[meter].config(state='readonly')
+        self.meter_entries[meter].config(state="readonly")
 
     def body(self, master):
-
         knobs = self.instrument.knobs
         knob_values = {
-            knob: getattr(self.instrument, knob.replace(' ', '_'))
-            for knob in knobs
+            knob: getattr(self.instrument, knob.replace(" ", "_")) for knob in knobs
         }
         self.knob_entries = {}
 
         meters = self.instrument.meters
         self.meter_entries = {}
 
-        label = tk.Label(master, text='Knobs', font=("Arial", 14, 'bold'))
+        label = tk.Label(master, text="Knobs", font=("Arial", 14, "bold"))
         label.grid(row=0, column=0, sticky=tk.W)
 
-        label = tk.Label(master, text='Meters', font=("Arial", 14, 'bold'))
+        label = tk.Label(master, text="Meters", font=("Arial", 14, "bold"))
         label.grid(row=0, column=3, sticky=tk.W)
 
         self.set_buttons = {}
         self.get_buttons = {}
         i = 1
         for knob in knobs:
-            formatted_name = ' '.join(
-                [word[0].upper() + word[1:] for word in knob.split(' ')]
+            formatted_name = " ".join(
+                [word[0].upper() + word[1:] for word in knob.split(" ")]
             )
 
             label = tk.Label(master, text=formatted_name)
             label.grid(row=i, column=0, sticky=tk.W)
 
             self.knob_entries[knob] = tk.Entry(master)
             self.knob_entries[knob].grid(row=i, column=1)
             self.knob_entries[knob].insert(0, str(knob_values[knob]))
 
             self.set_buttons[knob] = tk.Button(
-                master, text='Set',
-                command=lambda knob=knob: self.set_knob_entry(knob)
+                master, text="Set", command=lambda knob=knob: self.set_knob_entry(knob)
             )
             self.set_buttons[knob].grid(row=i, column=2)
 
             self.get_buttons[knob] = tk.Button(
-                master, text='Get',
-                command=lambda knob=knob: self.get_knob_entry(knob)
+                master, text="Get", command=lambda knob=knob: self.get_knob_entry(knob)
             )
             self.get_buttons[knob].grid(row=i, column=3)
 
             i += 1
 
         self.measure_buttons = {}
         i = 1
         for meter in meters:
-            formatted_name = ' '.join(
-                [word[0].upper() + word[1:] for word in meter.split(' ')]
+            formatted_name = " ".join(
+                [word[0].upper() + word[1:] for word in meter.split(" ")]
             )
 
             label = tk.Label(master, text=formatted_name)
             label.grid(row=i, column=4, sticky=tk.W)
 
             self.meter_entries[meter] = tk.Entry(master)
             self.meter_entries[meter].grid(row=i, column=5)
-            self.meter_entries[meter].insert(0, '???')
-            self.meter_entries[meter].config(state='readonly')
+            self.meter_entries[meter].insert(0, "???")
+            self.meter_entries[meter].config(state="readonly")
 
             self.measure_buttons[meter] = tk.Button(
-                master, text='Measure',
-                command=lambda meter=meter: self.update_meter_entry(meter)
+                master,
+                text="Measure",
+                command=lambda meter=meter: self.update_meter_entry(meter),
             )
             self.measure_buttons[meter].grid(row=i, column=6)
 
             i += 1
```

### Comparing `empyric-0.2.0/empyric/instruments.py` & `empyric-0.2.3/empyric/instruments.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,9 +10,12 @@
 from empyric.collection.humans import *
 from empyric.collection.spectrometers import *
 from empyric.collection.virtual import *
 from empyric.collection.generators import *
 from empyric.collection.scopes import *
 from empyric.collection.io import *
 
-supported = {key: value for key, value in vars().items()
-             if type(value) is type and issubclass(value, Instrument)}
+supported = {
+    key: value
+    for key, value in vars().items()
+    if type(value) is type and issubclass(value, Instrument)
+}
```

### Comparing `empyric-0.2.0/empyric/routines.py` & `empyric-0.2.3/empyric/routines.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,32 @@
 import time
 import select
 import functools
 
 import numpy as np
 import pandas as pd
 
-from empyric.tools import convert_time, autobind_socket, read_from_socket, \
-    write_to_socket, get_ip_address
-from empyric.types import recast, Boolean, Integer, Float, Toggle, OFF, ON, \
-    Array, String
+from empyric.tools import (
+    convert_time,
+    autobind_socket,
+    read_from_socket,
+    write_to_socket,
+    get_ip_address,
+)
+from empyric.types import (
+    recast,
+    Boolean,
+    Integer,
+    Float,
+    Toggle,
+    OFF,
+    ON,
+    Array,
+    String,
+)
 from empyric.types import supported as supported_types
 from empyric.variables import Variable
 
 
 class Routine:
     """
     A Routine periodically updates a set of `knobs` based on a given state of an
@@ -32,32 +46,30 @@
 
     All other arguments are fixed values or string dictionary keys,
     corresponding to variables values of the controlling experiment.
     """
 
     assert_control = True
 
-    def __init__(self,
-                 knobs: dict,
-                 enable: String = None,
-                 start=0.0, end=np.inf, **kwargs):
-
+    def __init__(
+        self, knobs: dict, enable: String = None, start=0.0, end=np.inf, **kwargs
+    ):
         self.knobs = knobs
 
         for knob in self.knobs.values():
             knob._controller = None  # to control access to knob
 
         self.enable = enable
         self.start = convert_time(start)
         self.end = convert_time(end)
         self.prepped = False
         self.finished = False
 
         for key, value in kwargs.items():
-            self.__setattr__(key.replace(' ', '_'), value)
+            self.__setattr__(key.replace(" ", "_"), value)
 
     @staticmethod
     def enabler(update):
         """
         Checks the enabling variable, start and stop times for the
         routine. If the enable variable evaluates to `True` and the time is
         between the start and stop times, the update method is called.
@@ -68,44 +80,40 @@
         Otherwise, if the time is before the start time, the routine's prep
         method is called. If the time is after the end time, the routine's
         cleanup method is called.
         """
 
         @functools.wraps(update)
         def wrapped_update(self, state):
-
             if self.enable is not None and not state[self.enable]:
                 for name, knob in self.knobs.items():
                     if knob._controller == self:
                         knob._controller = None
                 return
 
-            elif state['Time'] < self.start:
-
+            elif state["Time"] < self.start:
                 if not self.prepped:
                     self.prep(state)
                     self.prepped = True
 
                 return
 
-            elif state['Time'] >= self.end:
-
+            elif state["Time"] >= self.end:
                 if not self.finished:
                     self.finish(state)
                     self.finished = True
 
                     # Release knobs from control
                     for name, knob in self.knobs.items():
                         if knob._controller == self:
                             knob._controller = None
 
                 return
 
             else:
-
                 for name, knob in self.knobs.items():
                     if knob._controller and knob._controller != self:
                         # take no action if another routine has control
                         return
                     elif self.assert_control:
                         # assert control if needed
                         knob._controller = self
@@ -149,32 +157,26 @@
     """
     Sets `knobs` to the given values.
 
     The `values` argument should be either a single key/value for all knobs or
     a 1D array of keys/values of the same length as the `knobs` argument.
     """
 
-    def __init__(self,
-                 knobs: dict,
-                 values,
-                 **kwargs):
-
+    def __init__(self, knobs: dict, values, **kwargs):
         Routine.__init__(self, knobs, **kwargs)
 
         if len(self.knobs) > 1 and np.ndim(values) == 0:
             # One value for all knobs
             self.values = [values] * len(self.knobs)
         else:
             self.values = values
 
     @Routine.enabler
     def update(self, state):
-
         for knob, value in zip(self.knobs.values(), self.values):
-
             if isinstance(value, str):
                 value = state[value]
 
             if value:
                 knob.value = value
 
 
@@ -182,19 +184,15 @@
     """
     Ramps the set of `knobs` to given `target` values at `given rates`.
 
     The `target` or `rate` arguments can be single keys/values for all knobs, or
     1D arrays of keys/values.
     """
 
-    def __init__(self,
-                 knobs: dict,
-                 targets,
-                 rates,
-                 **kwargs):
+    def __init__(self, knobs: dict, targets, rates, **kwargs):
         """
         :param rates: (1D array) list of ramp rates
         """
 
         Routine.__init__(self, knobs, **kwargs)
 
         if np.ndim(rates) == 0:  # single rate for all knobs
@@ -207,63 +205,59 @@
         self.targets = targets
 
         self.now = None
         self.then = None
 
     @Routine.enabler
     def update(self, state):
-
-        self.now = state['Time']
+        self.now = state["Time"]
 
         if self.then is None:
-            self.then = state['Time']
+            self.then = state["Time"]
 
         for knob, rate, target in zip(self.knobs, self.rates, self.targets):
-
             if isinstance(target, String):
                 target = state[target]
 
             if isinstance(rate, String):
                 rate = state[rate]
 
             val_now = self.knobs[knob]._value
 
-            if not isinstance(target, numbers.Number) \
-                    or not isinstance(rate, numbers.Number) \
-                    or not isinstance(val_now, numbers.Number) \
-                    or target == val_now:
+            if (
+                not isinstance(target, numbers.Number)
+                or not isinstance(rate, numbers.Number)
+                or not isinstance(val_now, numbers.Number)
+                or target == val_now
+            ):
                 # Do nothing if knob, rate or target are undefined
                 continue
 
             sign = (target - val_now) / abs(target - val_now)
 
-            val_nxt = val_now + sign*rate*(self.now - self.then)
+            val_nxt = val_now + sign * rate * (self.now - self.then)
 
-            if sign*val_now <= sign*target < sign*val_nxt:
+            if sign * val_now <= sign * target < sign * val_nxt:
                 self.knobs[knob].value = target
             else:
                 self.knobs[knob].value = val_nxt
 
-        self.then = state['Time']
+        self.then = state["Time"]
 
 
 class Timecourse(Routine):
     """
     Ramps the `knobs` linearly through a series of `values` at given `times`.
 
     The `times` and `values` should be 1D or 2D arrays of values (or keys for
     `values`); if 2D then the first dimension needs to have the same length as
     the `knobs` argument.
     """
 
-    def __init__(self,
-                 knobs: dict,
-                 times,
-                 values,
-                 **kwargs):
+    def __init__(self, knobs: dict, times, values, **kwargs):
         """
 
         :param times: (1D/2D array) array or list of times relative to
                       the start time
         :param values: (1D/2D array) array or list of values
         :param kwargs: keyword arguments for Routine
         """
@@ -282,45 +276,41 @@
         elif np.ndim(values) == 1:  # single list of values for all knobs
             self.values = [values] * len(self.knobs)
         else:
             self.values = values
 
         # Times and/or values can be stored in CSV files
         for i, (t_elem, v_elem) in enumerate(zip(self.times, self.values)):
-
-            if type(t_elem[0]) == str and '.csv' in t_elem[0]:
+            if type(t_elem[0]) == str and ".csv" in t_elem[0]:
                 df = pd.read_csv(t_elem[0])
-                self.times[i] = df['times'].values
+                self.times[i] = df["times"].values
 
-            if type(v_elem[0]) == str and '.csv' in v_elem[0]:
+            if type(v_elem[0]) == str and ".csv" in v_elem[0]:
                 df = pd.read_csv(v_elem[0])
-                self.values[i] = [recast(val) for val in df['values'].values]
+                self.values[i] = [recast(val) for val in df["values"].values]
 
         self.times = np.array(convert_time(self.times)).astype(float)
         self.values = np.array(self.values, dtype=object)
 
         # Infer start and end times from times argument, if not given
-        if 'start' not in kwargs:
+        if "start" not in kwargs:
             self.start = np.min(self.times)
 
-        if 'end' not in kwargs:
+        if "end" not in kwargs:
             self.end = np.max(self.times)
 
     @Routine.enabler
     def update(self, state):
-
         knobs_times_values = zip(self.knobs, self.times, self.values)
         for knob, times, values in knobs_times_values:
-
-            if np.min(times) > state['Time'] \
-                    or np.max(times) < state['Time']:
+            if np.min(times) > state["Time"] or np.max(times) < state["Time"]:
                 continue
 
-            j_last = np.argwhere(times <= state['Time']).flatten()[-1]
-            j_next = np.argwhere(times > state['Time']).flatten()[0]
+            j_last = np.argwhere(times <= state["Time"]).flatten()[-1]
+            j_next = np.argwhere(times > state["Time"]).flatten()[0]
 
             last_time = times[j_last]
             next_time = times[j_next]
 
             last_value = values[j_last]
             next_value = values[j_next]
 
@@ -330,79 +320,72 @@
                 last_value = state[last_value]
 
             last_is_number = isinstance(last_value, numbers.Number)
             next_is_number = isinstance(next_value, numbers.Number)
 
             if next_is_number and last_is_number:
                 # ramp linearly between numerical values
-                value = last_value + (next_value - last_value) \
-                        * (state['Time'] - last_time) / (next_time - last_time)
+                value = last_value + (next_value - last_value) * (
+                    state["Time"] - last_time
+                ) / (next_time - last_time)
             else:
                 # stay at last value until next time,
                 # when value variable will be evaluated
                 value = last_value
 
             self.knobs[knob].value = value
 
     def finish(self, state):
-
         # Upon routine completion, set each knob to its final value
         for knob, value in zip(self.knobs.values(), self.values[:, -1]):
             if knob._controller is None or knob._controller == self:
                 knob.value = value
 
 
 class Sequence(Routine):
     """
     Passes the `knobs` through a series of `values` regardless of time.
 
     The `values` should be a 1D or 2D array of keys/values; if 2D then the first
     dimension needs to have the same length as the `knobs` argument.
     """
 
-    def __init__(self,
-                 knobs: dict,
-                 values,
-                 **kwargs):
-
+    def __init__(self, knobs: dict, values, **kwargs):
         Routine.__init__(self, knobs, **kwargs)
 
         if np.ndim(values) == 0:  # single value or file path
             self.values = [[values]] * len(self.knobs)
         elif np.ndim(values) == 1:  # single list of values for all knobs
             self.values = [values] * len(self.knobs)
         else:
             self.values = values
 
         # Times and/or values can be stored in CSV files
         for i, v_elem in enumerate(self.values):
-            if type(v_elem[0]) == str and '.csv' in v_elem[0]:
+            if type(v_elem[0]) == str and ".csv" in v_elem[0]:
                 df = pd.read_csv(v_elem[0])
-                self.values[i] = [recast(val) for val in df['values'].values]
+                self.values[i] = [recast(val) for val in df["values"].values]
 
         self.values = np.array(self.values, dtype=object)
 
         self.iteration = 0
 
     @Routine.enabler
     def update(self, state):
-
         for knob, values in zip(self.knobs.values(), self.values):
-
             value = values[self.iteration]
 
             if isinstance(value, String):
                 value = state[value]
 
             knob.value = value
 
         self.iteration = (self.iteration + 1) % len(self.values[0])
 
     def finish(self, state):
-
         # Upon routine completion, set each knob to its final value
         for knob, value in zip(self.knobs.values(), self.values[:, -1]):
             if knob._controller is None or knob._controller == self:
                 knob.value = value
 
 
 class Minimization(Routine):
@@ -415,22 +398,17 @@
     indicating the maximum change per step for each knob; if not specified,
     defaults to a list of ones. The `T0` and `T1` argumnets are the initial and
     final temperatures; if not specified, defaults to T0 = 0.0 and T1 = 0.0.
     The `samples` argument determines the number of meter values to average
     together for each step.
     """
 
-    def __init__(self,
-                 knobs: dict,
-                 meter,
-                 max_deltas=None,
-                 T0=0.0, T1=0.0,
-                 samples=1,
-                 **kwargs):
-
+    def __init__(
+        self, knobs: dict, meter, max_deltas=None, T0=0.0, T1=0.0, samples=1, **kwargs
+    ):
         Routine.__init__(self, knobs, **kwargs)
 
         self.meter = meter
 
         if max_deltas:
             self.max_deltas = np.array([max_deltas]).flatten()
         else:
@@ -445,27 +423,28 @@
         self.best_meter = None
         self.best_knobs = [None for _ in self.knobs]
 
         self.revert = False  # going back?
 
     @Routine.enabler
     def update(self, state):
-
         # Take no action if knobs values are undefined
-        if None in [state[knob] for knob in self.knobs] \
-                or np.nan in [state[knob] for knob in self.knobs]:
+        if None in [state[knob] for knob in self.knobs] or np.nan in [
+            state[knob] for knob in self.knobs
+        ]:
             return
 
         if not self.prepped:
             self.prep(state)
             self.prepped = True
 
         # Update temperature
-        self.T = self.T0 + (self.T1 - self.T0) \
-                 * (state['Time'] - self.start) / (self.end - self.start)
+        self.T = self.T0 + (self.T1 - self.T0) * (state["Time"] - self.start) / (
+            self.end - self.start
+        )
 
         # Get meter values
         meter_value = state[self.meter]
 
         # Check for valid new meter value
         if meter_value is not None and meter_value != np.nan:
             self.meter_values.append(meter_value)
@@ -474,40 +453,37 @@
 
         # Check if enough samples have been measured
         if len(self.meter_values) <= self.samples:
             return
 
         # Check if found (or returned to) minimum
         if self.better(np.mean(self.meter_values)) or self.revert:
-
             # Record this new (or past) optimal state
             self.best_meter = np.mean(self.meter_values)
             self.best_knobs = [state[knob] for knob in self.knobs]
 
             # Generate and apply new knob settings
-            new_knobs = self.best_knobs \
-                        + self.max_deltas \
-                        * (2 * np.random.rand(len(self.knobs)) - 1)
+            new_knobs = self.best_knobs + self.max_deltas * (
+                2 * np.random.rand(len(self.knobs)) - 1
+            )
 
             for knob, new_value in zip(self.knobs.values(), new_knobs):
                 knob.value = new_value
 
             self.meter_values = []
             self.revert = False
 
         else:
-
             for knob, best_val in zip(self.knobs.values(), self.best_knobs):
                 knob.value = best_val
 
             self.meter_values = []
             self.revert = True
 
     def better(self, meter_value):
-
         if meter_value is None or meter_value == np.nan:
             return False
 
         if self.best_meter is None or self.best_meter == np.nan:
             return False
 
         change = meter_value - self.best_meter
@@ -515,34 +491,31 @@
         if self.T > 0:
             _rand = np.random.rand()
             return (change < 0) or (np.exp(-change / self.T) > _rand)
         else:
             return change < 0
 
     def prep(self, state):
-
         self.best_knobs = [state[knob] for knob in self.knobs]
         self.best_meter = state[self.meter]
 
     def finish(self, state):
-
         for knob, best_val in zip(self.knobs.values(), self.best_knobs):
             knob.value = best_val
 
 
 class Maximization(Minimization):
     """
     Maximize a `meter`/expression influenced by the set of knobs;
     otherwise, works the same way as Minimize.
     """
 
     best_meter = -np.inf
 
     def better(self, meter_value):
-
         if meter_value is None or meter_value == np.nan:
             return False
 
         if self.best_meter is None or self.best_meter == np.nan:
             return False
 
         change = meter_value - self.best_meter
@@ -563,15 +536,14 @@
     Clients can also read the values of any variables of the controlling
     experiment, via the `state` argument of the `update` method.
     """
 
     assert_control = False
 
     def __init__(self, knobs: dict = None, **kwargs):
-
         if knobs is None:
             knobs = {}
 
         Routine.__init__(self, knobs, **kwargs)
 
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
@@ -583,46 +555,40 @@
         self.clients_queue = queue.Queue(1)
         self.clients_queue.put({})
 
         self.running = True
 
         self.state = {}
 
-        self.acc_conn_thread = threading.Thread(
-            target=self.accept_connections
-        )
+        self.acc_conn_thread = threading.Thread(target=self.accept_connections)
 
         self.acc_conn_thread.start()
 
-        self.proc_requ_thread = threading.Thread(
-            target=self.process_requests
-        )
+        self.proc_requ_thread = threading.Thread(target=self.process_requests)
 
         self.proc_requ_thread.start()
 
     def terminate(self):
-
         # Kill client handling threads
         self.running = False
         self.acc_conn_thread.join()
         self.proc_requ_thread.join()
 
     def accept_connections(self):
         while self.running:
-
             try:
                 (client, address) = self.socket.accept()
 
                 clients = self.clients_queue.get()
 
                 clients[address] = client
 
                 self.clients_queue.put(clients)
 
-                print(f'Client at {address} has connected')
+                print(f"Client at {address} has connected")
 
             except socket.timeout:
                 pass
 
             time.sleep(0.1)
 
         # Close sockets
@@ -631,123 +597,109 @@
         except OSError:  # socket was not connected
             pass
         self.socket.close()
 
         clients = self.clients_queue.get()
 
         for address, client in clients.items():
-
             try:
                 client.shutdown(socket.SHUT_RDWR)
                 client.close()
             except ConnectionError:
                 pass
 
         # Return empty clients dict to queue so process_requests can exit
         self.clients_queue.put({})
 
     def process_requests(self):
         while self.running:
-
             clients = self.clients_queue.get()
 
             # Purge disconnected clients
             clients = {
-                address: client for address, client in clients.items()
+                address: client
+                for address, client in clients.items()
                 if client is not None
             }
 
             for address, client in clients.items():
-
                 outgoing_message = None
 
                 try:
                     request = read_from_socket(client, chunk_size=1)
                 except ConnectionError:
                     clients[address] = None
                     continue
 
                 if client and request:
+                    alias = " ".join(request.split(" ")[:-1])
+                    value = request.split(" ")[-1]
 
-                    alias = ' '.join(request.split(' ')[:-1])
-                    value = request.split(' ')[-1]
-
-                    if alias not in self.knobs \
-                            and alias not in self.state:
+                    if alias not in self.knobs and alias not in self.state:
+                        outgoing_message = f"Error: invalid alias"
 
-                        outgoing_message = f'Error: invalid alias'
-
-                    elif value == 'settable?':
-
-                        settable = (alias in self.knobs) \
-                                   and self.knobs[alias].settable
+                    elif value == "settable?":
+                        settable = (alias in self.knobs) and self.knobs[alias].settable
 
                         if settable:
-                            outgoing_message = f'{alias} settable'
+                            outgoing_message = f"{alias} settable"
                         elif alias in self.state:
-                            outgoing_message = f'{alias} read-only'
+                            outgoing_message = f"{alias} read-only"
                         else:
-                            outgoing_message = f'{alias} undefined'
-
-                    elif value == 'type?':
+                            outgoing_message = f"{alias} undefined"
 
+                    elif value == "type?":
                         if alias in self.knobs:
                             _type = self.knobs[alias].type
                         elif alias in self.state:
-
                             _type = None
                             for supported_type in supported_types.values():
                                 value = self.state[alias]
                                 if isinstance(value, supported_type):
                                     _type = supported_type
 
                         else:
                             _type = None
 
-                        outgoing_message = f'{alias} {_type}'
-
-                    elif value == '?':  # Query of value
+                        outgoing_message = f"{alias} {_type}"
 
+                    elif value == "?":  # Query of value
                         if alias in self.knobs:
                             _value = self.knobs[alias].value
                         elif alias in self.state:
                             _value = self.state[alias]
                         else:
                             _value = None
 
-                        outgoing_message = f'{alias} {_value}'
+                        outgoing_message = f"{alias} {_value}"
 
                     else:  # Setting a value
-
                         knob_exists = alias in self.knobs
 
-                        is_free = not getattr(
-                            self.knobs[alias], '_controller', None
-                        )
+                        is_free = not getattr(self.knobs[alias], "_controller", None)
 
                         if knob_exists and is_free:
-
                             knob = self.knobs[alias]
 
                             knob.value = recast(value, to=knob.type)
 
-                            outgoing_message = f'{alias} {knob.value}'
+                            outgoing_message = f"{alias} {knob.value}"
 
                         else:
-                            outgoing_message = f'Error: cannot set {alias}'
+                            outgoing_message = f"Error: cannot set {alias}"
 
                 # Send outgoing message
                 if outgoing_message is not None:
                     write_to_socket(client, outgoing_message)
 
                 # Remove clients with problematic connections
                 exceptional = client in select.select([], [], [client], 0)[2]
 
                 if exceptional:
-                    print(f'Client at {address} has a connection issue')
+                    print(f"Client at {address} has a connection issue")
                     clients[address] = None
 
             self.clients_queue.put(clients)
 
             time.sleep(0.01)
 
     @Routine.enabler
@@ -781,70 +733,65 @@
     any metadata (i.e. data type). Note that the that `state` of an instance of
     `Experiment` has `Time` as its first entry.
     """
 
     assert_control = False
 
     def __init__(self, knobs: dict = None, meters=None, **kwargs):
-
         if knobs is None:
             knobs = {}
 
         Routine.__init__(self, knobs, **kwargs)
 
         self.meters = meters
 
         self.state = None  # set by update method
 
         # Check for PyModbus installation
         try:
-            importlib.import_module('pymodbus')
+            importlib.import_module("pymodbus")
         except ModuleNotFoundError:
             raise ModuleNotFoundError(
-                'pymodbus must be installed to run a Modbus server'
+                "pymodbus must be installed to run a Modbus server"
             )
 
         # Import tools from pymodbus
-        datastore = importlib.import_module('.datastore', package='pymodbus')
-        device = importlib.import_module('.device', package='pymodbus')
-        payload = importlib.import_module('.payload', package='pymodbus')
+        datastore = importlib.import_module(".datastore", package="pymodbus")
+        device = importlib.import_module(".device", package="pymodbus")
+        payload = importlib.import_module(".payload", package="pymodbus")
 
         self._builder_cls = payload.BinaryPayloadBuilder
         self._decoder_cls = payload.BinaryPayloadDecoder
 
         DataBlock = datastore.ModbusSequentialDataBlock
 
         # Set up a PyModbus TCP Server
         datastore.ModbusSlaveContext.setValues = self.setValues_decorator(
             datastore.ModbusSlaveContext.setValues
         )
 
         self.slave = datastore.ModbusSlaveContext(
-                ir=DataBlock.create(),
-                hr=DataBlock.create()
-            )
-
-        self.context = datastore.ModbusServerContext(
-            slaves=self.slave,
-            single=True
+            ir=DataBlock.create(), hr=DataBlock.create()
         )
 
+        self.context = datastore.ModbusServerContext(slaves=self.slave, single=True)
+
         self.identity = device.ModbusDeviceIdentification(
             info_name={
                 "VendorName": "Empyric",
                 "VendorUrl": "https://github.com/dmerthe/empyric",
                 "ProductName": "Modbus Server",
                 "ModelName": "Modbus Server",
             }
         )
 
         # Run server
         self.server = None  # assigned in _run_async_server
-        self.ip_address = kwargs.get('address', get_ip_address())
-        self.port = kwargs.get('port', 502)
+        self.ip_address = kwargs.get("address", get_ip_address())
+        self.port = kwargs.get("port", 502)
 
         self.server_thread = threading.Thread(
             target=asyncio.run, args=(self._run_async_server(),)
         )
 
         self.server_thread.start()
 
@@ -863,82 +810,75 @@
             else:
                 # update variables according to the request
 
                 fc_as_hex, address, values = args
 
                 if fc_as_hex != 16:
                     print(
-                        f'Warning: an attempt was made to write to a readonly '
-                        f'register at address {address}'
+                        f"Warning: an attempt was made to write to a readonly "
+                        f"register at address {address}"
                     )
                 else:
-
                     if self.knobs:
-
                         variable = list(self.knobs.values())[address // 5]
 
-                        controller = getattr(variable, '_controller', None)
+                        controller = getattr(variable, "_controller", None)
 
                         if controller:
-
                             name = list(self.knobs.keys())[address // 5]
 
                             print(
-                                f'Warning: an attempt was made to set {name}, '
-                                'but it is currently controlled by '
-                                f'{controller}.'
+                                f"Warning: an attempt was made to set {name}, "
+                                "but it is currently controlled by "
+                                f"{controller}."
                             )
                             return
 
-                        decoder = self._decoder_cls.fromRegisters(
-                            values, byteorder='>'
-                        )
+                        decoder = self._decoder_cls.fromRegisters(values, byteorder=">")
 
                         if issubclass(variable._type, Boolean):
                             variable.value = decoder.decode_64bit_uint()
                         elif issubclass(variable._type, Toggle):
                             int_value = decoder.decode_64bit_uint()
                             variable.value = ON if int_value == 1 else OFF
                         elif issubclass(variable._type, Integer):
                             variable.value = decoder.decode_64bit_int()
                         elif issubclass(variable._type, Float):
                             variable.value = decoder.decode_64bit_float()
 
         return wrapped_method
 
     async def _update_registers(self):
-
         if self.state is None:  # do nothing if state is undefined
             await asyncio.sleep(0.1)
             asyncio.create_task(self._update_registers())
             return
 
         # Store readwrite variable values in holding registers (fc = 3)
-        builder = self._builder_cls(byteorder='>')
+        builder = self._builder_cls(byteorder=">")
 
         for i, (name, variable) in enumerate(self.knobs.items()):
-
             value = variable._value
 
             # encode the value into the 4 registers
             if value is None or variable.type is None:
-                builder.add_64bit_float(float('nan'))
+                builder.add_64bit_float(float("nan"))
             elif issubclass(variable.type, Boolean):
                 builder.add_64bit_uint(value)
             elif issubclass(variable.type, Toggle):
                 builder.add_64bit_uint(int(value in Toggle.on_values))
             elif issubclass(variable.type, Integer):
                 builder.add_64bit_int(value)
             elif issubclass(variable.type, Float):
                 builder.add_64bit_float(value)
             else:
                 raise ValueError(
-                    f'unable to update modbus server registers from value '
-                    f'{value} of variable {name} with data type '
-                    f'{variable.type}'
+                    f"unable to update modbus server registers from value "
+                    f"{value} of variable {name} with data type "
+                    f"{variable.type}"
                 )
 
             # encode the meta data
             meta_reg_val = {
                 Boolean: 0,
                 Toggle: 1,
                 Integer: 2,
@@ -957,65 +897,56 @@
 
         if self.meters:
             selection = self.state[self.meters]
         else:
             selection = self.state
 
         for i, (name, value) in enumerate(selection.items()):
-
             _type = None
             for supported_type in supported_types.values():
                 if isinstance(value, supported_type):
                     _type = supported_type
 
             # encode the value into the 4 registers
             if value is None or _type is None:
-                builder.add_64bit_float(float('nan'))
+                builder.add_64bit_float(float("nan"))
             elif _type == Boolean:
                 builder.add_64bit_uint(value)
             elif _type == Toggle:
                 builder.add_64bit_uint(int(value in Toggle.on_values))
             elif _type == Integer:
                 builder.add_64bit_int(value)
             elif _type == Float:
                 builder.add_64bit_float(value)
             else:
                 raise ValueError(
-                    f'unable to update modbus server registers from value '
-                    f'{value} of variable {name} with data type '
-                    f'{_type}'
+                    f"unable to update modbus server registers from value "
+                    f"{value} of variable {name} with data type "
+                    f"{_type}"
                 )
 
             # encode the meta data
-            type_int = {
-                Boolean: 0,
-                Toggle: 1,
-                Integer: 2,
-                Float: 3
-            }.get(_type, -1)
+            type_int = {Boolean: 0, Toggle: 1, Integer: 2, Float: 3}.get(_type, -1)
 
             builder.add_16bit_int(type_int)
 
         # from_vars kwarg added with setValues_decorator above
         self.slave.setValues(4, 0, builder.to_registers(), from_vars=True)
 
         await asyncio.sleep(0.1)
 
         asyncio.create_task(self._update_registers())
 
     async def _run_async_server(self):
-
         asyncio.create_task(self._update_registers())
 
-        server = importlib.import_module('.server', package='pymodbus')
+        server = importlib.import_module(".server", package="pymodbus")
 
         self.server = server.ModbusTcpServer(
-            self.context,
-            identity=self.identity,
-            address=(self.ip_address, self.port)
+            self.context, identity=self.identity, address=(self.ip_address, self.port)
         )
 
         try:
             await self.server.serve_forever()
         except asyncio.exceptions.CancelledError:
             # Server shutdown cancels the _update_registers task
             pass
@@ -1024,9 +955,12 @@
     def update(self, state):
         self.state = state
 
     def terminate(self):
         asyncio.run(self.server.shutdown())
 
 
-supported = {key: value for key, value in vars().items()
-             if type(value) is type and issubclass(value, Routine)}
+supported = {
+    key: value
+    for key, value in vars().items()
+    if type(value) is type and issubclass(value, Routine)
+}
```

### Comparing `empyric-0.2.0/empyric/runcard_schema.yaml` & `empyric-0.2.3/empyric/runcard_schema.yaml`

 * *Files identical despite different names*

### Comparing `empyric-0.2.0/empyric/tests/henon_runcard_example.yaml` & `empyric-0.2.3/empyric/tests/henon_runcard_example.yaml`

 * *Files identical despite different names*

### Comparing `empyric-0.2.0/empyric/tests/test_adapter.py` & `empyric-0.2.3/empyric/tests/test_adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 # Tests for adapters
 
 import sys
 import importlib
 
 
 def test_serial():
-
-    Serial = importlib.import_module('empyric.adapters').Serial
+    Serial = importlib.import_module("empyric.adapters").Serial
 
     assert Serial.lib is not None
 
 
 def test_gpib():
-
-    GPIB = importlib.import_module('empyric.adapters').GPIB
+    GPIB = importlib.import_module("empyric.adapters").GPIB
 
     assert GPIB.lib is not None
 
 
 def test_usb():
-
-    USB = importlib.import_module('empyric.adapters').USB
+    USB = importlib.import_module("empyric.adapters").USB
 
     assert USB.lib is not None
 
 
 def test_modbus():
-
-    Modbus = importlib.import_module('empyric.adapters').Modbus
+    Modbus = importlib.import_module("empyric.adapters").Modbus
 
     assert Modbus.lib is not None
 
 
 def test_phidget():
-
-    Phidget = importlib.import_module('empyric.adapters').Phidget
+    Phidget = importlib.import_module("empyric.adapters").Phidget
 
     assert Phidget.lib is not None
```

### Comparing `empyric-0.2.0/empyric/tests/test_experiment.py` & `empyric-0.2.3/empyric/tests/test_experiment.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,71 +14,70 @@
     Test experiment.Experiment
     """
 
     os.chdir(str(tmp_path))
 
     echo = Echo()
 
-    echo_in = Knob(instrument=echo, knob='input')
-    echo_out = Meter(instrument=echo, meter='output')
+    echo_in = Knob(instrument=echo, knob="input")
+    echo_out = Meter(instrument=echo, meter="output")
 
-    variables = {'Echo In': echo_in, 'Echo Out': echo_out}
+    variables = {"Echo In": echo_in, "Echo Out": echo_out}
 
     step_up_routine = Timecourse(
-        knobs={'Echo In': echo_in},
+        knobs={"Echo In": echo_in},
         times=[0.1, 0.2, 0.3, 0.4, 0.5],
-        values=[10, 20, 30, 40, 50]
+        values=[10, 20, 30, 40, 50],
     )
 
-    routines = {'Step Up Timecourse': step_up_routine, }
+    routines = {
+        "Step Up Timecourse": step_up_routine,
+    }
 
-    experiment = Experiment(variables, routines=routines, end='with routines')
+    experiment = Experiment(variables, routines=routines, end="with routines")
 
     for _ in experiment:
         time.sleep(0.001)
 
     # check that experiment ended on time
-    assert round(experiment.state['Time'], 1) == 0.5
+    assert round(experiment.state["Time"], 1) == 0.5
     assert round(echo_out.value) == 50
 
     # check data saving
     experiment.save()
 
-    assert any(glob.glob('data_*.csv'))
+    assert any(glob.glob("data_*.csv"))
 
 
 # Use Henon runcard example for testing
 tests_dir = os.path.dirname(__file__)
 
 test_runcard_path = os.path.abspath(
-    os.path.join(
-        tests_dir, 'henon_runcard_example.yaml'
-    )
+    os.path.join(tests_dir, "henon_runcard_example.yaml")
 )
 
-def test_runcard_validation():
 
+def test_runcard_validation():
     try:
         assert os.path.isfile(test_runcard_path)
     except AssertionError:
         raise AssertionError(
             "test runcard 'henon_runcard_example.yaml' was not found in "
             "installed package. This is normally configured by pip running "
             "setup.py. For a proper install, please use pip or similar."
         )
 
     assert validate_runcard(test_runcard_path)
 
 
 def test_manager(tmp_path):
-
     manager = Manager(test_runcard_path)
 
     # Check that the runcard loaded
-    assert manager.description['name'] == 'Henon Map Experiment'
+    assert manager.description["name"] == "Henon Map Experiment"
 
     # Run a short version of the Henon Map example experiment
     manager.experiment.end = 10
     manager.followup = None
 
     manager.run(directory=tmp_path)
```

### Comparing `empyric-0.2.0/empyric/tests/test_variable.py` & `empyric-0.2.3/empyric/tests/test_variable.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 def test_variable():
     """
     Test experiment.Variable
     """
 
     clock = Clock()
 
-    test_knob = Knob(instrument=clock, knob='state')
+    test_knob = Knob(instrument=clock, knob="state")
 
-    test_meter = Meter(instrument=clock, meter='time')
+    test_meter = Meter(instrument=clock, meter="time")
 
     test_parameter = Parameter(parameter=5)
 
     test_expression = Expression(
-        expression='time + offset',
-        definitions={'time': test_meter, 'offset': test_parameter}
+        expression="time + offset",
+        definitions={"time": test_meter, "offset": test_parameter},
     )
 
-    assert test_knob.value == 'STOP'
+    assert test_knob.value == "STOP"
     assert test_meter.value == 0
     assert test_parameter.value == 5
     assert test_expression.value == 5
```

### Comparing `empyric-0.2.0/empyric/tools.py` & `empyric-0.2.3/empyric/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,38 +23,44 @@
         return [convert_time(t) for t in time_value]
 
     if isinstance(time_value, numbers.Number):
         return time_value
     elif isinstance(time_value, str):
         # times can be specified in the runcard with units, such as minutes,
         # hours or days, e.g. "6 hours"
-        time_parts = time_value.split(' ')
+        time_parts = time_value.split(" ")
 
         if len(time_parts) == 1:
             return float(time_parts[0])
         elif len(time_parts) == 2:
             value, unit = time_parts
             value = float(value)
-            return value * {
-                'seconds': 1, 'second': 1,
-                'minutes': 60, 'minute': 60,
-                'hours': 3600, 'hour': 3600,
-                'days': 86400, 'day': 86400
-            }[unit]
+            return (
+                value
+                * {
+                    "seconds": 1,
+                    "second": 1,
+                    "minutes": 60,
+                    "minute": 60,
+                    "hours": 3600,
+                    "hour": 3600,
+                    "days": 86400,
+                    "day": 86400,
+                }[unit]
+            )
         else:
-            raise ValueError(f'Unrecognized time format for {time_value}!')
+            raise ValueError(f"Unrecognized time format for {time_value}!")
 
 
 class Clock:
     """
     Clock for keeping time in an experiment; works like a standard stopwatch
     """
 
     def __init__(self):
-
         self.start_time = self.stop_time = time.time()  # initially stopped
         self.stoppage = 0  # total time during which the clock has been stopped
 
     def start(self):
         if self.stop_time:
             self.stoppage += time.time() - self.stop_time
             self.stop_time = False
@@ -95,15 +101,15 @@
         nearest = np.argwhere(diffs == np.min(diffs)).flatten()
 
     if len(nearest) > 0:
         return allowed[nearest[0]]
 
 
 # Tools for handling sockets
-def get_ip_address(remote_ip='8.8.8.8', remote_port=80):
+def get_ip_address(remote_ip="8.8.8.8", remote_port=80):
     """
     Connect to a server to resolve IP address; defaults to Google's DNS server
     if `remote_ip` and `remote_port` are not specified
     """
 
     with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as tst_sock:
         tst_sock.connect((remote_ip, remote_port))
@@ -125,21 +131,22 @@
             _socket.bind((ip_address, port))
             bound = True
             break
         except OSError:
             pass
 
     if not bound:
-        raise IOError(f'unable to bind socket at {ip_address} to any port!')
+        raise IOError(f"unable to bind socket at {ip_address} to any port!")
 
     return ip_address, port
 
 
-def read_from_socket(_socket, nbytes=None, termination='\r', timeout=1,
-                     decode=True, chunk_size=4096):
+def read_from_socket(
+    _socket, nbytes=None, termination="\r", timeout=1, decode=True, chunk_size=4096
+):
     """
     Read from a socket, with some effort taken to get the whole message.
 
     :param _socket: (socket.Socket) socket to read from.
     :param nbytes: (int) number of bytes to read; defaults to infinite.
     :param termination: (str/bytes/callable) if str or bytes, expected message
                         termination character(s); if callable, a function that
@@ -168,55 +175,51 @@
     _socket.settimeout(timeout)
 
     if nbytes is None:
         nbytes = np.inf
 
         if termination is None:
             raise ValueError(
-                'nbytes must be a non-negative integer if termination is None'
+                "nbytes must be a non-negative integer if termination is None"
             )
 
     null_responses = 0
     max_nulls = 3
 
     if type(termination) == str:
         termination = termination.encode()
 
     def is_terminated(message):
-
         if isinstance(termination, bytes):
             return termination in message
         elif callable(termination):
             return termination(message)
         else:
             return False
 
-    message = b''
+    message = b""
 
     while len(message) < nbytes and null_responses < max_nulls:
-
-        part = b''
+        part = b""
 
         remaining_bytes = nbytes - len(message)
 
         try:
-
             if remaining_bytes < chunk_size:
                 part = _socket.recv(remaining_bytes)
             else:
                 part = _socket.recv(chunk_size)
 
         except ConnectionResetError as err:
-            print(f'Warning: {err}')
+            print(f"Warning: {err}")
             break
         except socket.timeout:
             pass
 
         if len(part) > 0:
-
             message = message + part
 
             if is_terminated(message):
                 break
 
         else:
             null_responses += 1
@@ -225,15 +228,15 @@
 
     if decode:
         return message.decode().strip()
     else:
         return message
 
 
-def write_to_socket(_socket, message, termination='\r', timeout=1):
+def write_to_socket(_socket, message, termination="\r", timeout=1):
     """
     Write a message to a socket, with care taken to get the whole message
     transmitted.
 
     :param _socket: (socket.Socket) socket to write to.
     :param message: (str) message to send.
     :param termination: (str/bytes) expected message termination character(s).
@@ -254,21 +257,18 @@
 
     failures = 0
     max_failures = 3
 
     total_sent = 0
 
     while total_sent < msg_len and failures < max_failures:
-
         sent = _socket.send(bytes_message[total_sent:])
 
         if sent == 0:
             failures += 1
 
         total_sent = total_sent + sent
 
     if total_sent < msg_len:
-        raise IOError(
-            f'Socket connection to {_socket.getsockname()} is broken!'
-        )
+        raise IOError(f"Socket connection to {_socket.getsockname()} is broken!")
 
     return total_sent
```

### Comparing `empyric-0.2.0/empyric/types.py` & `empyric-0.2.3/empyric/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,130 +1,135 @@
 # Standardization of data types
 import abc
 import os
 import re
 from abc import ABC
 import pandas as pd
 import numpy as np
-from typing import Any
+from typing import Any, Union
 
 
 class Type(ABC):
     """Abstract base class for all supported data types"""
+
     pass
 
 
 class Boolean(Type):
     """Abstract base class for all boolean types; `bool` and `np.bool_` are
     subclasses"""
+
     pass
 
 
 Boolean.register(bool)
 Boolean.register(np.bool_)
 
 
 class Toggle(Type):
     """
     Convenience class for handling toggle variables, which are either off or on.
     """
 
-    on_values = [True, 1, '1', 'ON', 'On', 'on']
-    off_values = [False, 0, '0', 'OFF', 'Off', 'off']
-
-    def __init__(self, state: [str, bool, int, type]):
+    on_values = [True, 1, "1", "ON", "On", "on"]
+    off_values = [False, 0, "0", "OFF", "Off", "off"]
 
-        if hasattr(state, 'on'):
+    def __init__(self, state: Union[str, bool, int, type]):
+        if hasattr(state, "on"):
             self.on = state.on
         elif state in self.on_values:
             self.on = True
         elif state in self.off_values:
             self.on = False
         else:
-            raise ValueError(
-                f'toggle was initialized with invalid state {state}'
-            )
+            raise ValueError(f"toggle was initialized with invalid state {state}")
 
     def __bool__(self):
         return True if self.on else False
 
     def __int__(self):
         return 1 if self.on else 0
 
     def __str__(self):
-        return 'ON' if self.on else 'OFF'
+        return "ON" if self.on else "OFF"
 
     def __eq__(self, other):
-
-        if hasattr(other, 'on'):
+        if hasattr(other, "on"):
             return self.on == other.on
         else:
             if self.on and other in self.on_values:
                 return True
             elif not self.on and other in self.off_values:
                 return True
             else:
                 return False
 
 
-ON = Toggle('ON')
-OFF = Toggle('OFF')
+ON = Toggle("ON")
+OFF = Toggle("OFF")
 
 
 class Integer(Type):
     """Abstract base class for all integer types; `int` and `np.integer` are
     subclasses"""
+
     pass
 
 
 Integer.register(int)
 Integer.register(np.integer)
 
 
 class Float(Type):
     """Abstract base class for all float types; `float` and `np.floating` are
     subclasses"""
+
     pass
 
 
 Float.register(float)
 Float.register(np.floating)
 
 
 class String(Type):
     """Abstract base class for all string types; `str` and `np.str_` are
     subclasses"""
+
     pass
 
 
 String.register(str)
 String.register(np.str_)
 
 
 class Array(Type):
     """
     Abstract base class for all array-like types, essentially any commonly
     used type that can be indexed; `list`, `tuple`, `numpy.ndarray`,
     `pandas.Series` and `pandas.Dataframe` are subclasses
     """
+
     pass
 
 
 Array.register(list)
 Array.register(tuple)
 Array.register(np.ndarray)
 Array.register(pd.Series)
 Array.register(pd.DataFrame)
 
 
-supported = {key: value for key, value in vars().items()
-             if type(value) is abc.ABCMeta and issubclass(value, Type)}
+supported = {
+    key: value
+    for key, value in vars().items()
+    if type(value) is abc.ABCMeta and issubclass(value, Type)
+}
 
 
-def recast(value: Any, to: type = Type) -> [Type, None]:
+def recast(value: Any, to: type = Type) -> Union[Type, None]:
     """
     Convert a value into the appropriate type for the information it contains.
 
     Booleans are converted into numpy booleans; integers are converted into
     64-bit numpy integers; floats are converted into 64-bit numpy floats.
 
     Array-like values are converted into the analogous numpy array.
@@ -142,15 +147,14 @@
     :param value: (Any) the value whose type needs converting
     :param to: (Type) optional keyword argument indicating which type to
                        convert to; default value is `Type` which indicates
                        that the type should be inferred based on the value.
     """
 
     if to != Type:
-
         if value is None:
             return None
 
         for dtype in np.array([to], dtype=object).flatten():
             try:
                 # recast to desired
                 if issubclass(dtype, Boolean):
@@ -164,53 +168,47 @@
                 elif issubclass(dtype, String):
                     return np.str_(value)
                 elif issubclass(dtype, Array) and np.ndim(value) > 0:
                     return np.array(value)
             except ValueError:
                 pass
 
-        print(
-            f'Warning: unable to recast value {value} to type {to}'
-        )
+        print(f"Warning: unable to recast value {value} to type {to}")
 
         return None
 
     else:
         # infer type
         if isinstance(value, Boolean):
             return np.bool_(value)
         elif isinstance(value, Toggle):
             return value
         elif isinstance(value, Integer):
             return np.int64(value)
         elif isinstance(value, Float):
             return np.float64(value)
         elif isinstance(value, String):
-
-            if value.lower() == 'true':
+            if value.lower() == "true":
                 return np.bool_(True)
-            elif value.lower() == 'false':
+            elif value.lower() == "false":
                 return np.bool_(False)
-            elif re.fullmatch('[0-9]+', value):  # integer
+            elif re.fullmatch("[0-9]+", value):  # integer
                 return np.int64(value)
-            elif re.fullmatch('[-+]?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)?', value):
+            elif re.fullmatch("[-+]?[0-9]*\.?[0-9]+([eE][-+]?[0-9]+)?", value):
                 # float
                 return float(value)
             elif value in (Toggle.on_values + Toggle.off_values):
                 return Toggle(value)
             elif os.path.isfile(value):  # path in the current working directory
                 return os.path.abspath(value)
-            elif os.path.isfile(os.path.join('..', value)):  # ... up one level
-                return os.path.abspath(os.path.join('..', value))
+            elif os.path.isfile(os.path.join("..", value)):  # ... up one level
+                return os.path.abspath(os.path.join("..", value))
             else:
                 return value  # must be an actual string
         if isinstance(value, Array):  # value is an array
             np_array = np.array(value)  # convert to numpy array
             rep_elem = np_array.flatten()[0]  # representative element
             return np_array.astype(type(recast(rep_elem)))
         else:
-
-            print(
-                f'Warning: unable to recast value {value} of type {type(value)}'
-            )
+            print(f"Warning: unable to recast value {value} of type {type(value)}")
 
             return None
```

### Comparing `empyric-0.2.0/empyric/variables.py` & `empyric-0.2.3/empyric/variables.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,20 +43,20 @@
     def value(self, value):
         # overwritten by child classes
         pass
 
     @staticmethod
     def setter_type_validator(setter):
         """Checks that set value is compatible with variable's type"""
+
         @wraps(setter)
         def wrapped_setter(self, value):
-
-            if not isinstance(value, Array) \
-                    and (value is None or value == float('nan')):
-
+            if not isinstance(value, Array) and (
+                value is None or value == float("nan")
+            ):
                 self._value = None
 
             elif self.type is not None:
                 setter(self, recast(value, to=self.type))
             else:
                 # if type is not explicitly defined upon construction,
                 # infer from first set value
@@ -69,22 +69,22 @@
                         setter(self, recasted_value)
 
         return wrapped_setter
 
     @staticmethod
     def getter_type_validator(getter):
         """Checks that get value is compatible with variable's type"""
+
         @wraps(getter)
         def wrapped_getter(self):
-
             value = getter(self)
 
-            if not isinstance(value, Array) \
-                    and (value is None or value == float('nan')):
-
+            if not isinstance(value, Array) and (
+                value is None or value == float("nan")
+            ):
                 self._value = None
 
             elif self.type is not None:
                 self._value = recast(value, to=self.type)
             else:
                 # if type is not explicitly defined upon construction,
                 # infer from first set value
@@ -110,29 +110,30 @@
     associated with.
 
     The `knob` argument is the label of the knob on the instrument.
     """
 
     _settable = True  #:
 
-    def __init__(self,
-                 instrument: Instrument,
-                 knob: str,
-                 lower_limit: numbers.Number = None,
-                 upper_limit: numbers.Number = None):
-
+    def __init__(
+        self,
+        instrument: Instrument,
+        knob: str,
+        lower_limit: numbers.Number = None,
+        upper_limit: numbers.Number = None,
+    ):
         self.instrument = instrument
         self.knob = knob  # name of the knob on instrument
         self.lower_limit = lower_limit
         self.upper_limit = upper_limit
 
         # infer type from type hint of first argument of set method
-        set_method = getattr(instrument, 'set_'+knob.replace(' ', '_'))
+        set_method = getattr(instrument, "set_" + knob.replace(" ", "_"))
         type_hints = typing.get_type_hints(set_method)
-        type_hints.pop('return', None)  # exclude return type hint
+        type_hints.pop("return", None)  # exclude return type hint
 
         if type_hints:
             arg_hints = list(type_hints)
             self._type = type_hints[arg_hints[0]]
 
         self._value = None
 
@@ -158,17 +159,15 @@
         if self.upper_limit and value > self.upper_limit:
             self.instrument.set(self.knob, self.upper_limit)
         elif self.lower_limit and value < self.lower_limit:
             self.instrument.set(self.knob, self.lower_limit)
         else:
             self.instrument.set(self.knob, value)
 
-        self._value = self.instrument.__getattribute__(
-            self.knob.replace(' ', '_')
-        )
+        self._value = self.instrument.__getattribute__(self.knob.replace(" ", "_"))
 
 
 class Meter(Variable):
     """
     Variable that is measured by an instrument, such as temperature.
 
     Some meters can be controlled directly or indirectly through
@@ -186,26 +185,25 @@
     variable evaluates to 1/True/On, the meter can be measured. Otherwise,
     attempts to measure the meter will have no effect (`None` is returned).
     """
 
     _settable = False  #:
 
     def __init__(self, instrument: Instrument, meter: str, gate=None):
-
         self.instrument = instrument
         self.meter = meter
 
         if gate and isinstance(gate, Variable):
             self.gate = gate
         else:
             self.gate = Parameter(ON)
 
         self._type = typing.get_type_hints(
-            getattr(instrument, 'measure_' + meter.replace(' ', '_'))
-        ).get('return', None)
+            getattr(instrument, "measure_" + meter.replace(" ", "_"))
+        ).get("return", None)
 
         self._value = None
 
     @property
     @Variable.getter_type_validator
     def value(self):
         """
@@ -236,65 +234,61 @@
     The `definitions` argument is a dictionary mapping symbols in the
     `expression` argument to variables.
     """
 
     _settable = False  #:
 
     _functions = {
-        'sqrt(': 'np.sqrt(',
-        'exp(': 'np.exp(',
-        'sin(': 'np.sin(',
-        'cos(': 'np.cos(',
-        'tan(': 'np.tan(',
-        'sum(': 'np.nansum(',
-        'mean(': 'np.nanmean(',
-        'rms(': 'np.nanstd(',
-        'std(': 'np.nanstd(',
-        'var(': 'np.nanvar(',
-        'diff(': 'np.diff(',
-        'max(': 'np.nanmax(',
-        'min(': 'np.nanmin('
+        "sqrt(": "np.sqrt(",
+        "exp(": "np.exp(",
+        "sin(": "np.sin(",
+        "cos(": "np.cos(",
+        "tan(": "np.tan(",
+        "sum(": "np.nansum(",
+        "mean(": "np.nanmean(",
+        "rms(": "np.nanstd(",
+        "std(": "np.nanstd(",
+        "var(": "np.nanvar(",
+        "diff(": "np.diff(",
+        "max(": "np.nanmax(",
+        "min(": "np.nanmin(",
     }
 
     def __init__(self, expression: str, definitions: dict = None):
-
         self.expression = expression
         self.definitions = definitions if definitions is not None else {}
 
     @property
     @Variable.getter_type_validator
     def value(self):
         """
         Value of the expression
         """
 
         expression = self.expression
 
         # carets represent exponents
-        expression = expression.replace('^', '**')
+        expression = expression.replace("^", "**")
 
         for symbol, variable in self.definitions.items():
-
-            expression = expression.replace(
-                symbol, f"({variable._value})"
-            )
+            expression = expression.replace(symbol, f"({variable._value})")
 
         for shorthand, longhand in self._functions.items():
             if shorthand in expression:
                 expression = expression.replace(shorthand, longhand)
 
         try:
-            if 'None' not in expression and 'nan' not in expression:
+            if "None" not in expression and "nan" not in expression:
                 self._value = eval(expression)
             else:
                 self._value = None
         except BaseException as err:
             print(
-                f'Unable to evaluate expression {self.expression} due to '
-                f'error: ', err
+                f"Unable to evaluate expression {self.expression} due to " f"error: ",
+                err,
             )
             self._value = None
 
         self.last_evaluation = time.time()
 
         return self._value
 
@@ -326,49 +320,49 @@
     the variable value is read from the holding registers (`readwrite`
     variables), otherwise the variable value is read from the input registers
     (`readonly` variables).
 
     """
 
     type_map = {
-        Toggle: '64bit_uint',
-        Boolean: '64bit_uint',
-        Integer: '64bit_int',
-        Float: '64bit_float'
+        Toggle: "64bit_uint",
+        Boolean: "64bit_uint",
+        Integer: "64bit_int",
+        Float: "64bit_float",
     }
 
-    def __init__(self,
-                 server: str,
-                 alias: [int, str],
-                 protocol: str = None,
-                 settable: bool = False  # needed for modbus protocol
-                 ):
-
+    def __init__(
+        self,
+        server: str,
+        alias: Union[int, str],
+        protocol: str = None,
+        settable: bool = False,  # needed for modbus protocol
+    ):
         self.server = server
         self.alias = alias
         self.protocol = protocol
 
-        if protocol == 'modbus':
+        if protocol == "modbus":
             self._client = instruments.ModbusClient(server)
             self._settable = settable
 
         else:
-            server_ip, server_port = server.split('::')
+            server_ip, server_port = server.split("::")
 
             self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
             self._socket.connect((server_ip, int(server_port)))
 
-            write_to_socket(self._socket, f'{self.alias} settable?')
+            write_to_socket(self._socket, f"{self.alias} settable?")
 
             response = read_from_socket(self._socket, timeout=60)
-            self._settable = response == f'{self.alias} settable'
+            self._settable = response == f"{self.alias} settable"
 
             # Get type
-            write_to_socket(self._socket, f'{self.alias} type?')
+            write_to_socket(self._socket, f"{self.alias} type?")
 
             response = read_from_socket(self._socket, timeout=60)
 
             if response is not None:
                 for _type in types.supported:
                     if str(_type) in response.split(alias)[-1]:
                         self._type = types.supported.get(_type, None)
@@ -378,113 +372,103 @@
     @property
     @Variable.getter_type_validator
     def value(self):
         """
         Value of the remote variable on a server
         """
 
-        if self.protocol == 'modbus':
-
+        if self.protocol == "modbus":
             fcode = 3 if self.settable else 4
 
-            type_int = self._client.read(
-                fcode, self.alias + 4, _type='16bit_int'
-            )
+            type_int = self._client.read(fcode, self.alias + 4, _type="16bit_int")
 
             _type = {
                 0: Boolean,
                 1: Toggle,
                 2: Integer,
                 3: Float,
             }.get(type_int, None)
 
             if _type is not None:
                 self._value = self._client.read(
-                    fcode, self.alias, count=4,
-                    _type=self.type_map[_type]
+                    fcode, self.alias, count=4, _type=self.type_map[_type]
                 )
 
         else:
-            write_to_socket(self._socket, f'{self.alias} ?')
+            write_to_socket(self._socket, f"{self.alias} ?")
 
             response = read_from_socket(self._socket, timeout=60)
 
             try:
-
                 if response is None:
                     self._value = None
-                elif 'Error' in response:
-                    raise RuntimeError(response.split('Error: ')[-1])
+                elif "Error" in response:
+                    raise RuntimeError(response.split("Error: ")[-1])
                 else:
-                    self._value = recast(response.split(' ')[-1])
+                    self._value = recast(response.split(" ")[-1])
 
             except BaseException as error:
                 print(
-                    f'Warning: unable to retrieve value of {self.alias} '
+                    f"Warning: unable to retrieve value of {self.alias} "
                     f'from server at {self.server}; got error "{error}"'
                 )
 
         return self._value
 
     @value.setter
     @Variable.setter_type_validator
     def value(self, value):
         """
         Set the value of a remote variable
         """
 
-        if self.protocol == 'modbus':
-
-            self._client.write(
-                16, self.alias, value, _type=self.type_map[self.type]
-            )
+        if self.protocol == "modbus":
+            self._client.write(16, self.alias, value, _type=self.type_map[self.type])
 
         else:
-            write_to_socket(self._socket, f'{self.alias} {value}')
+            write_to_socket(self._socket, f"{self.alias} {value}")
 
             check = read_from_socket(self._socket, timeout=60)
 
-            if check == '' or check is None:
+            if check == "" or check is None:
                 print(
-                    f'Warning: received no response from server at '
-                    f'{self.server} while trying to set {self.alias}'
+                    f"Warning: received no response from server at "
+                    f"{self.server} while trying to set {self.alias}"
                 )
-            elif 'Error' in check:
+            elif "Error" in check:
                 print(
                     f'Warning: got response "{check}" while trying to set '
-                    f'{self.alias} on server at {self.server}'
+                    f"{self.alias} on server at {self.server}"
                 )
             else:
                 try:
-
-                    check_value = recast(check.split(f'{self.alias} ')[1])
+                    check_value = recast(check.split(f"{self.alias} ")[1])
 
                     if value != check_value:
                         print(
-                            f'Warning: attempted to set {self.alias} on '
-                            f'server at {self.server} to {value} but '
-                            f'checked value is {check_value}'
+                            f"Warning: attempted to set {self.alias} on "
+                            f"server at {self.server} to {value} but "
+                            f"checked value is {check_value}"
                         )
 
                 except ValueError as val_err:
                     print(
-                        f'Warning: unable to check value while setting '
-                        f'{self.alias} on server at {self.server}; '
+                        f"Warning: unable to check value while setting "
+                        f"{self.alias} on server at {self.server}; "
                         f'got error "{val_err}"'
                     )
                 except IndexError as ind_err:
                     print(
-                        f'Warning: unable to check value while setting '
-                        f'{self.alias} on server at {self.server}; '
+                        f"Warning: unable to check value while setting "
+                        f"{self.alias} on server at {self.server}; "
                         f'got error "{ind_err}"'
                     )
 
     def __del__(self):
-
-        if self.protocol == 'modbus':
+        if self.protocol == "modbus":
             self._client.disconnect()
         else:
             self._socket.shutdown(socket.SHUT_RDWR)
             self._socket.close()
 
 
 class Parameter(Variable):
@@ -495,15 +479,14 @@
 
     The `parameter` argument is the given value of the parameter.
     """
 
     _settable = True  #:
 
     def __init__(self, parameter: Type):
-
         self.parameter = recast(parameter)
         self._value = parameter
 
     @property
     @Variable.getter_type_validator
     def value(self):
         """Value of the parameter"""
@@ -513,9 +496,12 @@
     @Variable.setter_type_validator
     def value(self, value):
         """Set the parameter value"""
         self.parameter = value
         self._value = value
 
 
-supported = {key: value for key, value in vars().items()
-             if type(value) is type and issubclass(value, Variable)}
+supported = {
+    key: value
+    for key, value in vars().items()
+    if type(value) is type and issubclass(value, Variable)
+}
```

### Comparing `empyric-0.2.0/pyproject.toml` & `empyric-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "empyric"
-version = "0.2.0"
+version = "0.2.3"
 description = "A package for experiment automation"
 authors = ["Daniel Merthe <dmerthe@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/dmerthe/empyric"
 packages = [
     { include = "empyric"},
 ]
```

### Comparing `empyric-0.2.0/PKG-INFO` & `empyric-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empyric
-Version: 0.2.0
+Version: 0.2.3
 Summary: A package for experiment automation
 Home-page: https://github.com/dmerthe/empyric
 Author: Daniel Merthe
 Author-email: dmerthe@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,71 +21,71 @@
 Description-Content-Type: text/markdown
 
 # Empyric 
 ## A Python Library for Experiment Automation
 
 For more details, [read the docs](https://empyric.readthedocs.io/en/latest/).
 
-Empyric, at its most basic level, is an easy to use Python interface for communication with and controlling scientific instruments, such as digital multimeters, digital oscilloscopes, and power supplies. On top of that is a general purpose experiment-building architecture, which allows the user to combine process control, measurements and data plotting in a highly customizable fashion, using a straightforward "runcard" formalism, which additionally serves the purpose of experiment documentation.
+Empyric, at its most basic level, is an easy-to-use Python interface for communication with and controlling laboratory instruments, such as digital multimeters, oscilloscopes, and power supplies. On top of that is a general purpose experiment-building architecture, which allows the user to combine process control, measurements and data plotting in a highly customizable fashion, using a straightforward "runcard" formalism, which additionally serves the purpose of experiment documentation.
 
-The preferred method of installing Empyric is via pip:
+Empyric can be installed with pip:
 ```commandline
 pip install empyric
 ```
 
 ### Instruments and Adapters
 
 Empyric contains a number of *instruments* with various associated methods of communication, such as serial or GPIB. For example, to remotely control a Keithley 2400 Sourcemeter from your PC, simply import the `Keithley2400` object from the library and instantiate it with its GPIB address:
 
 ```
 from empyric.instruments import Keithley2400
 
 keithley2400 = Keithley2400(1)  # if GPIB address is 1
 
-kiethley2400.set('voltage', 10)
-current = keithley2400.measure('current')
+kiethley2400.set_voltage(10)  # sets output voltage to 10 volts
+current = keithley2400.measure_current()  # measures current in amperes
 ```
 
 Communication with instruments is facilitated through Empyric's library of *adapters*. If you have an instrument that is not in the Empyric library but which uses one of the more common communication protocols (Serial, GPIB, USBTMC, Modbus, etc.), you can still make use of Empyric's adapters, which automatically manage many of the underlying details of the communication backends:
 
 ```
 from empyric.instruments import Instrument
 from empyric.adapters import Modbus
 
 class MyInstrument(Instrument):
 	"""
 	Basic template of an instrument object in Empyric
 	"""
 
-	name = 'My Instrument'
+	name = 'MyInstrument'
 	
 	supported_adapters = ((Modbus, {'baud_rate':115200}),)
 	
-	knobs = ('knob',)
-	meters = ('meter',)
+	knobs = ('some knob',)
+	meters = ('some meter',)
 	
-	def set_knob(self, value):
-		# ... set your knob
+	def set_some_knob(self, value):
+		# set your knob
 	
-	def measure_meter(self):
-		# ... measure your meter
+	def measure_some_meter(self):
+		# measure your meter
 	
 instrument = MyInstrument('COM5::1')  # connect to your instrument
 
-meter_value = instrument.measure_meter()  # take a measurement
+some_meter_value = instrument.measure_some_meter()  # take a measurement
 
 ```
 
 ### Experiments
 
 The real purpose of Empyric is to simplify and standardize construction of an experiment, and automate its execution. The two main elements of an experiment are its *variables* which are controlled and/or measured by your instruments, and *routines* which are the various processes that you run on your controllable variables.
 
-*Variables* come in four flavors: knobs, meters, expressions and parameters. A knob is a variable that you can directly control through an instrument, such as voltage from a power supply. A meter is a variable that you directly measure through an instrument, such as temperature from a thermocouple. In some cases, a meter can be controlled indirectly through a feedback loop. For example, PID temperature controllers provide a temperature knob (the setpoint) as well as a temperature meter (the actual temperature measured with a thermocouple or RTD). An expression is a variable that is evaluated in terms of other experiment variables, such as the power delivered by a power supply being the product of the voltage knob value and the current meter value. A parameter is a user-defined value that is relevant to the experiment, such as a unit conversion factor, a variable setpoint (e.g. used in a routine) or a quantity that must be manually logged.
+*Variables* come in five flavors: knobs, meters, expressions, parameters and remotes. A knob is a variable that you can directly control through an instrument, such as voltage from a power supply. A meter is a variable that you directly measure through an instrument, such as temperature from a thermocouple. In some cases, a meter can be controlled indirectly through a feedback loop. For example, PID temperature controllers provide a temperature knob (the setpoint) as well as a temperature meter (the actual temperature measured with a thermocouple or RTD). An expression is a variable that is evaluated in terms of other experiment variables, such as the power delivered by a power supply being the product of the voltage knob value and the current meter value. A parameter is a user-defined value that is relevant to the experiment, such as a unit conversion factor, a variable setpoint (e.g. used in a routine) or a quantity that must be manually logged. A remote variable is a variable defined in another experiment with a server routine running, that can be read or controlled remotely. A variable's value can be read and set through its `value` property.
 
-Here is an example showing how to define and use experiment variables in Empyric:
+Here is an example showing how to define and use variables in Empyric:
 ```
 from empyric.variables import Knob, Meter, Parameter, Expression
 from empyric.instruments import Keithley2400
 
 keithley2400 = Keithley2400(1)
 
 voltage = Knob(instrument=keithley2400, knob='voltage')
@@ -94,17 +94,16 @@
 power = Expression(expression='V * I / mW', definitions={'V':voltage, 'I':current, 'mW':milliwatt})
 
 voltage.value = 10 # sets the voltage of the Keithley 2400 to 10 V
 
 # Obtain 10 measurements of current, voltage and power sourced by a Keithley 2400
 measurements = [[current.value, voltage.value, power.value] for i in range(10)]
 ```
-Assigning a value to the `value` property of a knob-type variable commands the corresponding instrument to set the associated knob accordingly, and the value is stored in the corresponding attribute of the instrument (`[instrument].[knob]`). Calling the `value` property of a meter-type variable commands the corresponding instrument to record a measurement of the associated meter, and then return the value as well as store it as an attribute of the instrument  (`[instrument].measured_[meter]`). Calling the `value` property of an expression-type variable retrieves the values of the variables that define it from the stored attributes of the corresponding knobs, meters and other expressions; it does not trigger any new measurements. Therefore, for repeated calls, be sure to trigger measurements or retrievals of the values of any defining variables prior to each evaluation of the expression.
 
-*Routines* allow one to define the trajectory that an experiment takes through parameter space over the duration of the experiment. Every routine has a start and end, assigned variables and assigned values. Routines update their associated variables based on a given state, containing the current time (in seconds) and values of all variables. The most basic routine is the `Hold` routine:
+*Routines* allow one to define the trajectory that an experiment takes through parameter space over the duration of the experiment. Every routine has a set of knobs that it updates based on a given state, containing the current time (in seconds) and values of all relevant variables. The most basic routine is the `Set` routine:
 ```
 import time
 
 # ... define knob1 and knob2 as instances of Knob from above
 
 knobs = {'Knob 1': knob1, 'Knob 2': knob2}
 values = [10, 20]
@@ -124,8 +123,8 @@
 	
 	state['Knob 1] = knob1.value
 	state['Knob 2] = knob2.value
 	
 	print(state)  # prints "{'Time': ..., 'Knob 1': 10, 'Knob 2': 20}"
 ```
 
-An *Experiment* monitors a set of variables as a set of routines takes action on them. In Empyric, the `Experiment` object is an iterable that updates routines and records data on each iteration. It also has `start`, `hold` and `stop` methods which initiate/resume the experiment, holds routines while continuing to measure meters, and stops all routines and measurements, respectively. The `terminate` method saves the collected data to a file in the working directory and raises the `StopIteration` exception. An experiment will terminate automatically when all routines are finished. See henon_python_eaxmple.py in the 'examples/Henon Map Experiment' directory to see how a basic experiment is set up as a python script. This particular example uses a virtual instrument (`HenonMapper`), so the only requirement to run it is having Python installed along with the usual scientific packages (numpy, scipy, pandas and matplotlib).
+An *Experiment* monitors a set of variables as a set of routines takes action on them. In Empyric, the `Experiment` object is an iterable that updates routines and records data on each iteration, which has a defined state. It also has `start`, `hold` and `stop` methods which initiate/resume the experiment, holds routines while continuing to measure meters, and stops all routines and measurements, respectively. The `terminate` method saves the collected data to a file in the working directory and raises the `StopIteration` exception. An experiment will terminate automatically when all routines are finished. See henon_python_eaxmple.py in the 'examples/Henon Map Experiment' directory to see how a basic experiment is set up as a python script. This particular example uses a virtual instrument (`HenonMapper`), so the only requirement to run it is having Python installed along with the usual scientific packages (numpy, scipy, pandas and matplotlib).
```

