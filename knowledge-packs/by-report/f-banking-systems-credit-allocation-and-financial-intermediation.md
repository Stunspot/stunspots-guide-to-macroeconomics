# **F. Banking Systems, Credit Allocation, and Financial Intermediation — The Operational Architecture of Credit Creation and Capital Distribution**

Commercial banks and non-bank financial intermediaries do not merely distribute pre-existing capital; they act as the primary operational conduits through which purchasing power is generated, priced, and selectively distributed across the macroeconomy. While aggregate monetary policy operates on system-wide liquidity parameters, the transmission of that policy is highly selective, regulated by institutional filters, balance-sheet constraints, and risk-pricing terms.

This report traces the mechanics of credit creation, wholesale funding, maturity transformation, shadow banking channels, corporate and consumer credit markets, and the structural entanglement between the banking system and the sovereign state.

## **Operational Mechanics of Credit Creation and Interbank Settlement**

The foundational mechanism of commercial banking is the expansion of the balance sheet through credit creation, a process historically termed "fountain pen money".1 Contrary to the loanable-funds model, which posits that banks act as passive intermediaries lending out pre-existing deposits, modern commercial banks create deposits endogenously in the act of lending.1

### **The Endogenous Credit Creation Process**

When a commercial bank approves a loan, it does not transfer physical currency or pre-existing central bank reserves to the borrower.2 Instead, it executes a bilateral ledger expansion:

Bank Asset: Loan (Borrower's Promise to Pay) \<--\> Bank Liability: Deposit (Bank's Promise to Pay on Demand)

New broad money is created at the transaction interface.1 The borrower's note represents an illiquid asset for the bank, while the newly credited deposit represents a highly liquid, demand-executable liability that enters the broad money supply.1

The bank's capacity to create credit is not constrained ex-ante by the quantity of reserves it holds.2 Rather, the reserve constraint operates ex-post, arising when the borrower draws down the deposit to make payments to accounts at other institutions.2

### **Interbank Settlement and Reserve Management**

While a bank can create deposits without a prior transfer of reserves, the settlement of those deposits across different banks requires the wholesale clearing layer of the monetary hierarchy.1 If a borrower transfers funds to a recipient at another bank, the originating bank must settle the obligation by transferring central bank reserves through the national real-time gross settlement (RTGS) system (e.g., Fedwire in the United States, TARGET2 in the Eurozone).1

This wholesale settlement layer operates on a double-entry ledger managed by the central bank:

Change in Originating Bank Reserves (Asset at Central Bank) \< 0 \<--\> Change in Receiving Bank Reserves (Asset at Central Bank) \> 0

Central bank reserves do not circulate in the wider retail economy; they exist solely to settle net clearing balances between authorized depository institutions and the sovereign issuer.1 Thus, reserve management is the process of acquiring sufficient clearing balances ex-post to meet these settlement obligations and satisfy statutory reserve requirements, if any.2

If a bank faces a net reserve deficit at the end of the clearing cycle, it must secure funding in the wholesale interbank market, tap central bank standing facilities, or draw down liquid assets.4

### **Bank Balance-Sheet Mechanics Map**

The table below maps the structural interactions of bank balance-sheet components under various operational and stress conditions.

| Transaction / Event | Asset-Side Balance Sheet Impact | Liability-Side Balance Sheet Impact | Regulatory Capital & Liquidity Impact | Operational / Macro Consequence |
| :---- | :---- | :---- | :---- | :---- |
| **Endogenous Loan Origination** | Change in Loans \+100 2 | Change in Deposits \+100 2 | Risk-Weighted Assets (RWA) rise 7; LCR decreases as simulated outflows increase.7 | Expands broad money supply; no initial change in base money.2 |
| **Interbank Payment Settlement** | Change in Reserves \-100; Net change: 0 4 | Change in Deposits \-100; Net change: 0 2 | HQLA falls 9; LCR declines unless offset by cash inflows.7 | Restricts liquidity buffer; forces bank to source wholesale funding.5 |
| **FHLB Advance Drawdown** | Change in Reserves \+100 5 | Change in Short-Term Borrowings \+100 6 | Increases HQLA 9; improves short-term LCR but requires collateral encumbrance.6 | Super-senior lien is placed on bank assets, subordinating depositors.6 |
| **BTFP Par Valuation Borrowing** | Change in Reserves \+100 11 | Change in Secured Term Debt \+100 12 | Replaces lost deposits; avoids HQLA fire sales and regulatory capital hits.13 | Transfers duration loss to the public balance sheet via undercollateralization.14 |
| **Loan Write-Off (Default)** | Change in Allowance for Credit Losses \-100; Change in Gross Loans \-100 1 | Net 0 on liabilities; Change in Retained Earnings \-100 | Reductions in CET1 Capital 7; Risk-Weighted Assets decrease slightly. | Direct hit to bank solvency; credit contraction ensues.1 |

## **Bank Funding Architectures, Deposit Betas, and Digital Run Dynamics**

To sustain credit expansion and settle transaction balances, commercial banks construct a liability framework designed to manage interest rate sensitivity, regulatory compliance, and run risk. This liability hierarchy is detailed in the Bank Funding Fragility Map below.

A critical determinant of bank profitability and deposit stability during monetary tightening cycles is the **deposit beta**—defined as the percentage of a change in the central bank's policy rate that a bank passes through to its deposit pricing.17 During the aggressive monetary tightening cycle of 2022–2023, where the Federal Reserve raised the federal funds target rate by 525 basis points, the average cumulative US deposit beta was approximately 0.27, though it varied significantly by institution size and depositor sophistication.17

Small Banks (\< 1B USD assets): Cumulative Beta ≈ 0.25  
Digital-Broker / Highly Sophisticated Banks: Cumulative Beta ≈ 0.44 \- 0.46

This pricing friction generates the **deposit franchise value**, which represents the intangible asset value accruing to a bank from its capacity to maintain sticky, low-cost retail deposits.19 Under zero-interest-rate regimes, the deposit franchise value approaches zero, but it expands significantly as policy rates rise—provided deposits remain stable.19

However, the proliferation of digital banking platforms, mobile applications, and integrated brokerage sweep accounts has structurally altered deposit behavior.17 In 2022–2023, rather than displaying historical inertia, financially sophisticated depositors engaged in a rapid **digital bank walk**, reallocating balances away from low-yielding transactions accounts into high-yielding wholesale vehicles such as money market funds (MMFs).17

This digital migration forces banks to choose between two balance-sheet strains:

1. Suffer deposit outflows, shrinking the balance sheet and forcing the liquidation of high-quality liquid assets (HQLA) or the accumulation of high-cost wholesale liabilities.17  
2. Aggressively raise deposit rates, which spikes the deposit beta, compresses the net interest margin (NIM), and erodes the deposit franchise value.17

### **Deep Dive: Silicon Valley Bank (SVB) Pre-Run Insolvency Metrics**

The structural fragility of a digital-broker model is illustrated by the collapse of Silicon Valley Bank (SVB) in March 2023\.19 In 2022, SVB held 173.1 billion USD in deposits and reported 2.2 billion USD in pre-tax income.19 Under its digital-broker parameters, SVB experienced an extreme rate of deposit franchise value erosion.19

Because of its razor-thin operating margins, if SVB had raised deposit rates by just 125 basis points to match the Fed's target rate hikes, its interest expenses would have wiped out its entire annual net profit.19 In fact, SVB's actual interest paid on deposits surged from 62 million USD in 2021 to 862 million USD in 2022\.19

The bank’s deposit franchise value, when calculated with digital-broker parameters (which account for rapid outflows and higher betas), was 14% to 22% lower than that of a comparable traditional bank.19 This impairment eliminated the deposit franchise's natural role as an interest rate hedge, driving SVB into economic insolvency months before the actual retail run materialized.19

### **Bank Funding Fragility Map**

| Funding Instrument | Cost Structure | Behavioral Stability | Run Risk & Digital Sensitivity | Regulatory / LCR Treatment |
| :---- | :---- | :---- | :---- | :---- |
| **Insured Retail Deposits** | Low; highly lagged rate pass-through (low beta).17 | High; anchored by federal safety net.6 | Low; highly insulated from digital runs.19 | Presumed stable; receives 3% to 5% runoff rate under LCR.8 |
| **Uninsured Retail Deposits** | Medium; subject to moderate beta pressure.17 | Moderate; influenced by institutional panic.17 | High; vulnerable to social-media-driven runs.17 | Treated as less stable; receives 10% runoff rate under LCR.7 |
| **Brokered Deposits** | High; priced directly at wholesale money market yields.5 | Low; hot money pursuing yield optimization.5 | High; easily withdrawn at maturity or upon bank downgrades.5 | Subject to highly restrictive regulatory caps and high LCR runoff rates.5 |
| **Uninsured Wholesale Deposits** | High; tied directly to market benchmark rates.17 | Low; highly sensitive to bank solvency metrics.17 | Very High; prone to rapid, synchronized digital flight.17 | Treated as unstable; receives 40% to 100% runoff rate under LCR.8 |
| **Repo Funding** | Low-to-Medium; linked to SOFR.23 | Dependent on daily mark-to-market valuations.23 | High; subject to sudden haircut increases and collateral rejection.23 | High regulatory value if collateralized by HQLA; subject to capital rules.7 |
| **FHLB Advances** | High; floating or fixed rates pegged to market cost of funds.6 | Medium; accessible as long as eligible collateral is prepositioned.6 | Low; secured by super-senior legal priority over bank assets.6 | Counts as stable wholesale funding; requires collateral pledging.6 |
| **Interbank Borrowing** | High; typically priced at Fed Funds effective rate.27 | Low; highly sensitive to market-wide liquidity shocks.5 | High; overnight lines can be cut instantly. | Short-term funding; receives high required outflow factors.7 |
| **Commercial Paper (CP)** | High; tied to credit quality and short-term rates.24 | Low; requires continuous rolling of short maturities.24 | High; markets can lock up completely during systemic stress.29 | Unsecured wholesale; receives 100% outflow rate under LCR.7 |
| **Securitization / ABS** | Medium; structural cost of tranche design.24 | High; transfers underlying assets off-balance-sheet.24 | Low; once issued, funding is structurally locked in.30 | Enhances balance-sheet space and conserves capital.24 |
| **Central Bank Facilities** | High; primary credit rate pegged to top of target range.13 | High; reliable lender of last resort.22 | Extremely Low; operates as administrative backstop.31 | High stigma prevents proactive usage; collateral must be pre-pledged.22 |

