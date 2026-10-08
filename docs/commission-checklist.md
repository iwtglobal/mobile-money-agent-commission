# Commission Design Checklist — Mobile Money Agents

A working checklist for designing or reviewing **mobile money agent and dealer commission**. Use it before launch and at every plan change.

## Structure

- [ ] Every billable transaction type has a commission rule (cash-in, cash-out, registration, bill payment, merchant payment, wallet-to-bank)
- [ ] Commission bands line up with customer fee bands
- [ ] Agent and dealer shares are defined for each rule
- [ ] Zero-fee or promotional products have an explicit commission rule (not an accidental zero)
- [ ] Caps exist on percentage-based commission

## Integrity

- [ ] Registration commission is paid only after a qualifying first transaction
- [ ] Splitting detection: same customer, same agent, short window, amounts near band edges
- [ ] Self-dealing detection: agent transacting with their own or linked wallets
- [ ] Commission reverses automatically when the transaction is reversed
- [ ] Outlier report: agents whose commission per customer is far above their peers

## Payout

- [ ] Commission is held in a separate commission wallet or ledger, not mixed with float
- [ ] Payout frequency is defined (instant, daily, monthly) and communicated
- [ ] Withholding or other required taxes are deducted at payout and reported
- [ ] Agents and dealers receive statements showing each transaction and share

## Governance

- [ ] Plan changes go through maker-checker approval
- [ ] Every plan has an effective-from date; old plans remain for historical recalculation
- [ ] Dealers can view, but not edit, their agents' commission
- [ ] Monthly reconciliation: commission paid equals commission rated minus clawbacks

## Related

See the main [README](../README.md). Product context: [merchant and agency onboarding, commissions and QR](https://evdsystem.com/evd-software/merchant-agency-onboarding-commissions-qr/).
