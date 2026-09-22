# ONE4ALL (o4A)
## Project litepaper

Version 0.3 — September 22, 2026

**Published with project-owner approval. Preliminary project disclosure; verification limits remain as stated below.**

This document describes the project, its reported token mechanics and material limitations. It is not an independent audit, legal opinion, investment recommendation or promise of exchange acceptance. It does not establish regulatory status, contractual holder rights or a guaranteed return.

## 1. Project overview

ONE4ALL is a Solana-based community and creative project associated with the o4A token. Its character, Omni, is a black-hooded, green-faced repair cat used in original entertainment, artwork and community-building. The project combines this character-led identity with public information about its token and reward activity.

The intended experience has two parts: people can enjoy Omni and community tools without purchasing a token, while interested users can examine the project's public blockchain and protocol references. Content popularity is not evidence of token demand, financial performance or future adoption.

The project describes o4A as a revenue-share memecoin. In this document, that term refers to the protocol's conditional SOL reward mechanism; it is not a claim of equity ownership, a legally enforceable share of company profits, or a fixed yield. Holders may receive SOL when the protocol distributes rewards. Amounts and eligibility vary, and distributions are not guaranteed.

## 2. Token identity

| Field | Project reference |
|---|---|
| Project | ONE4ALL |
| Token display name | one4All |
| Symbol | o4A |
| Network | Solana |
| Token standard | Token-2022, as displayed by Solscan [4] |
| Decimals | 9 [4] |
| Current supply | 999,966,271.179488869 o4A; Solscan observation September 22, 2026, not a circulating or maximum supply claim [4] |
| Mint | `5BoCYsrqTucqoceJqq8oZbkmrpuzutDsTUkvtTteRREV` |
| Launch platform | RevShare |
| Market reference | Meteora DBC pool `8roivUoLyZbyyxQCFG1bs5uPRo4dC6wXjpyZ8dUZbhpk` |
| Website | https://o4asol.com/ |

The mint, not the name or symbol alone, identifies the token. Similar names and symbols can refer to unrelated assets. RevShare's token page links to the project website, X account and Telegram community. [1]

Solscan displayed owner program `TokenzQdBNbLqP5VEhdkAS6EPFLC1PHnBqCXEpPxuEb`, decimals 9 and the current supply above. Its authority detail displayed Mint Authority, Freeze Authority and Update Authority as `N/A`. Its extension table displayed `metadataPointer` with authority `NULL` and `tokenMetadata` with updateAuthority `NULL`. These are explorer observations, not an independently decoded finalized-chain snapshot or a claim that all protocol controls are absent. [4]

This document does not assert initial, maximum or circulating supply, allocation percentages, a vesting schedule or locked liquidity. Current supply must not be substituted for those distinct fields.

## 3. Fee and reward model

At the September 22 review, the public RevShare token page displayed a **3% tax**, with a **30% creator / 70% holder** fee-distribution split. These are publisher-reported configuration figures, not a percentage return on a holder's investment, and not a division of total token supply. They have not been independently reconciled against the mint configuration or every settlement transaction for this document. [1]

Conceptually, configured token fees feed protocol processing, which may result in SOL distributions to eligible holders. The precise conversion, deductions, eligibility calculation and settlement path require protocol and on-chain verification. Gross fees collected must not be presented as SOL actually paid to holders. Creator receipts must not be described as holder rewards.

RevShare's distribution guide describes multiple possible fee sources, including transfer fees, Meteora position fees and bonding-curve fees. Its general documentation also uses broader language about fees on every transfer. Neither description establishes which mechanism applies to this mint. Pool-level trading fees and token-level transfer fees must be assessed separately. [5]

Solscan's displayed extension table contained `metadataPointer` and `tokenMetadata`; it did not display `transferFeeConfig` during this review. Consequently, RevShare's reported 3% tax must not be described as a verified Token-2022 transfer fee. The applicable trading/protocol fee mechanism still requires reconciliation. Absence from the explorer's displayed table is not a substitute for independent mint-account decoding. [4] Solana's transfer-fee documentation explains that optional extension in general; it does not establish that o4A uses it. [2]

This litepaper makes no promise of a distribution interval, minimum payout, annual percentage yield, universal eligibility or future income. Dashboard configuration and past transactions do not guarantee future distributions. Current eligibility and transaction evidence should be checked through the protocol and explorer links.

## 4. Public product and transparency

ONE4ALL's public project documentation describes an Omni character experience, PFP and meme tools, SOL reward records, a read-only treasury view, and a separate Wall of Legends flow. These are project-described surfaces, not independently audited services. [3]

Read-only treasury and reward viewing is distinct from an explicit wallet action elsewhere on the site. A Wall of Legends action may require wallet authorization; this is not necessary merely to inspect public records. A displayed token valuation is not cash held in a wallet or a guaranteed liquidation value.

The public GitHub repository contains project documentation and media rather than the complete deployable runtime. Public documentation alone does not allow a reviewer to reproduce or audit every operational component. The project's stated agent boundary is that AI assistance does not itself authorize wallet signing, treasury movement or changes to token mechanics. That is an operating policy, not an independent security certification. [3]

## 5. Operations and liquidity

The owner states that liquidity is managed personally. No external professional market-making firm has been identified or contracted according to the owner's disclosures for this document. On-chain liquidity management is not equivalent to a commitment to quote a centralized exchange order book, maintain specified spreads or meet minimum depth requirements.