## **Maturity Transformation, Regulatory Constraints, and Underwriting Cycles**

Maturity transformation is the core economic proposition of banking: institutions create value by absorbing short-term, highly liquid liabilities (such as demand deposits) and investing in long-term, illiquid, and risky assets (such as commercial mortgages, industrial loans, and corporate infrastructure finance).24 This structural mismatch exposes the banking system to inherent vulnerabilities. If all liability holders simultaneously demand cash, the bank's illiquid assets cannot be monetized rapidly without triggering catastrophic fire sales and systemic insolvency.8

To manage this risk, modern states provide regulatory frameworks, liquidity backstops, and deposit insurance systems.4

### **The Basel III Regulatory Apparatus**

Post-2008 macroprudential regulation operates on the assumption that banking safety can be mathematically codified through capital and liquidity constraints.7 The primary pillars of this apparatus include:

1. **Common Equity Tier 1 (CET1) Capital Ratio**: The ratio of high-quality loss-absorbing equity capital to Risk-Weighted Assets (RWA) 7:  
   CET1 Ratio \= Common Equity Tier 1 Capital / Risk-Weighted Assets \>= 4.5% (plus macroprudential buffers) 7  
   Risk-weighted assets are calculated by multiplying specific asset categories by regulatory risk weights (e.g., 0% for sovereign debt, 50% for standard residential mortgages, 100% or higher for commercial corporate loans).7  
2. **Liquidity Coverage Ratio (LCR)**: This short-term liquidity constraint requires banks to hold an adequate stock of unencumbered High-Quality Liquid Assets (HQLA)—such as central bank reserves and government bonds—that can be easily converted into cash to meet simulated cash outflows over a 30-day stress horizon 7:  
   LCR \= Stock of HQLA / Total Net Cash Outflows over 30 Days \>= 100% 7  
   A structural inefficiency of the LCR is that it functions as an unusable buffer.8 Because breaching the 100% threshold triggers severe regulatory and market penalties, banks must hoard an additional "usable" layer of liquidity above the statutory minimum, restricting their capacity to extend credit to the real economy during stress events.8  
3. **Net Stable Funding Ratio (NSFR)**: A medium-to-long-term structural constraint designed to align the maturities of assets and liabilities over a one-year horizon 7:  
   NSFR \= Available Stable Funding (ASF) / Required Stable Funding (RSF) \>= 100% 9  
   Available Stable Funding (ASF) is calculated by applying stability factors to liabilities (e.g., regulatory capital receives a 100% factor; retail deposits receive a 90% to 95% factor).28 Required Stable Funding (RSF) applies liquidity factors to assets, forcing banks to back long-term loans and illiquid holdings with more stable, long-term liabilities.28

### **Underwriting Cycles and Credit Terms**

Underwriting is the mechanism through which macroeconomic regimes translate into micro-level risk pricing. During economic expansions, rising asset values and low default rates compress risk premia.35 Underwriting standards loosen as risk models over-weight recent performance, covenants are stripped from loan agreements, and Debt-Service Coverage Ratios (DSCR) are calculated under optimistic growth and low interest rate assumptions.36

Crucially, credit tightening does not manifest solely through loan rejection; it operates by manipulating credit terms.20 The table below compares these parameters across borrower classes.

### **Credit Underwriting and Terms Map**

| Borrower Segment | Cash-Flow / Underwriting Basis | Collateral Basis & LTV Limits | Covenant & Amortization Structure | Refinancing Dependency | Macro & Rate Sensitivity |
| :---- | :---- | :---- | :---- | :---- | :---- |
| **Middle-Market Corporate** | EBITDA multiples; Debt/EBITDA ratios.36 | Senior secured liens on enterprise assets.36 | Shifting from maintenance to incurrence-only covenants.36 | High; heavily dependent on revolving facility rollovers.37 | High; floating-rate structures expose cash flows to rate hikes.36 |
| **Commercial Real Estate (CRE)** | Net Operating Income (NOI); DSCR metrics.40 | Property appraisal values; LTV typically capped at 60-65%.41 | Standard amortization with significant bullet payments at maturity.42 | Extreme; requires periodic refinancing of large principal balances.41 | Extreme; highly sensitive to capitalization (cap) rates.40 |
| **Residential Mortgage** | Debt-to-Income (DTI); verifiable household wages.44 | Residential property; LTV limits 80% to 95%.2 | 30-year fully amortizing; fixed-rate dominates in the US.27 | Low; long-term fixed structures eliminate maturity risk. | Medium; sensitive to home prices but insulated from direct refinancing pressure. |
| **Venture-Backed Startup** | Future equity funding expectations; revenue run-rate.45 | Intellectual property (IP); cash balances held in custody.46 | Warrants; strict cash-burn covenants and milestone-based tranches.45 | Extreme; relies on sequential VC priced funding rounds.45 | Very High; tied directly to equity valuations and exit windows.45 |

## **Shadow Banking, Collateral Plumbing, and the Bank–Nonbank Nexus**

As regulatory capital constraints have tightened the perimeter of traditional commercial banking under Basel III, financial intermediation has migrated toward Non-Bank Financial Intermediation (NBFI)—commonly referred to as shadow banking.38 The shadow banking system does not rely on state-backed retail deposits; instead, it matches credit demand with investor capital through wholesale funding markets, securitized vehicles, and collateral-backed credit chains.24

### **Collateral Plumbing: The Repo Market and Collateral Chains**

The primary liquidity engine of the shadow banking system is the repurchase agreement (repo) market.23 Repo functions as a collateralized loan where a borrower sells a security (typically a government bond or high-grade corporate asset) to a lender with a simultaneous agreement to buy it back at a premium on a future date.23 The difference between the asset's market value and the cash lent is the **haircut**, which reflects the collateral's liquidity and credit risk.24

Cash Lent \= Market Value of Collateral \* (1 \- Haircut) 25

The global sovereign repo market exceeds 16 trillion USD in outstanding trades, acting as the foundational pricing mechanism for financial system leverage.23 A critical feature of this market is the **rehypothecation** or reuse of collateral.23 A single Treasury bond can be pledged, received, and re-pledged multiple times across a chain of intermediaries to support multiple leverage transactions 23:

Prime Broker \--\> Hedge Fund \--\> MMF \--\> Securities Lending \--\> Dealer

These collateral chains are highly efficient during liquidity booms, but they create severe systemic fragility.23 Because repo and Credit Default Swaps (CDS) possess a privileged "safe harbor" status in bankruptcy—meaning they are exempt from the automatic stay that freezes assets during insolvency—creditors can immediately seize and liquidate collateral during a counterparty default.24

This legal privilege can trigger a self-reinforcing liquidation spiral: a minor drop in asset values prompts lenders to raise haircuts, forcing leveraged entities to sell assets to meet margin calls, which drives prices down further and triggers systemic margin spirals.23

### **The Bank-Nonbank Intermediation Model**

Rather than operating in isolation, banks and NBFIs have formed a deeply interconnected, symbiotic relationship.38 The structural division of labor highlights a fundamental risk asymmetry: **credit risk has migrated to NBFIs, while liquidity risk remains concentrated in the banking system**.51

                    ┌─────────────────────────┐  
                    │      Regulated Core     │  
                    │    (G-SIBs and Banks)   │  
                    └────────────┬────────────┘  
                                 │  
                                 │ Senior Debt / Credit Lines  
                                 ▼  
                    ┌─────────────────────────┐  
                    │       NBFI Sector       │  
             (Private Credit, Pension Funds, Insurers, CLOs, MMFs)  
                    └────────────┬────────────┘  
                                 │  
                                 │ Junior Credit / Direct Lending  
                                 ▼  
                        ┌─────────────────┐  
                        │  Real Economy   │  
                        │    Borrowers    │  
                        └─────────────────┘

Under this structure, NBFIs hold riskier, junior credit exposures (e.g., leveraged loans, private corporate debt, structured products).36 However, NBFIs are not self-funded; they depend on senior credit facilities, subscription lines, and liquidity guarantees provided by G-SIBs and large commercial banks.30

When macroeconomic conditions deteriorate or asset values fall, NBFIs draw down these bank-provided credit lines to defend their positions, shifting the liquidity shock back onto the regulated banking sector's balance sheet.39

### **Bank–Nonbank Intermediation Map**

The table below maps the structural flow of credit risk, assets, and liquidity linkages across key financial entities.

| Intermediary Entity | Core Credit Assets | Primary Funding Source | Regulatory Capital/Risk Constraints | Banking System Credit/Liquidity Link |
| :---- | :---- | :---- | :---- | :---- |
| **Commercial Bank** | Mortgages, consumer credit, corporate loans, HQLA.9 | Insured and uninsured deposits, wholesale debt.5 | CET1, Leverage Ratio, LCR, NSFR constraints.7 | Direct account holder at the central bank wholesale ledger.1 |
| **Broker-Dealer** | Market-making inventories, derivative collateral.7 | Repo funding, parent bank advances.24 | Net Capital Rule, haircut requirements on non-cleared positions.26 | Prime brokerage lending, intraday liquidity clearing agreements.39 |
| **Money Market Fund (MMF)** | Short-term Treasury bills, commercial paper, repo.24 | Retail and institutional investor shares.4 | Strict SEC 2a-7 rules on asset maturity and liquidity.24 | Repo counterparty to major banks; deposit holder at banks.4 |
| **Insurance Company** | Corporate bonds, real estate debt, structured credit.32 | Policy premiums, annuity liabilities.32 | Risk-Based Capital (RBC) requirements; rating dependency.7 | LP commitments to private credit; buyers of securitized bank debt.36 |
| **Pension Fund** | Long-duration bonds, equities, private assets.32 | Future beneficiary liabilities. | Long-term liability matching constraints. | LP commitments to private credit; buyers of securitized bank debt.36 |
| **Hedge Fund** | Long/short equities, sovereign debt, derivatives.50 | Prime brokerage leverage, investor equity.23 | Margin requirements; prime brokerage house limits.23 | Repo funding borrower; derivative counterparty to G-SIBs.7 |
| **Private Credit Fund** | Direct middle-market senior and unitranche loans.38 | Closed-end LP capital commitments.38 | No direct bank capital constraints; locked-up capital structures.52 | Subscription credit lines, NAV financing facilities.30 |
| **Securitization Vehicle (SPV)** | Asset pools (mortgages, auto loans, credit cards).24 | Tiered notes (senior to equity tranches).24 | Structural rating-agency requirements.30 | Bank warehousing credit lines; bank purchases of AAA senior tranches.36 |
| **Finance Company** | Consumer auto loans, equipment leases, small-biz loans.29 | Commercial paper, securitization, bank credit lines.24 | Asset-to-liability covenants in wholesale funding agreements. | Bank corporate credit lines; direct asset sales to bank books.29 |
| **Fintech Lender** | Point-of-sale consumer debt, short-term BNPL.54 | Bank warehouse facilities, securitization.30 | Partner bank compliance standards.54 | Bank originator partnerships; warehouse debt financing.30 |

