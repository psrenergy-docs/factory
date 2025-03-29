---
title: Release Notes
nav_order: 2
---

📚 [Factory Documentation](https://docs.psr-inc.com/factory/)

# Version 4.0.22

🔗 [Download for Windows](https://www.psr-inc.com/app/link/?t=d&f=factory_python-4.0.22-windows-x64-9392bcb-release.zip)

🔗 [Download for Linux](https://www.psr-inc.com/app/link/?t=d&f=factory_python-4.0.22-linux-x64-d611670-release.zip)

## Changes

- Rename `MaximumStoragePenalty` to `MaximumOperativeStoragePenalty`.

- Remove validation for negative values of `EvaporationCoefficient`, `MaximumOperativeStoragePenalty` and `MinimumOperativeStoragePenalty`.

- Fix `psr.runner` module, fix SDDP version check for beta and release candidate versions.


# Version 4.0.21

## Changes

- Add capability of generating external scenarios via TSL.

- Add support for reading/saving `gndforh.dat` as/from dataframe.

- Add `run_sddp_convert_fcf` to `psr.runner` module.

- Add `type` member to property descriptions.

- Fix reading/setting `ReserveGeneration` `HourReserve`.

- Fix saving incomplete `EnergyPerBlock` data.

- Fix saving incomplete `VariableDurationOfBlocks` data.

- Fix saving SDDP circuit data - avoiding GUI update.

- Update `psr.cloud` module.


# Version 4.0.20

## Changes

- Fix saving Hydro and Thermal plant maintenance data.

- Fix generating detailed log.

- Fix saving secondary reserve prices.

- Fix saving hour block map.

- Update property descriptions.

- Rename `Bus`' `VoltageLevel` to `BaseVoltage`.


# Version 4.0.19

## Changes

- Fix `Study.get_df` when reading references.

- Update pycloud module, remove CPU limit.

- Add new sddp parameters.


# Version 4.0.18

## Changes

- Fix loading monthly/hourly dataframes data.

- Remove duplicated element check on reference lists.

- Update `psr.cloud` module.

- Update `CSP` TSL properties.


# Version 4.0.17

## Changes

- Optimize reading binary outputs via `load_dataframe`.

- Fix `FilterAgents` of `DataFrameLoadOptions`.

- Rename `FilterSeries` to `FilterScenarios` of `DataFrameLoadOptions`.

- Update docs on filtered output data.

- Update `psr.cloud` module.


# Version 4.0.16

## Changes

- Fix setting and getting `InterpolationGenericConstraint`'s name and code.

- Fix accessing read-only Study properties such as `CalculatedFinalYear` and `CalculatedFinalStage`.

- Rename `MinimumStoragePenalty` to `MinimumOperativeStoragePenalty` to avoid clash with existing NCP property.

- Rename `FinalYear` to `CalculatedFinalYear` and `FinalStage` to `CalculatedFinalStage`.


# Version 4.0.15

## Changes

- Add `run_sddp_cleanup`, `run_optgen_cleanup`, and `run_optgen_check` to `psr.runner` module.

- Fix loading `GenericConstraint` objects.


# Version 4.0.14

## Changes

- Add `MinimumOperativeStorage` constraint, converting `MinimumStorage` as the `HydroPlant` reservoir structural value.

- Fix saving OptGen study with batteries and without network data.

- Fix validation error message on saving output/dataframes.

- Update error treatment for longer messages.

- Fix saving variable duration data.

- Update PyCloud module.


# Version 4.0.13

## Changes

- Fix crash with old VC++ redistributables.

- Downgrade Linux build to support libc.so 2.28.


# Version 4.0.12

🔗 [Download for Windows](https://www.psr-inc.com/app/link/?t=d&f=factory_python-4.0.12-windows-x64-686ec3d-release.zip)


## Changes

- Optimize `find`, `find_by_name`, `find_by_code`, `find_by_id`.

- Add deprecation warning to `find_by_code` called with one string argument.

- Fix reading results by block and hours.


# Version 4.0.11

## Changes

- Fix weekly cases hourly date/time string format.

- Fix reading `RefElements` of loaded `InterpolationGenericConstraint` objects.


# Version 4.0.10

🔗 [Download for Linux](https://www.psr-inc.com/app/link/?t=d&f=factory_python-4.0.10-linux-x64-81c519a1-release.zip)

## Changes

- `Study.get_at`, `Study.set_at`, `DataObject.get_at`, `DataObject.set_at` accepting Python's `datetime` object as date argument.

- Fix `psr.runner` module for beta SDDP versions.

- Add `cluster_settings` to `psr.runner.run_sddp`.


# Version 4.0.9

## Changes

- `Study.find_by_code` accepting two parameters - type name as string and object code as integer.

- Add support for paths specified with `pathlib.Path` objects.

- Fix reading `RefElements` of `InterpolationGenericConstraint` objects.

- Add `TSLMainTurbinePath`, `TSLCustomTurbinePath`, and `TSLMERRAPath` properties to `LoadOptions` objects.


# Version 4.0.8

## Changes

- Fix reading dates on Linux version.

- Fix loading `SumOfCircuits` of NetPlan studies.

- Add support for `CircuitFlowConstraint` of NetPlan studies.


# Version 4.0.7

## Changes

- Update `psr.cloud` module, fix auth issue.

- Update `psr.runner` module, fix SDDP parallel run.


# Version 4.0.6

## Changes

- Fix issue identifying integer/float types coming from `pandas`/`numpy` packages.


# Version 4.0.5

## Changes

- Fix `GenerationConstraint`'s `RefPlants` and `RefBatteries`.

- Fix validation of `R` and `X` values for circuits.

- Update `psr.cloud` module.

- Update `psr.runner.run_nwsddp`.


# Version 4.0.4

## Changes

- Fix saving `ExpansionGenericConstraint`.

- Add `run_optgen` to `psr.runner` module.

- Add `run_sddp_check` to `psr.runner` module.

- Add `run_hydro_estimation` to `psr.runner` module.


# Version 4.0.3

## Changes

- Optmize loading dataframes from output files.


# Version 4.0.2

## Changes

- Add support for `ExpansionGenericConstraint`

- Optmize loading dataframes from output files.


# Version 4.0.1

## Changes

- Fix coefficients of GenericConstraint, SumOfCircuit and SumOfInterconnection constraints of loaded cases.

- Update `psr.cloud` module, import cases to PSR Cloud Desktop.

- Add `run_nwsddp` to `psr.runner` module.


# Version 4.0.0

## Changes

- Add `psr.factory.DataFrame` object

- Read/write/convert models' output files

- Conversion from `psr.factory.DataFrame` to `pandas.DataFrame`/`polars.DataFrame` and vice-versa.

- Bundle `psr.cloud` module for PSR Cloud case upload and control automation.


# Version 3.6.5

## Changes

- Allow `TwoTerminalsDCLink` objects on `SumOfCircuits` constraints.


# Version 3.6.4

## Changes

- Fix fast case loading.

- Update docs.


# Version 3.6.3

## Changes

- Fix log levels.

- Fast NetPlan case loading.


# Version 3.6.2

## Changes

- Fix loading/saving `CSP` data.

- Rename `DCLink` to `TwoTerminalsDCLink`.

- Add `MTDCLink` as NetPlan's detailed `DCLink`.


# Version 3.6.1

## Changes

- Fix loading `DCLink` data from NetPlan studies.


# Version 3.6.0

## Changes

- Add `TSL` model support.

- Load and save Hydrological Parameter Estimation data with SDDP studies.

- Add `NetPlanIncrementalToSddp` option to `LoadOptions` to control loading detailed SDDP data.


# Version 3.5.1

## Changes

- Add references properties to documentation.

- Hide internal properties from documentation.

- Fix `HydroPlant`'s `OperationMode` property access.

- Performance improvements.


# Version 3.5.0

## Changes

- Add diagnostics features:

	- `set_log_level` enable log generation in current working directory (`factory.log`).

	- `set_debug_mode` adds more details in log messages such as loaded elements.


# Version 3.4.5

## Changes

- Fix bug where factory enters into an infinite loop while accessing planned NetPlan data.

- Automatically load OptGen data when NetPlan model is specified.

- Fix multidimensional property default expression.

- Fix issue with property names containing `.`.

- Fix loading NetPlan cases with `LCCConverter`, `VSCConverter` and `SeriesCapacitor`.


# Version 3.4.4

## Changes

- Fix bug where a weekly case's context is set as monthly.

- Fix dataframe date format to reflect case's stage type (weekly or monthly).


# Version 3.4.3

## Changes

- Remove temporary files (.tmp) generated after loading a study when a study is deleted or module unloaded.


# Version 3.4.2

## Changes

- Fix behaviour of `clear_values` and `set_at` after clearing values of a property grouped with other(s).


# Version 3.4.1

## Changes

- Fix support for other encodings such as latin-1.


# Version 3.4.0

## Changes

- Fix behaviour of `clear_values` - previous version could clear other grouped values.

- `clear_value` will set property values to the default when grouped with other values. 


# Version 3.3.11

## Changes

- Fix DataFrame index name when DataObjects are returned as indices.


# Version 3.3.10

## Changes

- Fix handling empty hourly scenarios.

- Update `psr.runner` module, adds `run_psrio` function.


# Version 3.3.9

## Changes

- Update docs.


# Version 3.3.8

## Changes

- Make `RenewablePlant`'s `RefStation` optional for Unitary Scenario option.


# Version 3.3.7

## Changes

- Improved error mesages when invalid indices are provided do `set_df`.


# Version 3.3.6

## Changes

- Add name to returned dataframe's index.

- Add `extra_args` parameter to `psr.runner.run_sddp` method.


# Version 3.3.5

## Changes

- Add reflection method to access grouped properties (`grouped_with`).


# Version 3.3.4

## Changes

- Fix setting `ThermalPlant` modification values to `None`.


# Version 3.3.3

## Changes

- Update NetPlan database support.


# Version 3.3.2

## Changes

- Add support for `numpy` int and float types.


# Version 3.3.1

## Changes

- Fix sorting battery modification by date (`mbattery*.dat`).


# Version 3.3.0

## Changes

- Update `DataObject.get_df` and `Study.get_df` behaviour: show `None` values when a grouped property contains no value set at that date. Reproduces modification files behaviour with blank values.


# Version 3.2.16

## Changes

- Update `psr.runner` module, call NCP's post-build script.


# Version 3.2.15

## Changes

- Fix valid values of `Activities` property.


# Version 3.2.14

## Changes

- Implement `remove` for `RenewableStation` objects.


# Version 3.2.13

## Changes

- Add `clear_values` method.

- Add streamlit simulation_loop.py dashboard sample.

- Minor changes in docs and Python binding


# Version 3.2.12

## Changes

- Deprecate `fetch`, replaced with `get_df`.

- Deprecate `update`, replaced with `set_df`.


# Version 3.2.11

## Changes

- Add `RefTransformers` to `ThreeWindingsTransformer` objects.

- Fix `help` call on objects.

- Fix Sddp's `DCLink` object creation.


# Version 3.2.10

## Changes

- Add `RefTransformers` to `ThreeWindingsTransformer` objects.


# Version 3.2.9

## Changes

- New docs structure and fixes on automatic generation


# Version 3.2.8

## Changes

- Fix regression loading `HydroPlant` objects.


# Version 3.2.7

## Changes

- Add `LoadOptions` object support.


# Version 3.2.6

## Changes

- Add `NetPlan` model support.


# Version 3.2.5

## Changes

- Fix adding NCP's `TargetGeneration` objects to `Study`.


# Version 3.2.4

## Changes

- Rename NCP's `MaintenanceValue` for hydro units to `Maintenance`.


# Version 3.2.3

## Changes

- Rename NCP's `MaintenanceValue` for hydro units to `Maintenance`.


# Version 3.2.2

## Changes

- Fix NCP's `MaintenanceValue` for hydro units.


# Version 3.2.1

## Changes

- Fix NCP's `MaintenanceValue` for `HydroPlant`s, `ThermalPlant`s and circuits.

- Fix NCP's `ForcedGeneration` for `ThermalPlant`s.

- Add `MaintenanceUnit` for NCP's Hydro units.


# Version 3.2.0

## Changes

- Implement support for intervallic data such as maintenances.


# Version 3.1.1

## Changes

- Add `get_objects_values` and `get_objects_values_at` to `Study` objects.

- Fix `MaintenanceValue` of `HydroPlant` and `ThermalPlant` objects.


# Version 3.1.0

## Changes

- Add `find_by_name`, `find_by_id`, and `find_by_code` methods to `Study` objects.


# Version 3.0.7

## Changes

- Use system character encoding by default instead of `utf-8` to handle library strings.

- Add `get_default_encoding` and `set_default_encoding` methods to override library string encoding.


# Version 3.0.6

## Changes

- Add support for NCP's `ShortTermGeneration` on `RenewablePlant` objects.


# Version 3.0.5

## Changes

- Raises an exception when passing any object type other than `DataObject` to `add` and `remove` functions.

- `Study.context` and `DataObject.context` are no longer functions, but properties.

- Fix bug on loading data for `System` that contains `TargetGeneration` constraints.


# Version 3.0.4

## Changes

- Fix accessing `RefGenerators` property of `RenewablePlant` objects.


# Version 3.0.3

## Changes

- Fix saving NCP `condih.dat`.

- Fix initial value of `StageDuration` for NCP studies.

- Fix copying `Models` property of `Context` objects.

- Fix `DataObject` context when instantiated via `find`.


# Version 3.0.2

## Changes

- Fixed Study's `FixedDurationOfBlocks` property.

- Study's `StagesCount` renamed to `NumberOfStages`.

- Study's `ScenariosCount` renamed to `NumberOfSeries`.

- Fix saving NCP condit.dat and condih.dat.

- `psr.runner` raises `RuntimeError` on simulation error.

- Fix `psr.runner` relative case path support.

- Fix `DataObject.get` when unique value is not at beginning of the time.

- Add aliases for new properties after updating reference PSRDataDictionary.xml


# Version 3.0.1

## Changes

- Fix NCP sddpcp.dat's fcf file name.


# Version 3.0.0

## Changes

- Add `psr.runner` module, with `run_sddp` and `run_ncp` methods.