No independent project audit has been supplied; the owner confirms there is no independent audit. Launching through RevShare does not constitute an audit, platform endorsement, guarantee or assumption of responsibility for ONE4ALL by RevShare. RevShare's own public disclaimer describes independently managed user-created tokens. [1]

This document does not claim a registered issuer entity, incorporation jurisdiction, verified executive identities, institutional investors, fundraising history, formal governance rights or legal clearance. Exchanges may require those facts separately. Personal contact details and identity documents are intentionally excluded from the public-facing document.

## 6. Exchange integration considerations

An exchange must assess Solana Token-2022 and the actual enabled extensions, not assume that generic Solana support is sufficient. Review should cover deposit and withdrawal behavior, relevant authorities and changes, custody-wallet reward behavior, market liquidity and protocol dependencies. Any transfer-fee or withheld-fee handling requirements must be established from the actual mint configuration, not inferred from RevShare's tax label.

An exchange-held balance must not be represented as guaranteeing end-user reward eligibility or pass-through. Any such treatment needs explicit technical and commercial agreement with the venue.

ONE4ALL is seeking consideration through no-fee or zero-budget application routes. This document does not commit tokens, deposits, paid marketing, liquidity capital or market-making services. Submitted applications, directory profiles and DEX tracking pages are not evidence that a centralized exchange has approved trading.

## 7. Risks and limitations

- **Loss and liquidity:** token prices can fall substantially or to zero; a holder may be unable to sell the desired amount. Self-managed liquidity is not a liquidity guarantee.
- **Reward uncertainty:** fees, activity, eligibility, protocol operation and costs can change outcomes. No distribution or amount is assured.
- **Technical and custody:** token extensions, contracts, wallets, frontends and third-party integrations can fail or be exploited. No independent project audit is claimed.
- **Control and concentration:** authority configuration, ownership concentration and liquidity-control rights remain to be documented and independently checked. Their omission is not evidence that these risks are absent.
- **Data quality:** protocol dashboards and market trackers may be stale, incomplete or inconsistent. Estimates, token valuations and reported totals must be distinguished from settled transactions.
- **Operational dependence:** continuity depends on the project operator, Solana, RevShare and other service providers. No service-level or delivery guarantee is given.
- **Regulatory and venue restrictions:** legal treatment and exchange availability vary. This document does not establish compliance or eligibility in any jurisdiction.

## 8. Development direction

The project's stated direction is to continue original Omni content, community tools and clearer public project information. Potential exchange access is subject to independent venue review. This document establishes no funded delivery schedule, token-price objective or guaranteed listing milestone.

## 9. References and evidence scope

1. [RevShare — exact-mint token page](https://app.revshare.ltd/token/5BoCYsrqTucqoceJqq8oZbkmrpuzutDsTUkvtTteRREV). Live browser observation September 22, 2026; dynamic publisher content, publication date unavailable. Supports displayed identity, links and reported fee split, not independent audit or permanent configuration.
2. [Solana — Transfer Fees documentation](https://solana.com/docs/tokens/extensions/transfer-fees). Reviewed September 22, 2026; general technical documentation, not verification of o4A's specific mint.
3. [ONE4ALL — current project notes](https://github.com/o4a-sol/ONE4ALL/blob/main/NOW.md) and [project overview](https://github.com/o4a-sol/ONE4ALL). Project-authored documentation refreshed September 22, 2026; descriptions and policy statements, not independent assurances.
4. [Solscan mint](https://solscan.io/token/5BoCYsrqTucqoceJqq8oZbkmrpuzutDsTUkvtTteRREV). Live explorer observation September 22, 2026, including Overview, expanded Authority and Metadata/Extensions table. Supports the displayed current supply, decimals, owner program and specific authority/extension labels reported above. No finalized slot or independent RPC decoding was captured; dynamic values can change. Additional verification destinations: [DEX Screener pool](https://dexscreener.com/solana/8roivuolyzbyyxqcfg1bs5upro4dc6wxjpyz8duzbhpk) and [project website](https://o4asol.com/).

5. [RevShare distribution guide](https://app.revshare.ltd/guides/distribution-system) and [general documentation](https://app.revshare.ltd/docs). Reviewed September 22, 2026; publication dates unavailable. Platform descriptions differ in scope; neither is mint-specific verification. [Meteora DBC documentation](https://github.com/MeteoraAg/docs/blob/main/core-products/dbc/what-is-dbc.mdx) documents configurable pool-level fees and Token-2022 launch support, not o4A's exact configuration.

Owner disclosures concerning audit status, absence of a prior whitepaper, and personal liquidity management were provided during preparation of this document. They are owner-reported, not independently attested. This new litepaper must not be represented as a document that existed at token launch.

## 10. Outstanding verification

Publication was authorized by the project owner on September 22, 2026. The following verification remains outstanding: reconcile fee and reward mechanics, including the distinction between RevShare's tax label and Solscan's displayed extensions; independently confirm the explorer observations using a dated finalized-chain snapshot and document remaining protocol controls; check current links and product descriptions; and retain the explicit unresolved disclosures where verification remains incomplete. Legal or exchange-specific requirements need separate review. A published litepaper may satisfy a URL field but does not guarantee application eligibility or acceptance.