## **Corporate Debt Markets, Private Credit, and Working Capital Routing**

The corporate financing landscape is divided into three major categories based on firm size, credit ratings, and capital market access 29:

Large Investment-Grade Corporates (Public Bonds) \<--\> Leveraged / High-Yield Corporates (BSL / CLOs) \<--\> Middle-Market / Private Firms (Private Credit)

### **The Syndicated and Leveraged Loan Markets**

Broadly Syndicated Loans (BSLs) are large commercial loans structured by an arranging bank and distributed to a syndicate of institutional investors, primarily Collateralized Loan Obligations (CLOs), mutual funds, and insurance companies.36 Leveraged loans—corporate debt extended to borrowers with high leverage profiles and credit ratings below BB+—represent the raw material for CLOs, which purchase up to 60-70% of new syndicated issuances.36

As central banks raised interest rates in 2022–2023, the floating-rate structure of these loans caused immediate borrower interest expenses to rise, compressing cash-flow cushions and driving rating downgrades and default rates upward.36

### **The Private Credit Channel**

The expansion of **private credit** (non-bank direct lending to mid-sized businesses) has fundamentally transformed corporate capital routing, reaching an estimated 1.5 to 2.0 trillion USD globally at the end of 2024\.38

This expansion is structurally linked to regulatory arbitrage.30 As Basel III capital requirements raised the risk weights on banks' leveraged loan holdings, banks withdrew from middle-market lending, leaving private credit funds to fill the gap.29

### **The Competing Views on Private Credit Risk**

The systemic implications of private credit's growth are a subject of ongoing debate among financial stability authorities and market participants:

* **The Stabilizing View**: Proponents argue that private credit enhances systemic stability because it is funded by long-term, closed-end LP commitments (e.g., from pensions and endowments) that cannot be withdrawn on demand.38 This locked-up capital eliminates classic bank-run risks.52 Furthermore, because private credit loans are negotiated bilaterally, managers can easily restructure debt terms and work directly with distressed borrowers, avoiding costly public bankruptcy liquidations.38  
* **The Systemic Risk View**: Critics and regulators point out that private credit is characterized by significant valuation opacity and a lack of public disclosure.52 Loans are marked-to-model rather than marked-to-market, which hides credit deterioration.52 Furthermore, private credit borrowers are typically highly leveraged, with lower credit quality than public corporate bond issuers.52

The systemic link to banks is not severed but transformed: banks provide massive subscription lines and NAV loans to private credit funds, which captured exposures ranging from 220 billion to 500 billion USD by late 2024\.30

Additionally, the widespread use of Payment-in-Kind (PIK) options—which allow borrowers to defer cash interest payments by adding them to the loan principal—hides emerging cash flow strains and delays necessary restructuring.37

### **Supply Chain and Working Capital Finance**

At the micro-level of global commerce, corporate capital routing depends on trade finance and working capital structures.57 According to the Asian Development Bank, the global trade finance gap—the unmet demand for trade-related financing—stands at 1.7 trillion USD, disproportionately impacting Small and Medium-sized Enterprises (SMEs).57

To optimize working capital, firms rely on two primary receivables-based structures 16:

1. **Factoring**: A seller-led arrangement where an SME supplier sells its accounts receivable to a financial institution (the factor) at a discount to obtain immediate cash.16  
2. **Reverse Factoring (Payables Finance)**: A buyer-led program where a highly creditworthy corporate buyer partners with a bank or fintech platform to allow its suppliers to cash out their invoices early at a discount, based on the buyer's credit rating.16

This market has grown by over 30% annually, accelerated by digital blockchain platforms that reduce invoice processing delays by 47% and improve supplier survival rates by 32% during supply chain disruptions.57

## **Real Estate, Consumer Leverage, and Venture Capital Channels**

Credit allocation transmits macroeconomic shocks unevenly across commercial real estate, consumer credit, and venture capital, depending on the underwriting structures and funding channels of each sector.

### **Commercial Real Estate (CRE) Refinancing Friction**

The Commercial Real Estate (CRE) debt market, valued at 4.5 trillion USD in the United States, represents a highly interest-rate-sensitive credit channel.42 Approximately 1.2 trillion USD of this debt is scheduled to mature by the end of 2025, confronting borrowers with a major refinancing wall.42

The CRE transmission channel is driven by a structural misalignment between borrowing costs and collateral valuations 41:

Capitalization (Cap) Rate \= Net Operating Income (NOI) / Market Value of Property 40

When central banks raised interest rates rapidly in 2022–2023, risk-free bond yields surged, forcing cap rates higher to preserve the equity risk premium.40 Under stable or declining Net Operating Income (NOI)—particularly in the office sector, which has been hit by secular remote-work shifts—higher cap rates drove property valuations down, with global CRE prices declining by 12% to 23% in 2023\.40

When existing CRE loans mature, borrowers face an underwriting vise: the depreciated property value violates Loan-to-Value (LTV) limits, while higher interest rates compress Debt-Service Coverage Ratios (DSCR) below viable bank underwriting thresholds.40 This dynamics its smallest regional and community banks, which hold roughly 44% of their total loan portfolios in CRE debt, compared to just 13% for large multinational banks.42

### **Consumer Credit and Household Leverage Channels**

Unlike corporate or real estate borrowers, households convert wage income and liquid wealth directly into consumption through credit cards, auto loans, and fintech platforms.44 While credit card delinquency rates began to flatten in 2025 following a period of post-pandemic normalization, subprime borrowers and younger cohorts have faced mounting stress.44

A key innovation in retail credit is the proliferation of **Buy Now, Pay Later (BNPL)** products, dominated by fintech platforms.54 While BNPL "Pay-in-4" transactions represent a 70 billion USD market in 2025, the outstanding debt stock at any point is small (approximately 3.02 billion USD) due to rapid six-week amortization schedules.55

Nonetheless, BNPL represents a selective credit channel that bypasses traditional credit bureaus.54 BNPL underwriting relies on soft credit checks and automated transaction analysis.54 Consumers using these products exhibit higher rates of revolving credit card balances and are twice as likely to be delinquent on other debt obligations compared to non-users, indicating that BNPL functions as a credit facility of last resort for cash-strapped subprime households.61

### **Venture Capital and Startup Financing Architecture**

High-growth, non-revenue-generating startups rely on sequential capital injections rather than organic cash flow to survive.45 Startups typically secure early funding through unpriced **Simple Agreements for Future Equity (SAFEs)** or convertible notes, which defer formal valuation negotiations until a subsequent institutional priced equity round.45

Venture debt is then layered on top of this equity stack, typically structured as a loan equivalent to 20% to 35% of the preceding equity round, yielding 8% to 15% interest alongside equity warrants.46

When monetary policy tightens, this funding model is disrupted by the **denominator effect** 45:

Public Asset Correction \--\> LPs Over-Allocated to Private Equity/VC \--\> New Commitments Halted

As institutional LPs stop committing capital to venture funds, VC "dry powder" is hoarded rather than deployed.45 Startups face an abrupt contraction in priced equity rounds, leaving them unable to convert outstanding SAFEs or service fixed venture debt obligations.45

Because venture debt is typically structured with full recourse and strict cash-burn covenants, failures in the equity funding chain trigger rapid balance-sheet liquidations long before a startup's underlying technology or product has a chance to mature.45

### **Sectoral Capital Routing Matrix**

| Sector | Primary Funding Channel | Capital Allocation Constraint | Collateral Logic | Key Macro Trigger | Dominant Failure Mode |
| :---- | :---- | :---- | :---- | :---- | :---- |
| **Startups** | VC priced rounds, SAFEs, convertible notes, venture debt.45 | Refinancing exit liquidity; denominator effect on LPs.45 | IP, custody balances, warrant dilution upside.46 | Squeezed public valuations; higher risk-free yields.45 | Runway exhaustion; covenant breaches; liquidation of assets.45 |
| **Real Estate** | Commercial mortgages, construction/bridge loans, CMBS, REIT debt.41 | DSCR limits under high rates; cap rate expansions.40 | Physical real property appraised valuations.40 | Federal Funds rate hikes; commercial tenancy drops.40 | Refinancing failure at maturity; maturity defaults.41 |
| **Corporations** | syndicated BSLs, corporate bonds, trade/supplier lines, private credit.36 | Leverage multipliers (Debt/EBITDA); margin requirements.36 | Senior secured liens on global enterprise assets.36 | Sovereign credit spread widening; rising cost of debt.36 | Debt rating downgrades; restructuring under bankruptcy.36 |
| **Households** | Fixed-rate mortgages, credit cards, auto loans, BNPL.44 | Household debt-to-income; wage stability.44 | Residential real property; vehicle titling.2 | Real wage compression; spikes in unemployment.44 | Serious delinquencies; vehicle repos; retail defaults.44 |
| **Sovereigns** | Government Treasury bonds, sovereign reserve managers.33 | Primary fiscal balance; sovereign bond yields.32 | None (backed by national tax base and sovereign money power).32 | Spikes in domestic inflation; real rate hikes.32 | Sovereign-bank doom loop; sovereign currency crises.64 |
| **Speculative Assets** | Margin loans, dealer repos, prime broker credit.23 | Daily volatility metrics; haircut requirements.23 | High-beta equities, structured debt tranches, crypto.23 | Spikes in asset price volatility; global risk-off.23 | Self-reinforcing collateral liquidations; margin spirals.23 |
| **Supply Chains** | Working capital lines, factoring, reverse factoring.16 | Anchor buyer's credit rating and invoice approvals.16 | Verified accounts receivable invoices.16 | Spikes in trade-financing spreads; global tariffs.37 | Cash conversion cycle lockup; SME supplier insolvencies.57 |

