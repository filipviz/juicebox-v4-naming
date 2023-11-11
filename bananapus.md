# Bananapus Naming Suggestions

Contract names -> `s/^JB/BP/`

## I. bananapus-721-staking-delegate

Rename repo to `staking-hook`

### 1. JB721StakingDelegate

- Rename contract to `BPStakingHook`.
- "Token" and "tokens" can be vague given that both could refer to ERC-20s or ERC-721s depending on the context. Consider sticking to ERC-20 and ERC-721 (or staking token and "positions").
- Consider `encodedIPFSUri` -> `encodedFallbackIPFSUri` to make it clearer that this is used when no token resolver is provided.
- Consider `tierMultiplier` -> `tierPriceStep` or `tierPriceIncrement`, and `_getTierBaseAmount(...)` -> `_getTierMultiplier(...)`.
- Consider `userVotingPower` -> `totalVotingPowerOf` or `totalVotesOf`.
- Consider `numberOfTokensMintedOfTier` -> `mintCountForTierId` or even `mintCount`
- Consider `LockManagerUpdated` event -> `LockManagerSet` (consistent with function name).
- Consider `_getTierMinStake(...)` -> `_getTierPriceMinimum(...)` (maybe `_getTierPriceFloor(...)`)
- Should this repo and the tentacles repo be combined? Both heavily interface with the lock manager. 
- Consider `_generateTokenId(...)` -> `_tokenIdFromTierAndNumber(...)`
- Consider `tierIdOfToken(...)` -> `tierIdFromTokenId(...)`.

<!-- ### 2. JB721StakingDelegateDeployer

Rename contract to `BPStakingHookDeployer` (maybe `BPStakingProjectDeployer`)

## II. bananapus-distributor

Rename repo to

## III. bananapus-tentacles

Rename repo to

## IV. bananapus-sucker

Rename repo to -->
