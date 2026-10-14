# WaEnhancer + fix for upstream issue #838

Patched builds of [Dev4Mod/WaEnhancer](https://github.com/Dev4Mod/WaEnhancer) that carry the fix for
[#838](https://github.com/Dev4Mod/WaEnhancer/issues/838) (missing "+" button in the chat filter row).

`patches/*.patch` are applied on top of the latest upstream commit every 6 hours. A new APK is attached to a
release in this repo whenever upstream has a commit that was not built yet.

## One-time setup
1. Put these files in a new GitHub repo of yours.
2. Settings > Actions > General > Workflow permissions: Read and write.
3. Optional but recommended: add secrets KEY_STORE (base64 of your .jks), KEY_STORE_PASSWORD, ALIAS, KEY_PASSWORD.
   Without them each build is signed with a different key and you must uninstall the previous build first.
4. Actions > Build patched WaEnhancer > Run workflow.