## **Sovereign-Bank Entanglement, Fiscal Dominance, and Central Bank Backstops**

The commercial banking system is structurally entangled with sovereign fiscal operations, creating a mutual dependency known as the **sovereign-bank nexus**.32 Government bonds function as risk-free collateral that supports private credit creation, serves as HQLA for bank liquidity compliance, and acts as the primary tool for central bank monetary intervention.9

In return, the domestic commercial banking sector serves as a captive buyer of government debt, absorbing fiscal issuance during times of stress.32

### **The Sovereign-Bank Doom Loop**

The sovereign-bank nexus can mutate into a destructive feedback loop—historically referred to as the "doom loop"—via two distinct transmission vectors 64:

Sovereign Risk Rises ──► Sovereign Bond Yields Spike ──► Bank Assets Depreciate  
                                                             │  
                                                             ▼  
Fiscal Bailouts Impaired ◄── Bank Solvency Stress ◄──────────┘

Bank Solvency Stress ──► Fiscal Bailouts Required ──► Sovereign Risk Rises   
                                                             │  
                                                             ▼  
Bank Assets Depreciate ◄── Sovereign Bond Yields Spike ◄─────┘

1. **The Sovereign Contagion Vector**: In highly indebted nations, market concerns over fiscal sustainability drive sovereign bond yields up and bond prices down.32 Because domestic commercial banks hold concentrated positions in home-country sovereign debt—often exceeding 60% of their regulatory capital—the resulting mark-to-market capital losses damage bank solvency, contracting credit supply and weakening the domestic economy.32  
2. **The Banking Contagion Vector**: Conversely, a systemic banking crisis triggered by private credit or real estate defaults can force the sovereign to deploy massive fiscal resources, deposit guarantees, and bank recapitalizations.64 This sudden expansion of contingent sovereign liabilities damages the state’s fiscal position, causing sovereign bond yields to spike and initiating a downward economic spiral.32

This fragility is exacerbated by international bank regulations.32 Under current Basel Committee rules, national regulators are permitted to apply a **0% risk weight** to sovereign debt denominated and funded in the domestic currency, regardless of the sovereign's actual credit risk.32

This regulatory exemption incentivizes banks to hoard massive portfolios of domestic government bonds, bypassing concentration limits and reinforcing the systemic risk-sharing link between the state and the private banking system.32

### **Central Bank Liquidity Backstops: Discount Window and BTFP**

To interrupt liquidity-driven bank runs, central banks operate standing lender-of-last-resort facilities.6 However, traditional tools are often constrained by structural inefficiencies:

* **The Discount Window (DW)**: The classic central bank tool requires banks to preposition eligible collateral (valued at market value minus a haircut) to secure short-term primary credit.13 However, the DW is severely hampered by **borrowing stigma**.22 Banks fear that accessing the window signals financial weakness to rating agencies and counterparties, leading them to pay above-market rates for alternative wholesale funds rather than utilize the facility.22  
* **The Bank Term Funding Program (BTFP)**: In response to the March 2023 banking stress, the Federal Reserve established the BTFP under its Section 13(3) emergency powers.11 Unlike the DW, the BTFP offered primary credit loans up to one year, priced at the one-year OIS rate plus 10 basis points, with eligible collateral (U.S. Treasuries, agency debt, and MBS) valued at **par (face value)** rather than fair market value.11

This par valuation transfered significant interest rate risk to the public balance sheet.14 In late 2023, with bank investment portfolios on average 20% underwater due to rate hikes, the BTFP was effectively providing undercollateralized loans.5 The aggregate undercollateralization shortfall reached over 20 billion USD.15

Upon the failure of First Republic Bank, the FDIC assumed its BTFP debt, shifting approximately 3 billion USD in costs—which should have been absorbed by the Treasury under its Exchange Stabilization Fund (ESF) backstop—onto the banking system’s Deposit Insurance Fund (DIF).13

This dynamic highlights how emergency facilities designed to stabilize banking assets can create severe moral hazard, reducing bank incentives to self-insure against interest rate and liquidity risks.13

## **The Leverage Cycle, Minskyan Transitions, and Causal Intermediation**

The global financial system does not maintain a static posture toward risk; rather, it is characterized by endogenous credit cycles that amplify macroeconomic trends. This is the **leverage cycle**.35

### **The Mechanics of the Leverage Cycle**

The leverage cycle is driven by the dynamic interaction of asset valuations, collateral requirements, and risk tolerances.35 During macroeconomic expansions, rising asset values increase the value of pledged collateral.35 This appreciation prompts cash lenders in wholesale markets to lower haircut requirements, allowing borrowers to secure more funding against the same volume of assets.24

This credit expansion supports additional asset purchases, driving valuations higher, validating loose underwriting assumptions, and compressing risk spreads in a self-reinforcing upward spiral.23

Asset Valuations Up \--\> Collateral Appraisals Up \--\> Repo Haircuts Down \--\> Credit Availability Up \--\> Asset Demand Up

The cycle reverses when a macroeconomic shock—such as a monetary tightening cycle—raises borrowing costs and depresses asset valuations.20 As collateral values fall, cash lenders in repo and wholesale markets raise haircuts to protect their capital.24

This spike in haircuts forces leveraged borrowers to liquidate asset portfolios to meet margin calls, driving prices down further and triggering systemic margin spirals.23

Asset Valuations Down \--\> Collateral Appraisals Down \--\> Repo Haircuts Up \--\> Margin Calls Up \--\> Forced Asset Sales Up

### **Integrating Minskyan Postures with Modern Regulation**

This leverage cycle can be mapped directly to Hyman Minsky’s three financial postures—**hedge**, **speculative**, and **Ponzi**—integrated with modern regulatory constraints and private credit channels 35:

1. **Hedge Finance**: Under hedge finance, a borrower’s expected cash flows are sufficient to meet all contractual obligations, covering both principal repayments and interest expenses.66 In the modern banking book, hedge positions are represented by prime corporate borrowers, fully amortizing consumer mortgages, and well-covered commercial loans.27 These assets are heavily favored by bank capital regulations, receiving low regulatory risk weights under Basel III.7  
2. **Speculative Finance**: A speculative borrower has expected cash flows sufficient to meet interest payments but insufficient to repay the outstanding principal balance at maturity.66 The borrower depends on wholesale market liquidity to continuously roll over its debt obligations.24  
   In the modern macroeconomy, speculative finance is the dominant posture of Commercial Real Estate (CRE) portfolios, broadly syndicated leveraged loans, and revolving corporate credit facilities.36  
   As Basel III capital and liquidity rules (such as LCR and NSFR) raised the cost for banks to warehouse these roll-over exposures, speculative finance increasingly migrated toward private credit and NBFI structures.9  
3. **Ponzi Finance**: Under Ponzi finance, a borrower’s expected cash flows are insufficient to pay either principal or interest.66 The borrower depends entirely on rising asset valuations to secure more debt or sell assets at a gain to meet its liabilities.66  
   In the modern intermediation landscape, Ponzi structures are represented by early-stage venture-backed startups (which rely on sequential priced rounds to fund operating burn) and highly leveraged corporate borrowers utilizing Payment-in-Kind (PIK) deferral features in the private credit market.37  
   Because these positions violate traditional bank underwriting and leverage constraints, they are routed entirely through non-bank financial intermediaries, relying on bank-provided subscription and warehouse credit lines to maintain their funding plumbing.30

### **Leverage Cycle Atlas**

The table below outlines the behavioral characteristics of the leverage cycle across its key phases.

| Phase of the Leverage Cycle | Collateral & Haircut Dynamics | Underwriting & Covenant Behavior | Intermediary Balance-Sheet Portfolios | Real Economy Credit Transmission |
| :---- | :---- | :---- | :---- | :---- |
| **I. Expansionary Boom** | High collateral appraisals; repo haircuts compress toward zero.23 | Standards loosen; covenant-lite structures dominate; cash-flow metrics rely on pro-forma assumptions.36 | Banks expand senior credit lines to NBFIs; private credit funds aggressively deploy capital.38 | Rapid capital deployment to high-beta sectors, real estate, and leveraged corporates.27 |
| **II. Over-Extension / Peak** | Hidden leverage builds via multi-layered NAV loans and synthetic risk transfers.37 | Covenant-free structures peak; PIK interest terms are widely accepted to artificially defer defaults.37 | Portfolios are highly concentrated in tech, CRE, and leveraged loans.43 | Asset pricing reaches peak valuations; refinancing dependencies are high.42 |
| **III. Deleveraging Shock** | Volatility triggers collateral depreciations and spikes in repo haircuts.24 | Standards tighten abruptly; banks restrict credit lines and demand strict maintenance covenants.20 | NBFIs draw down bank credit commitments, transferring liquidity stress back to regulated banks.39 | Borrowers face refinancing hurdles; asset fire sales and insolvencies begin.24 |
| **IV. Systemic Trough** | Haircuts remain elevated; collateral chains contract due to counterparty hoarding.23 | Traditional lending is limited to highly rated sovereigns and prime borrowers with strong cash flows.7 | Balance sheets are repaired via loan-loss provisions, asset write-offs, and capital conservation.1 | Capital starvation in high-risk sectors; economic activity slows down.8 |

## **The Credit Allocation Constraint Model**

To analyze how credit is routed under changing macroeconomic regimes, we construct a conceptual **Credit Allocation Constraint Model**:

Ac \= f(Db, Cs, Fc, Kr, Vc, Ecf, Rt, Lx, Bp)

Where:

