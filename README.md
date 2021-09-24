# Static files

## Col-5 maintenance flags (`flags.json`)

1. Before shutdown chain
  - `maintenanceDownBlock: 5555555` target shutdown col-4 block height
  - `forceMaintenanceDown: false`
  - `useExternalOraclePrice: false`
2. After shutdown chain
  - `maintenanceDownBlock: -1`
  - `forceMaintenanceDown: true`
  - `useExternalOraclePrice: true`
3. Col-5 alive and before oracle bot ready
  - `maintenanceDownBlock: -1`
  - `forceMaintenanceDown: false`
  - `useExternalOraclePrice: true`
3. After oracle bot ready
  - `maintenanceDownBlock: -1`
  - `forceMaintenanceDown: false`
  - `useExternalOraclePrice: false`
