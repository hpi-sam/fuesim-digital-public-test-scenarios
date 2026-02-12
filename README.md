# FüSim Digital: Public Test Scenarios

Public test scenarios for the [FüSim Digital project](https://github.com/hpi-sam/fuesim-digital/), you are welcome to add test scenarios via pull requests to this repo.

The subfolder migration-test-scenarios contains test scenarios that should be migratable.

It contains only folders following the naming scheme `from-state-[stateVersion]` where [stateVersion] has to be replaced with the version of the state in the exports that are contained in that folder.

These folders contain up to three different folders named `combined-scenarios`, `one-action` or `state-altering-ui` depending on their contents. `combined-scenarios` are tests that test a range of different things. `one-action` are tests that test one action with very little overhead. `state-altering-ui` are tests that test one state altering ui-component with very little overhead.

Those folders contain the actual exports. Things in these folders named starting with EXCLUDE-FROM-TEST will not be tested.

Please use a name that describes what happened in the scenario and add a -complete or -current at the end depending on whether the
export was a full export or an export of the current state.

The resulting naming scheme is: `./migration-test-scenarios/from-state-[stateVersion]/[combined-scenarios | one-action | state-altering-ui]/test-name-[complete | current]`

Please do not create folders without exercises in them.

The files do not need to be formatted in a particular but it is also fine if they are.