* **Ac (Credit Allocation)**: The volume and pricing of credit directed to a specific economic sector.  
* **Db (Borrower Demand)**: Highly sensitive to nominal growth expectations, operating margins, and current policy rates.20  
* **Cs (Lender Balance-Sheet Capacity)**: Constrained by historical loan-loss provisions, asset write-offs, and portfolio concentration limits.1  
* **Fc (Funding Cost)**: Shaped by deposit beta dynamics, MMF competition, and the cost of wholesale borrowing.5  
* **Kr (Regulatory Capital Requirement)**: Defined by risk weights, leverage ratios, and capital conservation buffers.7  
* **Vc (Collateral Value)**: Dependent on continuous asset appraisals, cap rates, and market liquidity.40  
* **Ecf (Expected Cash Flow)**: Projections of borrower income relative to interest rate structures (fixed vs. floating).36  
* **Rt (Regulatory Treatment)**: Rules governing specific assets, such as LCR runoff assumptions and accounting rules for unrealized losses.7  
* **Lx (Exit Liquidity)**: The capacity of secondary markets, securitization channels, and IPO windows to absorb debt or equity assets.30  
* **Bp (Political or Institutional Backstop)**: The availability of emergency facilities, deposit guarantees, and state bailouts.6

### **Sectoral Failures Under the Credit Allocation Model**

Under this diagnostic model, different economic sectors fail specific terms during a tightening cycle:

* **Venture-Backed Startups** fail the expected cash-flow (Ecf) and exit-liquidity (Lx) tests.45 Because startups run on negative operational cash flows, their survival depends on sequential refinancing through IPOs or priced venture capital rounds.45 When risk-free rates rise, compressing venture valuations, these exit windows close, leading to runway exhaustion and venture capital contraction.45  
* **Commercial Real Estate (CRE)** fails the collateral valuation (Vc) and refinancing (Lx) tests.41 Spikes in cap rates depress property values, violating regulatory LTV constraints and preventing regional banks from refinancing maturing debts, regardless of the borrower's historical interest-only payment record.40  
* **Subprime Households** fail the expected cash-flow (Ecf) and regulatory capital (Kr) tests.7 High inflation and interest rates reduce disposable wages relative to debt payments.44 Banks, facing tighter regulatory requirements, raise risk-pricing spreads and tighten credit standards, pushing these households toward higher-cost, non-bank payday loans and fintech BNPL products.54  
* **Weak Sovereigns** fail the funding cost (Fc) and political backstop (Bp) tests.32 In a monetary union without a unified fiscal authority (e.g., the Eurozone), highly indebted sovereigns lack a direct monetary backstop, leaving their domestic bond yields vulnerable to capital flight and exposing the banking book to sovereign-bank contagion.32  
* **Speculative Assets** fail the collateral valuation (Vc) and haircut (Hr) tests.23 Because these positions are funded through overnight repo markets and prime brokerage margin lines, a sudden spike in asset volatility causes lenders to raise haircuts.23 This change triggers immediate margin calls, forcing liquidations in a contracting liquidity spiral.23

## **Epistemological Disputes and Intermediation Controversies**

Banking and financial intermediation theory is characterized by several fundamental disputes over the mechanics of credit creation, safety, and systemic stability.

### **I. Loanable-Funds Imagery vs. Endogenous Credit Creation**

The classical loanable-funds model posits that banks are passive intermediaries that collect deposits from savers and lend them out to borrowers, meaning credit volume is constrained by prior saving.2 Proponents of this view argue that central banks can control credit expansion through the reserve multiplier.2

The endogenous credit creation theory, verified by central bank research, shows that commercial banks create deposits in the act of lending, meaning credit volume is constrained by bank risk tolerance, funding costs, and capital requirements rather than prior reserves.1

The loanable-funds view persists in many standard economic models because it simplifies general equilibrium calculations, but it fails to explain the rapid expansion of bank balance sheets during liquidity booms.2

### **II. Bank Capital Constraints vs. Reserve Constraints**

A long-standing debate centers on whether bank lending is constrained by capital adequacy ratios (e.g., CET1) or by the quantity of central bank reserves.2 Under abundant reserve regimes (post-QE), reserves are supplied on-demand by central banks, making reserve levels irrelevant as a direct constraint on loan volume.2

Consequently, regulatory capital requirements function as the primary constraint on credit allocation, since banks must hold loss-absorbing equity against every new loan based on its risk weight.1

However, during monetary tightening cycles, reserve constraints can re-emerge for specific institutions if rapid deposit outflows force them to deplete their reserves, leaving them dependent on expensive wholesale borrowing.5

### **III. Relationship Banking vs. Market-Based Finance**

Relationship banking is characterized by long-term, bilateral connections where banks leverage soft, non-public information to monitor local borrowers and customize debt terms.39 Market-based finance routes credit through standardized, public debt markets (e.g., corporate bonds and commercial paper).24

Proponents of relationship banking argue that it stabilizes credit access during downturns because lenders are more willing to support troubled borrowers.39 Proponents of market-based finance argue that it is more efficient, reducing borrowing costs through continuous price discovery and liquid secondary trading.24

However, market-based finance is highly cyclical, prone to sudden liquidity freezes during market stress.29

### **IV. Bank Regulation as Safety vs. Credit Migration Engine**

The Basel Committee on Banking Supervision designs bank capital and liquidity regulations to enhance the safety and soundness of the regulated banking sector.7

However, critics argue that aggressive bank regulation acts as a credit migration engine.30 By raising the capital cost of high-yield commercial lending and leveraged loans, regulation does not eliminate credit risk; instead, it pushes riskier credit activities outside the regulatory perimeter into more opaque, less-regulated shadow banking and private credit sectors.30

This migration makes the overall financial system harder to monitor and govern during a crisis.52

### **V. Private Credit: Lock-Up Stability vs. Opaque Systemic Risk**

The rapid growth of the private credit market has split opinion on its systemic risks.38

Supporters emphasize its locked-up LP capital structures, which insulate funds from investor runs and allow managers to act as patient capital during downturns.38

Critics highlight the extreme opacity of private credit portfolios, the reliance on quarterly mark-to-model valuations, the growing use of PIK deferrals to hide borrower distress, and the deep, hidden leverage linkages with systemic banks through subscription and NAV credit lines.30

### **VI. Securitization: Risk Distribution vs. Fragility Amplifier**

Securitization—the pooling of illiquid loans to issue structured securities—is historically promoted as an efficient mechanism for distributing credit risk away from banks' balance sheets to global capital market investors.24

However, the 2008 financial crisis demonstrated that securitization can amplify systemic fragility.7 It creates asymmetric information along the underwriting chain, disincentivizes loan originators from conducting proper due diligence, and constructs highly complex, leveraged collateral networks (e.g., CDOs and CLOs) that can fail abruptly during asset corrections.24

### **VII. Shadow Banking: Efficient Intermediation vs. Regulatory Arbitrage**

Proponents of non-bank financial intermediation argue that shadow banking enhances economic efficiency by customizing credit solutions, lowering borrowing costs, and providing institutional investors with diverse yield-generating assets.38

Critics argue that shadow banking is fundamentally a vehicle for regulatory arbitrage, designed to evade the capital, liquidity, and consumer-protection rules imposed on traditional banks.30

This system remains dependent on the regulated banking sector for liquidity backstops and credit lines, meaning that shadow banking failures can still trigger systemic crises within the regulated core.39

### **VIII. Fintech Lending: Inclusion vs. Predatory Procyclicality**

Fintech and digital consumer lending platforms use real-time transaction data and automated underwriting algorithms to expand credit access to historically underserved or unbanked populations.29

However, critics argue that fintech platforms engage in predatory pricing, charge high fees, and foster procyclicality.54 Because fintech lenders do not have stable deposit franchises, they rely on warehouse credit lines and securitization markets to fund originations, meaning they must rapidly withdraw from lending during liquidity contractions, starving vulnerable households of credit.30

### **IX. Venture Finance: Innovation Engine vs. Liquidity-Dependent Speculation**

Venture capital is celebrated as the primary financial engine of technological innovation, providing risk-tolerant equity capital to early-stage startups that lack collateral or cash flows.45

Critics argue that venture finance has mutated into a liquidity-dependent speculative bubble.45 Startups are funded not by organic cash flow, but by sequential equity rounds priced at escalating valuations.45

This model relies on loose monetary policy and public IPO exit windows.45 When monetary policy tightens, the entire funding stack can collapse, revealing that many startups are structurally unviable Ponzi schemes.45

## **Banking and Credit Ontology Registry**

