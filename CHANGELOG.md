# Changelog

All notable changes to the Key Vault shared module are documented here.
Versions track the pinned AVM `key-vault/vault` module version.

## 0.14.2 — AVM bump

- Updated the AVM Key Vault module reference from `0.10.0` to `0.14.2`.
- Removed deprecated wrapper parameters `enableSoftDelete` and `accessPolicies`.
- Locked RBAC authorization, purge protection, network ACL default action, and
  public network access to their required secure values.
- No AVM parameters or outputs were added, removed, or changed.
- Retained the protected `vaultSku` compatibility alias.

## 0.11.0 — Initial wrapper

- Initial wrapper around `br/public:avm/res/key-vault/vault:0.11.0`.
- SCF-aligned defaults: RBAC-only auth, purge protection, soft-delete 90 days,
  `publicNetworkAccess: Disabled`, `networkAcls.defaultAction: Deny`.
- Outputs: `resourceId`, `name`, `uri`, `resourceGroupName`.