* **Commercial Bank**: A licensed financial depository institution authorized to endogenously create broad money through credit expansion while providing clearing, payment, and settlement services within the central bank wholesale ledger network.1  
* **Deposit Creation**: The process by which a commercial bank expands its balance sheet by crediting a borrower's account with a demand-executable liability (deposit) in exchange for a loan asset, thereby expanding the broad money supply.1  
* **Loan Origination**: The administrative, underwriting, and credit-scoring process through which a lender evaluates a borrower, establishes credit terms, and records a new loan on its balance sheet.1  
* **Reserve Settlement**: The process of clearing and settling transaction balances between commercial banks through the transfer of central bank reserves on the central bank's wholesale ledger.1  
* **Interbank Funding**: The wholesale money market network through which commercial banks borrow and lend central bank reserves and other liquid assets, overnight or at short maturities, to manage settlement balances and meet regulatory requirements.4  
* **Maturity Transformation**: The structural process of funding long-term, illiquid, and risky assets with short-term, highly liquid liabilities, creating economic value while exposing the institution to liquidity mismatch and run risk.24  
* **Duration Mismatch**: The risk exposure arising when the weighted average maturity of an institution's assets exceeds the maturity of its liabilities, leaving it vulnerable to capital losses when interest rates rise.5  
* **Liquidity Mismatch**: A structural vulnerability where an institution's liabilities can be withdrawn on demand or at short notice, while its assets are highly illiquid and cannot be quickly monetized during stress.9  
* **Deposit Beta**: The percentage of a change in a central bank's policy rate that a bank passes through to its deposit pricing, determining interest expenses and deposit franchise value.17  
* **Uninsured Deposit**: A deposit account balance that exceeds statutory insurance limits (e.g., 250,000 USD in the US), making it highly sensitive to bank credit risk and vulnerable to sudden runs.6  
* **Wholesale Funding**: Non-deposit wholesale liabilities used by banks to fund assets, including repos, commercial paper, interbank borrowing, and FHLB advances.5  
* **HQLA (High-Quality Liquid Assets)**: Unencumbered liquid assets (primarily central bank reserves and sovereign debt) that can be easily and immediately converted into cash in financial markets under stress.7  
* **Regulatory Capital**: The loss-absorbing capital cushion (such as Common Equity Tier 1, Additional Tier 1, or Tier 2 capital) that banks are required to maintain under macroprudential frameworks to ensure solvency.7  
* **Risk-Weighted Asset (RWA)**: A bank's assets and off-balance-sheet exposures multiplied by a regulatory risk factor that reflects credit, market, and operational risks.7  
* **Loan-Loss Provision**: A non-cash expense set aside by banks to account for expected credit losses on their loan portfolios, reducing net income and capital ex-ante.5  
* **Underwriting Standard**: The criteria, metrics, and risk limits established by a lender to govern the approval and pricing of loans.20  
* **Covenant**: A legally binding clause in a loan agreement requiring the borrower to meet specific performance targets (maintenance covenant) or restricting certain actions (incurrence covenant).30  
* **LTV (Loan-to-Value)**: The ratio of a loan's principal balance to the appraised market value of the collateral asset, functioning as a primary risk constraint.40  
* **DSCR (Debt-Service Coverage Ratio)**: The ratio of a borrower's operating cash flow or Net Operating Income (NOI) to its total debt-service obligations (principal and interest payments).36  
* **Credit Spread**: The difference in yield between a risky debt instrument and a risk-free benchmark asset (such as a Treasury bond) of equivalent maturity, reflecting the credit risk premium.36  
* **Revolving Credit Facility (RCF)**: A flexible credit line provided by banks that allows a borrower to draw down, repay, and re-draw funds up to a set limit over the facility's life.36  
* **Securitization**: The structural process of pooling illiquid assets (such as residential mortgages or auto loans) and issuing tiered, interest-bearing securities backed by those underlying cash flows.24  
* **Repo Funding**: Secured short-term funding obtained by selling securities to cash lenders with a simultaneous agreement to buy them back at a premium on a future date.23  
* **Shadow Banking**: Credit intermediation involving entities and activities outside the traditional, regulated banking perimeter that do not have direct access to central bank standing facilities or public safety nets.24  
* **NBFI (Non-Bank Financial Intermediation)**: The institutional sector comprising asset managers, pension funds, insurers, hedge funds, private credit funds, and finance companies that route capital outside of commercial banking licenses.23  
* **Private Credit**: Direct, bilaterally negotiated lending to non-publicly traded medium-sized or leveraged companies provided by non-bank asset managers.38  
* **Direct Lending**: A key segment of the private credit market where a non-bank lender originates loans directly to a corporate borrower without a financial intermediary.38  
* **Syndicated Loan**: A large commercial loan funded by a group of financial institutions (the syndicate) and managed by one or more lead originating banks.29  
* **Leveraged Loan**: A syndicated or corporate loan extended to a highly indebted borrower, typically rated BB+ or lower, with debt multiples exceeding standard regulatory limits.29  
* **High-Yield Bond**: A publicly traded, fixed-income security issued by a corporate borrower with a credit rating below investment grade (BB+ or lower), offering higher yields to offset default risk.36  
* **Trade Credit**: A business-to-business credit arrangement where a supplier allows a buyer to delay payment for goods or services for an agreed period (e.g., 30, 60, or 90 days).16  
* **Factoring**: A working capital financing technique where a business sells its accounts receivable to a third-party financier (the factor) at a discount to obtain immediate liquidity.16  
* **Mortgage Securitization**: The pooling of residential or commercial mortgages to issue mortgage-backed securities (MBS) to capital market investors.7  
* **CRE Refinancing Risk**: The vulnerability CRE borrowers face when their loans mature during high-rate or low-valuation regimes, making it difficult to secure a replacement loan.41  
* **Venture Debt**: A specialized form of debt financing provided to venture-backed, high-growth startups to extend runway between equity fundraising rounds.45  
* **LP Commitment**: The legally binding capital contribution that a Limited Partner agrees to provide to a private equity or venture capital fund over its investment period.30  
* **Denominator Effect**: A portfolio distortion that occurs when a sharp drop in public equity prices increases the percentage share of private equity and venture capital holdings in institutional portfolios, forcing LPs to halt new private commitments.45  
* **Prime Brokerage**: A suite of specialized services—including leveraged financing, securities lending, custody, and clearing—provided by investment banks to hedge funds and other institutional investors.23  
* **Margin Lending**: The provision of leverage secured by the borrower’s investment portfolio, subject to immediate margin calls and liquidations if the collateral value falls below maintenance thresholds.23  
* **Sovereign-Bank Nexus**: The deep, structural financial relationship between a sovereign state and its domestic commercial banking sector, where banks hold significant sovereign debt while relying on the state for fiscal backstops.32  
* **Credit Impulse**: The rate of change in the creation of new credit as a percentage of GDP, functioning as a leading indicator of macroeconomic growth and asset price momentum.

## **Applied Handoff to Report G: Asset Pricing Regimes & Cross-Market Liquidity Transmission**

This report's exploration of credit creation and capital distribution provides the structural foundation for **Report G: Asset Pricing Regimes & Cross-Market Liquidity Transmission**. To maintain analytical continuity across the Macro-KB, Report G must inherit and expand upon several core concepts:

1. **Leverage as Asset-Demand Fuel**: Report G should treat asset prices not merely as discounted cash flows, but as credit-allocation regimes.24 Systemic leverage, generated via repo rehypothecation and bank-provided prime brokerage lines, directly fuels asset-demand curves.23  
2. **The Bank-Nonbank Nexus as a Liquidity Conduit**: Report G must incorporate the structural risk asymmetry defined in Report F.51 When asset markets correct, credit risk remains with the NBFIs, but liquidity risk is transferred back to the banking perimeter as funds draw down committed credit lines.39  
3. **Refinancing Walls as Valuation Triggers**: The corporate and CRE refinancing walls (such as the 1.2 trillion USD in maturing CRE debt) must be treated in Report G as the primary triggers that convert book-value appraisal lags into realized market prices.41  
4. **Private Credit Opacity as Valuation Lag**: The quarterly model-based marks used in private credit hide emerging credit distress.52 Report G should utilize this pricing lag to analyze the valuation divergence between public and private asset classes during macroeconomic transitions.52  
5. **Sovereign Bonds as the Collateral Anchor**: Because sovereign government debt functions as the foundational risk-free collateral for repo markets and bank HQLA portfolios, fluctuations in sovereign yields directly alter the borrowing capacity and discount rates applied to all downstream financial assets.9

Through these inherited channels, Report G will demonstrate how changes in the credit-allocation machinery are transmitted across global financial markets, shaping asset-pricing regimes and cross-market liquidity.

#### **Works cited**

1. Credit Creation Theory of Banking \- The Economics Network, accessed May 11, 2026, [https://www.economicsnetwork.ac.uk/archive/starkey\_banking/](https://www.economicsnetwork.ac.uk/archive/starkey_banking/)  
2. Money creation in the modern economy \- Bank of England, accessed May 11, 2026, [https://www.bankofengland.co.uk/-/media/boe/files/quarterly-bulletin/2014/money-creation-in-the-modern-economy](https://www.bankofengland.co.uk/-/media/boe/files/quarterly-bulletin/2014/money-creation-in-the-modern-economy)  
3. Towards an institutional “landscape” view of modern money creation mechanisms and some reflections on their ecological significance \- PMC, accessed May 11, 2026, [https://pmc.ncbi.nlm.nih.gov/articles/PMC10064958/](https://pmc.ncbi.nlm.nih.gov/articles/PMC10064958/)  
4. Endorsing the Money-Creation View of Banking \- Rethinking Economics, accessed May 11, 2026, [https://rethinkeconomics.org/journal/endorsing-the-money-creation-view-of-banking/](https://rethinkeconomics.org/journal/endorsing-the-money-creation-view-of-banking/)  
5. 2023 Risk Review Section 4 | FDIC, accessed May 11, 2026, [https://www.fdic.gov/analysis/risk-review/2023-risk-review/2023-risk-review-section-4.pdf](https://www.fdic.gov/analysis/risk-review/2023-risk-review/2023-risk-review-section-4.pdf)  
6. Bank Funding and FHLB Advances \- Federal Reserve Bank of Kansas City, accessed May 11, 2026, [https://www.kansascityfed.org/research/economic-bulletin/bank-funding-and-fhlb-advances/](https://www.kansascityfed.org/research/economic-bulletin/bank-funding-and-fhlb-advances/)  
7. Basel III \- Wikipedia, accessed May 11, 2026, [https://en.wikipedia.org/wiki/Basel\_III](https://en.wikipedia.org/wiki/Basel_III)  
8. The Upside-Down World of the Liquidity Coverage Ratio: Some Unpleasant Arithmetic, accessed May 11, 2026, [https://bpi.com/the-upside-down-world-of-the-liquidity-coverage-ratio-some-unpleasant-arithmetic/](https://bpi.com/the-upside-down-world-of-the-liquidity-coverage-ratio-some-unpleasant-arithmetic/)  
9. LCR and NSFR, banks' liquidity shield \- BBVA, accessed May 11, 2026, [https://www.bbva.com/en/economy-and-finance/lcr-and-nsfr-what-do-these-liquidity-ratios-stand-for/](https://www.bbva.com/en/economy-and-finance/lcr-and-nsfr-what-do-these-liquidity-ratios-stand-for/)  
10. GAO-26-107373, FEDERAL HOME LOAN BANKS: Role During Financial Stress and Members' Borrowing Trends and Outcomes, accessed May 11, 2026, [https://files.gao.gov/reports/GAO-26-107373/index.html](https://files.gao.gov/reports/GAO-26-107373/index.html)  
11. Emergency Lending and Moral Hazard \- FDIC, accessed May 11, 2026, [https://www.fdic.gov/center-financial-research/john-kandrac-presentation.pdf](https://www.fdic.gov/center-financial-research/john-kandrac-presentation.pdf)  
12. Bank Term Funding Program: Understanding Borrowing from the Federal Reserve Bank, accessed May 11, 2026, [https://www.hunton.com/blockchain-legal-resource/bank-term-funding-program-understanding-borrowing-from-the-federal-reserve-bank](https://www.hunton.com/blockchain-legal-resource/bank-term-funding-program-understanding-borrowing-from-the-federal-reserve-bank)  
13. Bank Term Funding Program (BTFP) and Other Federal Reserve Support to Banking System in Turmoil \- EveryCRSReport.com, accessed May 11, 2026, [https://www.everycrsreport.com/reports/IN12134.html](https://www.everycrsreport.com/reports/IN12134.html)  
14. Emergency Lending and Moral Hazard \- FDIC, accessed May 11, 2026, [https://www.fdic.gov/center-financial-research/emergency-lending-and-moral-hazard.pdf](https://www.fdic.gov/center-financial-research/emergency-lending-and-moral-hazard.pdf)  
15. Bank Term Funding Program: Experience and Lessons Learned, accessed May 11, 2026, [https://bpi.com/bank-term-funding-program-experience-and-lessons-learned/](https://bpi.com/bank-term-funding-program-experience-and-lessons-learned/)  
16. New Finance Support \- ebrd-restructuring.com, accessed May 11, 2026, [https://ebrd-restructuring.com/storage/uploads/r\_p\_documents/15148%20EBRD%20(New%20finance%20report%202023)%20ARTWORK\_digital\_HR.pdf](https://ebrd-restructuring.com/storage/uploads/r_p_documents/15148%20EBRD%20\(New%20finance%20report%202023\)%20ARTWORK_digital_HR.pdf)  
17. Depositor Characteristics and Deposit Stability \- FDIC, accessed May 11, 2026, [https://www.fdic.gov/media/168196](https://www.fdic.gov/media/168196)  
18. Why Banks Are Redesigning Their Deposit Strategies \- International Banker, accessed May 11, 2026, [https://internationalbanker.com/banking/why-banks-are-redesigning-their-deposit-strategies/](https://internationalbanker.com/banking/why-banks-are-redesigning-their-deposit-strategies/)  
19. Destabilizing Digital "Bank Walks" \- NBER, accessed May 11, 2026, [https://www.nber.org/system/files/working\_papers/w32601/revisions/w32601.rev0.pdf](https://www.nber.org/system/files/working_papers/w32601/revisions/w32601.rev0.pdf)  
20. Banking Sector Performance during two periods of sharply higher interest rates: 2022 and 2004 to 2006 \- FDIC, accessed May 11, 2026, [https://www.fdic.gov/analysis/quarterly-banking-profile/fdic-quarterly/2023-vol17-3/article1.pdf](https://www.fdic.gov/analysis/quarterly-banking-profile/fdic-quarterly/2023-vol17-3/article1.pdf)  
21. FDIC Quarterly Banking Profile, accessed May 11, 2026, [https://www.fdic.gov/quarterly-banking-profile/data-tables-q1-2025.pdf](https://www.fdic.gov/quarterly-banking-profile/data-tables-q1-2025.pdf)  
22. Discount Window Stigma After the Global Financial Crisis \- Federal Reserve Bank of New York, accessed May 11, 2026, [https://www.newyorkfed.org/medialibrary/media/research/staff\_reports/sr1137.pdf](https://www.newyorkfed.org/medialibrary/media/research/staff_reports/sr1137.pdf)  
23. FSB warns of financial stability challenges in repo markets \- Securities Finance Times, accessed May 11, 2026, [https://www.securitiesfinancetimes.com/securitieslendingnews/repoarticle.php?article\_id=228460](https://www.securitiesfinancetimes.com/securitieslendingnews/repoarticle.php?article_id=228460)  
24. Regulation Shadow Banking FSB \- Financial Stability Board, accessed May 11, 2026, [https://www.fsb.org/uploads/c\_130129y.pdf](https://www.fsb.org/uploads/c_130129y.pdf)  
25. Reflections on Northern Rock: The Bank Run that Heralded the Global Financial Crisis, accessed May 11, 2026, [https://www.bis.org/publ/shin\_2009.pdf](https://www.bis.org/publ/shin_2009.pdf)  
26. Transforming Shadow Banking into Resilient Market-based Finance: Annex 1, accessed May 11, 2026, [https://www.fsb.org/uploads/P070920-2.pdf](https://www.fsb.org/uploads/P070920-2.pdf)  
27. Is This Time Different: How Are Banks Performing during the Recent Interest Rate Increases Compared to 2004-2006? \- Federal Reserve, accessed May 11, 2026, [https://www.federalreserve.gov/econres/notes/feds-notes/is-this-time-different-how-are-banks-performing-during-the-rir-increases-compared-to-2004-2006-20240412.html](https://www.federalreserve.gov/econres/notes/feds-notes/is-this-time-different-how-are-banks-performing-during-the-rir-increases-compared-to-2004-2006-20240412.html)  
28. Liquidity Adequacy Requirements (LAR) (2026) Chapter 3 – Net Stable Funding Ratio \- Office of the Superintendent of Financial Institutions \- OSFI, accessed May 11, 2026, [https://www.osfi-bsif.gc.ca/en/guidance/guidance-library/liquidity-adequacy-requirements-lar-2026-chapter-3-net-stable-funding-ratio](https://www.osfi-bsif.gc.ca/en/guidance/guidance-library/liquidity-adequacy-requirements-lar-2026-chapter-3-net-stable-funding-ratio)  
29. Evolution of Debt Financing toward Less-Regulated Financial Intermediaries in the United States \- NBER, accessed May 11, 2026, [https://www.nber.org/system/files/working\_papers/w32114/w32114.pdf](https://www.nber.org/system/files/working_papers/w32114/w32114.pdf)  
30. Private Credit Funds as Key Lenders in Subscription and NAV Lines: Market Insights, accessed May 11, 2026, [https://www.troutman.com/insights/private-credit-funds-as-key-lenders-in-subscription-and-nav-lines-market-insights/](https://www.troutman.com/insights/private-credit-funds-as-key-lenders-in-subscription-and-nav-lines-market-insights/)  
31. Where Collateral Sleeps \- NBER, accessed May 11, 2026, [https://www.nber.org/system/files/working\_papers/w34266/w34266.pdf](https://www.nber.org/system/files/working_papers/w34266/w34266.pdf)  
32. Challenges posed by the sovereign-bank loop in the EU \- Eurofi, accessed May 11, 2026, [https://www.eurofi.net/session/challenges-posed-by-the-sovereign-bank-loop-in-the-eu/](https://www.eurofi.net/session/challenges-posed-by-the-sovereign-bank-loop-in-the-eu/)  
33. SOVEREIGN-BANK LOOP IN THE EU | Eurofi, accessed May 11, 2026, [https://www.eurofi.net/wp-content/uploads/2019/11/9.-sovereign-bank-loop-in-the-eu.pdf](https://www.eurofi.net/wp-content/uploads/2019/11/9.-sovereign-bank-loop-in-the-eu.pdf)  
34. Basel III: the net stable funding ratio \- Bank for International Settlements, accessed May 11, 2026, [https://www.bis.org/bcbs/publ/d295.pdf](https://www.bis.org/bcbs/publ/d295.pdf)  
35. Bank Leverage Ratios and Financial Stability: A Micro- and Macroprudential Perspective \- Levy Economics Institute of Bard College, accessed May 11, 2026, [https://www.levyinstitute.org/pubs/wp\_849.pdf](https://www.levyinstitute.org/pubs/wp_849.pdf)  
36. Leveraged Bank Loans Primer \- NAIC, accessed May 11, 2026, [https://content.naic.org/sites/default/files/capital-markets-primer-leveraged-bank-loans.pdf](https://content.naic.org/sites/default/files/capital-markets-primer-leveraged-bank-loans.pdf)  
37. Will CLO performance and leveraged finance trends diverge or align in 2026? \- Moody's, accessed May 11, 2026, [https://www.moodys.com/web/en/us/creditview/blog/leveraged-finance-and-clo-2026.html](https://www.moodys.com/web/en/us/creditview/blog/leveraged-finance-and-clo-2026.html)  
38. Report on Vulnerabilities in Private Credit \- Financial Stability Board, accessed May 11, 2026, [https://www.fsb.org/uploads/P060526.pdf](https://www.fsb.org/uploads/P060526.pdf)  
39. Bank Loans to NBFIs: Evidence of Specialization, Part I, accessed May 11, 2026, [https://www.philadelphiafed.org/the-economy/banking-and-financial-markets/bank-loans-to-nbfis-part1](https://www.philadelphiafed.org/the-economy/banking-and-financial-markets/bank-loans-to-nbfis-part1)  
40. COMMERCIAL REAL ESTATE: Trends, Risks, and Federal Monitoring Efforts, accessed May 11, 2026, [https://www.gao.gov/assets/880/872054.pdf](https://www.gao.gov/assets/880/872054.pdf)  
41. Special topic – CRE-related risks | European Banking Authority, accessed May 11, 2026, [https://www.eba.europa.eu/publications-and-media/publications/special-topic-cre-related-risks](https://www.eba.europa.eu/publications-and-media/publications/special-topic-cre-related-risks)  
42. Commercial Real Estate Weighs on Regional Banks | Mellon Investments Corporation, accessed May 11, 2026, [https://www.mellon.com/insights/insights-articles/commercial-real-estate-debt-matures-amidst-policy-shifts.html](https://www.mellon.com/insights/insights-articles/commercial-real-estate-debt-matures-amidst-policy-shifts.html)  
43. The CRE Market, Regional Banks, and Possible Recession | Western Asset Management, accessed May 11, 2026, [https://www.westernasset.com/us/en/pdfs/whitepapers/the-cre-market-regional-banks-and-possible-recession.pdf](https://www.westernasset.com/us/en/pdfs/whitepapers/the-cre-market-regional-banks-and-possible-recession.pdf)  
44. The Fed \- A Note on Recent Dynamics of Consumer Delinquency Rates \- Federal Reserve, accessed May 11, 2026, [https://www.federalreserve.gov/econres/notes/feds-notes/a-note-on-recent-dynamics-of-consumer-delinquency-rates-20251124.html](https://www.federalreserve.gov/econres/notes/feds-notes/a-note-on-recent-dynamics-of-consumer-delinquency-rates-20251124.html)  
45. Bridge rounds, SAFEs, and venture debt: How to stack capital without boxing yourself in, accessed May 11, 2026, [https://mercury.com/blog/bridge-rounds-safes-venture-debt-how-to-stack-capital](https://mercury.com/blog/bridge-rounds-safes-venture-debt-how-to-stack-capital)  
46. Venture Debt for Startups: How Non-Dilutive Capital Works, accessed May 11, 2026, [https://www.moonshotnx.com/venture-debt-for-startups](https://www.moonshotnx.com/venture-debt-for-startups)  
47. Venture Debt: How It Works, Costs & When to Use It \- Founderpath, accessed May 11, 2026, [https://founderpath.com/blog/venture-debt](https://founderpath.com/blog/venture-debt)  
48. Understanding Priced Rounds vs SAFEs \- Carta, accessed May 11, 2026, [https://carta.com/learn/startups/fundraising/priced-rounds/](https://carta.com/learn/startups/fundraising/priced-rounds/)  
49. SAFE Rounds and Valuation Caps Explained: What Founders Need to Know Before Raising, accessed May 11, 2026, [https://www.finrofca.com/startup-qa/safe-rounds-valuation-caps-explained](https://www.finrofca.com/startup-qa/safe-rounds-valuation-caps-explained)  
50. SHADOW BANKING \- CFA Institute, accessed May 11, 2026, [https://www.cfainstitute.org/sites/default/files/-/media/documents/article/position-paper/shadow-banking-policy-frameworks-investor-perspectives-market-based-finance.pdf](https://www.cfainstitute.org/sites/default/files/-/media/documents/article/position-paper/shadow-banking-policy-frameworks-investor-perspectives-market-based-finance.pdf)  
51. Transformed Intermediation: Credit Risk to NBFIs, Liquidity Risk to ..., accessed May 11, 2026, [https://www.newyorkfed.org/medialibrary/media/research/staff\_reports/sr1176.pdf](https://www.newyorkfed.org/medialibrary/media/research/staff_reports/sr1176.pdf)  
52. FSB warns on private credit vulnerabilities \- Financial Stability Board, accessed May 11, 2026, [https://www.fsb.org/2026/05/fsb-warns-on-private-credit-vulnerabilities/](https://www.fsb.org/2026/05/fsb-warns-on-private-credit-vulnerabilities/)  
53. The Role of NAV Loans and How They Fit in GPs Financial Tool Kit | Data Analytics \- LSEG, accessed May 11, 2026, [https://www.lseg.com/en/data-analytics/investment-banking/lpc/podcast/lending-lowdown/episode-38-the-role-of-nav-loans-and-how-they-fit-in-gp-financial-tool-kit](https://www.lseg.com/en/data-analytics/investment-banking/lpc/podcast/lending-lowdown/episode-38-the-role-of-nav-loans-and-how-they-fit-in-gp-financial-tool-kit)  
54. Buy Now, Pay Later: Policy Issues and Options for Congress \- EveryCRSReport.com, accessed May 11, 2026, [https://www.everycrsreport.com/reports/R48858.html](https://www.everycrsreport.com/reports/R48858.html)  
55. Buy Now, Pay Later: Recent Developments and Implications | Richmond Fed, accessed May 11, 2026, [https://www.richmondfed.org/publications/research/economic\_brief/2026/eb\_26-05](https://www.richmondfed.org/publications/research/economic_brief/2026/eb_26-05)  
56. Vulnerabilities in Non-bank Commercial Real Estate Investors \- Financial Stability Board, accessed May 11, 2026, [https://www.fsb.org/uploads/P190625.pdf](https://www.fsb.org/uploads/P190625.pdf)  
57. Supply Chain Finance in Central Asia and Caucasus \- ADB Brief No. 250 \- Asian Development Bank, accessed May 11, 2026, [https://www.adb.org/sites/default/files/publication/891871/adb-brief-250-supply-chain-finance-central-asia.pdf](https://www.adb.org/sites/default/files/publication/891871/adb-brief-250-supply-chain-finance-central-asia.pdf)  
58. What Is Trade Finance? A Detailed Guide for International Businesses | SUISSE BANK, accessed May 11, 2026, [https://www.suissebank.com/en/what-is-trade-finance-a-detailed-guide-for-international-businesses.html](https://www.suissebank.com/en/what-is-trade-finance-a-detailed-guide-for-international-businesses.html)  
59. The role of supply chain finance (scf) platforms in mitigating financial risk and improving resilience \- American Institute of Mathematical Sciences, accessed May 11, 2026, [https://www.aimsciences.org/article/doi/10.3934/jdg.2026015?viewType=HTML](https://www.aimsciences.org/article/doi/10.3934/jdg.2026015?viewType=HTML)  
60. Center for Microeconomic Data | Credit Cards and Auto Loans \- Federal Reserve Bank of New York, accessed May 11, 2026, [https://www.newyorkfed.org/microeconomics/topics/credit-cards-auto-loans](https://www.newyorkfed.org/microeconomics/topics/credit-cards-auto-loans)  
61. CFPB Publishes New Findings on Financial Profiles of Buy Now, Pay Later Borrowers, accessed May 11, 2026, [https://www.consumerfinance.gov/about-us/newsroom/cfpb-publishes-new-findings-on-financial-profiles-of-buy-now-pay-later-borrowers/](https://www.consumerfinance.gov/about-us/newsroom/cfpb-publishes-new-findings-on-financial-profiles-of-buy-now-pay-later-borrowers/)  
62. Credit FAQ: What An Acceleration Of Quantitative Tightening Could Mean For Eurozone Banks \- S\&P Global, accessed May 11, 2026, [https://www.spglobal.com/ratings/en/regulatory/article/-/view/sourceId/12845076](https://www.spglobal.com/ratings/en/regulatory/article/-/view/sourceId/12845076)  
63. Stabilisation policies to strengthen Euro Area resilience: OECD Economic Surveys, accessed May 11, 2026, [https://www.oecd.org/en/publications/oecd-economic-surveys-euro-area-2018\_eco\_surveys-euz-2018-en/full-report/component-6.html](https://www.oecd.org/en/publications/oecd-economic-surveys-euro-area-2018_eco_surveys-euz-2018-en/full-report/component-6.html)  
64. “Doom Loop” Crises: The Sovereign-Banking Nexus and Implications for Country Risk Management | Columbia SIPA, accessed May 11, 2026, [https://www.sipa.columbia.edu/doom-loop-crises-sovereignbanking-nexus-and-implications-country-risk-management](https://www.sipa.columbia.edu/doom-loop-crises-sovereignbanking-nexus-and-implications-country-risk-management)  
65. Breaking the vicious circle between banks and sovereigns for good \- Deutsche Bundesbank, accessed May 11, 2026, [https://www.bundesbank.de/en/press/contributions/breaking-the-vicious-circle-between-banks-and-sovereigns-for-good-942468](https://www.bundesbank.de/en/press/contributions/breaking-the-vicious-circle-between-banks-and-sovereigns-for-good-942468)  
66. Financial Globalization: Culprit, Survivor or Casualty of the Great Crisis?, accessed May 11, 2026, [https://ycsg.yale.edu/sites/default/files/files/financial\_globalization.pdf](https://ycsg.yale.edu/sites/default/files/files/financial_globalization.pdf)  
67. Managing the Sovereign-Bank Nexus \- International Monetary Fund, accessed May 11, 2026, [https://www.imf.org/-/media/files/publications/dp/2018/45133-dp1816-managing-the-sovereign-bank-nexus.pdf](https://www.imf.org/-/media/files/publications/dp/2018/45133-dp1816-managing-the-sovereign-bank-nexus.pdf)  
68. SOVEREIGN AND BANKING RISKS: WHAT POLICIES?, accessed May 11, 2026, [https://european-economy.eu/wp-content/uploads/2016/07/EE\_2016\_2.pdf](https://european-economy.eu/wp-content/uploads/2016/07/EE_2016_2.pdf)  
69. Regulating the doom loop \- European Banking Authority, accessed May 11, 2026, [https://www.eba.europa.eu/sites/default/files/documents/10180/2198067/391eef1b-517b-4090-b1b5-8ac1ee8897df/3\_S.%20Alogoskoufis%2C%20S.%20Langfield%20-%20Regulating%20the%20doom%20loop.pdf](https://www.eba.europa.eu/sites/default/files/documents/10180/2198067/391eef1b-517b-4090-b1b5-8ac1ee8897df/3_S.%20Alogoskoufis%2C%20S.%20Langfield%20-%20Regulating%20the%20doom%20loop.pdf)  
70. BANK POLICY INSTITUTE, BRETT WAXMAN \- Federal Reserve, accessed May 11, 2026, [https://www.federalreserve.gov/apps/proposals/comments/FR-0000-0137-01-C117](https://www.federalreserve.gov/apps/proposals/comments/FR-0000-0137-01-C117)  
71. BPI-Morgan Stanley Symposium on Money Markets \- Bank Policy Institute, accessed May 11, 2026, [https://bpi.com/bpi-morgan-stanley-symposium-on-money-markets/](https://bpi.com/bpi-morgan-stanley-symposium-on-money-markets/)  
72. the Role of liquidity in financial crises \- Federal Reserve Bank of Kansas City, accessed May 11, 2026, [https://www.kansascityfed.org/Jackson%20Hole/documents/3172/2008-allenandcarletti031209.pdf](https://www.kansascityfed.org/Jackson%20Hole/documents/3172/2008-allenandcarletti031209.pdf)  
73. Full article: Examining modern money creation: An institution-centered explanation and visualization of the “credit theory” of money and some reflections on its significance \- Taylor & Francis, accessed May 11, 2026, [https://www.tandfonline.com/doi/full/10.1080/00220485.2022.2075510](https://www.tandfonline.com/doi/full/10.1080/00220485.2022.2075510)

---