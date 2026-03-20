# Guidwirehack
GigZo — Pre → Present → Post Disruption Continuum Engine
AI-powered parametric income protection for India's food and quick-commerce delivery workforce — automatic payouts before, during, and after disruptions hit. No claims required. Ever.
Show Image
Show Image
Show Image
Show Image

The Problem
India's food and quick-commerce delivery partners — working for Zomato, Swiggy, Blinkit, and Zepto — are the human infrastructure of a sector processing over 10 million orders a day. They operate on a gig basis: no fixed salary, no safety net, no paid leave.
When external disruptions hit — a flash flood in Mumbai, a sudden curfew in a sensitive zone, a severe AQI advisory in Delhi, or a Zomato server outage on a peak Friday night — delivery partners lose 20–30% of their monthly income with zero recourse. They can't work. The orders don't move. Nobody compensates them.
Every parametric insurance solution built for this problem makes the same architectural mistake: it pays once, at the moment the trigger fires, then disappears. But a disruption is not a moment. It's a timeline.
GigZo exists to cover the entire timeline.

⚠️ Coverage Scope: GigZo insures INCOME LOSS ONLY. We do not cover health, life, accidents, or vehicle repairs. This is a pure parametric income protection product.


What Every Other Solution Gets Wrong
The standard DEVTrails submission has this architecture:
Rain > 50mm  →  Flat ₹500 payout  →  Done.
This is reactive, binary, and incomplete. It misses three phases that together represent the majority of a worker's actual financial loss:
Phase 1 — Pre-disruption (Days −4 to 0). The flood is coming. IMD can see it. The worker has no elevated coverage, no warning, and no locked-in premium rate. If the platform detects the risk, it could auto-protect the worker before anything happens. Nobody does this.
Phase 2 — During disruption (Hours 0 to N). Rain hits 80mm and is still climbing. The payout is still ₹500 flat — the same as if it had stopped at 51mm. The severity of the event bears no relationship to the compensation. Nobody addresses this.
Phase 3 — Post-disruption (Days +1 to +4). The flood clears Monday evening. Roads reopen Tuesday morning. But delivery orders don't return to normal until Thursday. The worker loses two additional days of income that no trigger ever fires for. Nobody compensates this.
GigZo covers all three. It is the only parametric platform with full temporal coverage of the disruption lifecycle.

Our Solution
GigZo is an AI-powered parametric insurance platform that:

Predicts disruptions 3–7 days ahead using ensemble weather models, GDELT social event detection, and labour court data — and automatically elevates worker coverage before anything happens
Monitors disruption severity in real-time using LSTM time-series models and stages payouts progressively as conditions worsen — not a flat amount at threshold crossing
Predicts income recovery time after a disruption clears using survival analysis, and automatically issues bridge credit to cover the shadow period
Logs every decision immutably on Hyperledger Fabric — workers can independently verify every payout decision via a QR-linked blockchain explorer in the app
Detects fraud using continuous sensor fusion throughout the event window, not a single GPS check at trigger time


Persona & Scenarios
Our Persona: Food and Quick-Commerce Delivery Partner

Platforms: Zomato, Swiggy, Blinkit, Zepto
Profile: Typically male, 22–38 years old, owns a two-wheeler, earns ₹600–₹900/day net, operates across Tier 1 Indian cities, week-to-week income with zero employer safety net
Financial reality: Gross monthly earnings ~₹26,500. After fuel, vehicle maintenance, and data — net take-home ~₹21,000. Fixed costs (EMI, rent) don't pause when a flood hits.


Scenario 1 — Environmental Disruption: Urban Flooding (Mumbai)
Ravi is a Swiggy delivery partner in Andheri West, Mumbai. On Thursday afternoon, IMD ensemble models show a 76% probability of rainfall exceeding 60mm in his zone by Saturday morning — four days away.
GigZo Pre-Engine Response (Thursday): The forecast crosses the confidence threshold. Ravi's coverage is automatically elevated from Standard to Elevated tier. His weekly premium is locked at ₹94. A push notification tells him: "Heavy rain likely Saturday. Your coverage is elevated. No action needed." The prediction is logged immutably on-chain with a timestamp.
GigZo Present-Engine Response (Saturday): Rain hits 55mm at 9 AM. Partial payout of ₹200 is issued. By 11 AM, rainfall reaches 74mm and is still rising — the LSTM model predicts 5 more hours of disruption. Payout stages up to ₹380. By 2 PM, satellite SAR data confirms zone waterlogging. Full payout of ₹550 plus a ₹100 recovery anticipation bonus is transferred to Ravi's UPI ID. He filed no claim. He pressed no button.
GigZo Post-Engine Response (Sunday): The Cox Proportional Hazards model predicts that order volumes in Andheri West won't normalise until Tuesday 10 AM — a 38-hour shadow gap. Bridge credit of ₹340 is auto-issued and will be repaid from Ravi's Week 3 premium deduction. Total received: ₹990. Total actions taken by Ravi: zero.

Scenario 2 — Social Disruption: Unplanned Curfew (Delhi)
Priya is a Blinkit delivery partner in Laxmi Nagar, Delhi. A sudden Section 144 curfew is imposed after a local incident. All movement is restricted from 1 PM to 9 PM.
GigZo Response: The GDELT social event monitor detects a burst of NLP-classified "curfew" and "Section 144" events mapped to Laxmi Nagar's pin code within a 12-minute window. Independent media corroboration pushes the confidence score above the trigger threshold. GigShield cross-references Priya's active delivery zone, confirms she was GPS-active in that zone at 12:45 PM, and initiates a payout for 8 hours of lost earnings. Priya receives ₹480 by 1:30 PM — 30 minutes after the curfew was imposed.

Scenario 3 — Systemic Disruption: Platform Outage (Nationwide)
Suresh is a Zomato delivery partner in Koramangala, Bengaluru. On a peak Friday evening, Zomato's app experiences a critical server outage lasting 3.5 hours.
GigZo Response: The platform monitoring layer detects Zomato's DNS downtime via cloud status APIs. The outage crosses the 2-hour threshold during a designated peak-hour window (7 PM–10 PM). GigZo initiates payouts for all active policyholders assigned to the Zomato platform. Suresh receives ₹260 for the lost peak-hour window without filing anything.

Scenario 4 — Environmental Disruption: Severe Pollution (Delhi NCR)
Deepak is a Zepto partner in Najafgarh, Delhi. In November, AQI in his zone sustains above 400 for two consecutive days. The government issues a two-wheeler delivery restriction advisory.
GigZo Response: CPCB sensor data and WAQI API confirm AQI > 400 in Deepak's pin code during his active shift hours. The government advisory is cross-validated via the news API. GigZo triggers a payout for restricted working hours. Deepak receives ₹310 for lost earnings during the advisory window.

Application Workflow
1. Onboard — Worker registers on GigZo via the app, enters their e-Shram UAN for instant KYC (Aadhaar-verified, NPCI bank-linked, zero manual paperwork), selects their primary delivery platform, and sets a UPI ID for payouts. Total onboarding time: 45 seconds.
2. Risk Profile — The AI engine scores the worker's zone risk based on flood history, AQI trends, curfew frequency, and platform outage patterns, combined with their personal delivery history and e-Shram occupation data.
3. Weekly Policy — Worker selects a coverage tier. The ML pricing engine generates a dynamic weekly premium based on the upcoming week's risk forecast for their zone. Premium is auto-debited every Monday from their linked UPI.
4. Active Coverage — The Pre-Engine runs continuously in the background. If a disruption is forecast with >70% confidence, coverage is elevated and the worker is notified. No action required.
5. Disruption Occurs — The Present-Engine detects threshold breaches in real-time and stages payouts progressively as severity escalates. Fraud validation runs continuously throughout the event.
6. Recovery Period — The Post-Engine predicts the income recovery timeline and auto-issues bridge credit for the shadow disruption period. Repaid automatically from the next week's premium cycle.
7. Audit Trail — Every decision across all three phases is logged immutably on Hyperledger Fabric. Workers can scan their in-app QR code at any time to view a complete, independently verifiable history of every data value, threshold check, and payout decision. No insurer discretion. No black box.

Weekly Premium Model
GigZo uses a weekly subscription model aligned with how delivery partners earn and think about money. No annual commitments. No confusing monthly math. Every Monday, coverage renews and premium is auto-debited.
Coverage Tiers
TierWeekly PremiumMax Weekly PayoutBest ForBasic Shield₹29/week₹500/weekOccasional workers (<20 hrs/week)Standard Shield₹64/week₹1,400/weekRegular workers (20–40 hrs/week)Pro Shield₹109/week₹2,800/weekFull-time partners (40+ hrs/week)
How the Premium is Calculated
The base tier price is adjusted each week by our ML Risk Engine using the following factors:
FactorEffect on Weekly PremiumZone flood risk score (GBM spatial model)+/− ₹5–18/weekHistorical AQI in zone (Oct–Feb)+/− ₹3–10/weekWorker's average active hoursScales coverage tierZone curfew frequency index+/− ₹2–8/weekPlatform outage history in zone+/− ₹1–6/weekWorker's claim history and Trust ScoreFraud flag adjustmentResilience streak (4+ weeks no claims)Up to −12% discount
The pricing kernel uses a Choquet integral representation to handle non-linear relationships between multi-dimensional risk indices and actual income loss. Premium recalculates fresh every Monday.
Example: A Standard Shield worker in Koregaon Park, Pune (low risk) pays ₹57/week. The same worker in Najafgarh, Delhi (high flood + AQI risk) pays ₹79/week.
Actuarial Viability Sketch
TierWeekly PremiumExpected Claim Freq.Avg. PayoutExpected Weekly LossMarginBasic₹29~8% of weeks₹260₹21~28%Standard₹64~10% of weeks₹650₹65Breakeven → cross-subsidisedPro₹109~12% of weeks₹1,300₹156Reinsurance layer above ₹90/week loss
These figures are based on IMD historical disruption data for Mumbai, Delhi, and Bengaluru (2019–2024). Actual loss ratios will be validated against real claim data and adjusted dynamically. The model targets a combined loss ratio below 85%, with reinsurance covering tail events.

Parametric Triggers
Objective, data-driven thresholds that automatically initiate a claim. No subjective assessment. No paperwork.
#TriggerData SourceThresholdPayout Basis1Heavy RainfallIMD + OpenWeatherMapRainfall > 64.5mm/day (Red Alert)Per hour unable to work2Urban Flood ConfirmationSAR satellite (Floodbase/ICEYE)Verified waterlogging in worker's pin codeFlat daily payout3Severe AQICPCB / WAQI APIAQI > 400 + govt two-wheeler advisoryPer restricted hour4Curfew / Section 144GDELT NLP event detectionHigh-confidence curfew event in delivery zonePer hour of restriction5Extreme HeatIMD + OpenWeatherMapWet-bulb temp > 35°C for 4+ consecutive hoursPer hour during advisory6Platform OutageCloud status APIs + custom pingsAggregator DNS/server downtime > 2 continuous hoursPer lost peak-hour window
All triggers are cross-validated against the worker's last known GPS location to prevent fraudulent claims from unaffected zones. Pre-Engine prediction timestamps on Hyperledger prove coverage was active before the event — preventing post-event fabrication.

The Three Engines — Technical Architecture
Engine 1 — Pre: Disruption Forecast Layer
The Pre-Engine continuously ingests eight data sources and runs a Gradient Boosting Machine (XGBoost) with Facebook Prophet for seasonal patterns. The feature matrix includes days since last major disruption in the zone, labour court filing spikes (eCourts API), union registration activity delta (Shram Suvidha), keyword velocity from GDELT NLP, political calendar proximity (ECI API), and historical disruption frequency per district.
When the predicted probability of a triggering event crosses 70% confidence for the upcoming week, the engine automatically elevates the worker's coverage tier, locks the premium at the current rate, writes an immutable prediction record to Hyperledger Fabric with a timestamp and data source hashes, and sends the worker a forecast notification. The on-chain timestamp is the proof — it makes post-event policy manipulation impossible.
Engine 2 — Present: Adaptive Payout Engine
The Present-Engine runs an LSTM model on a 24-hour rolling window of multi-source sensor data. Instead of a binary trigger, it tracks disruption severity continuously and stages payouts as conditions escalate. A flood that starts at 52mm and climbs to 80mm over six hours produces a correspondingly escalating payout — not the same flat amount as a flood that peaked at 51mm and cleared immediately.
The model outputs three values: predicted remaining disruption duration, current severity index, and recommended payout stage. Fraud validation runs continuously throughout the event using GPS and IMU sensor fusion — not a single point check. Spoofing a coherent 6-hour sensor fusion window is exponentially harder than spoofing a single GPS coordinate.
Engine 3 — Post: Income Recovery Predictor
The Post-Engine uses a Cox Proportional Hazards survival analysis model to predict time-to-full-income-recovery after a disruption clears. Inputs include historical post-event order volume patterns, road clearance time from Google Maps Traffic API, the worker's personal recovery history, delivery density in adjacent zones, and the disruption type and severity.
When the recovery prediction is generated, a bridge credit is automatically issued to cover the shadow gap period. Repayment is auto-deducted from the next week's premium cycle. The worker's account never goes negative. They never initiate anything.

Adversarial Defense & Anti-Spoofing Strategy
Why Simple GPS Verification Is Dead
A single GPS check at trigger time is trivially defeated by mock location apps freely available on Android. GigZo's fraud defense is built on the assumption that no single signal can be trusted in isolation. A legitimate claim must pass corroboration across four independent layers simultaneously.
Layer 1 — GPS Physics & Trajectory Validation
A real delivery partner's movement leaves a forensic signature: road-constrained paths, realistic velocity curves, natural deceleration at junctions, consistent cell tower handoffs. Spoofed GPS leaves a different one.
We check trajectory coherence against road geometry (the worker's GPS trace must follow plausible road paths within 50m over the preceding 30 minutes); speed physics (movement faster than ~40 km/h in an urban disruption zone during a claimed "unable to work" period flags the claim); cell tower cross-check (GPS coordinates are corroborated against the serving cell tower's known coverage area); and stationary validation (active delivery movement patterns during a claimed disruption auto-reject the claim).
This layer eliminates individual bad actors using mock location apps. GPS spoofing that passes visual inspection fails trajectory physics analysis.
Layer 2 — Fraud Ring Detection via Network Graph
This is the layer that addresses coordinated attacks. Individual anomaly detection misses a fraud ring by design — each individual claim looks plausible in isolation. Network analysis catches what individual checks cannot.
GigZo constructs a graph where nodes are individual workers and edges are connections between workers who share a device fingerprint, the same sub-zone claim within a tight time window, correlated claim timing patterns, or overlapping account registration metadata.
Ring detection works on temporal clustering — a genuine rainstorm triggers claims distributed across a zone over 1–3 hours as workers encounter the disruption at different times; a fraud ring triggers a burst within a narrow 5–15 minute window, detectable immediately via Z-score burst analysis. Device fingerprint overlap catches multiple accounts created from the same device. Graph density threshold catches clusters of workers with 2+ shared edges claiming simultaneously.
The key distinction: a legitimate mass disruption produces a distributed, uncorrelated claim graph. A fraud ring produces a dense, correlated cluster. These patterns are statistically distinguishable even at 500-person scale.
Layer 3 — Per-Worker Behavioral Baseline
Each worker builds a longitudinal behavioral profile. Workers with 4+ weeks of clean delivery history and consistent platform activity earn a Trust Score from 0–100. A first-time worker claiming on Day 1 of their first policy with no delivery history on their linked platform routes to manual review. A worker with 6 months of verified activity, 2 prior legitimate claims, and consistent GPS patterns in their declared zone gets expedited auto-approval.
This is how we distinguish the genuinely stranded worker from the fraudster. The honest Ravi who has been delivering in Andheri West for 8 months gets paid in minutes. The suspicious new account created 3 days ago, claiming from the same zone as 47 other new accounts, does not.
Layer 4 — Liquidity Circuit Breaker
Even if individual fraud signals are subtle, the aggregate effect of a coordinated attack is detectable at zone level. GigZo tracks a rolling Zone Claim Rate for each pin code — the number of active claims as a percentage of registered workers. If the Zone Claim Rate spikes more than 3× the historical baseline within a 2-hour window, the system pauses new disbursements from that zone, flags all pending claims for manual review, alerts the admin dashboard, and notifies legitimate affected workers with a resolution ETA.
Workers with a Trust Score above 80 receive a provisional 50% advance payout during a circuit breaker event. They are not penalised for someone else's fraud ring.
Summary: Why This Architecture Works
Attack TypeDefeated BySingle worker using mock location appLayer 1 — GPS physicsSmall group with coordinated GPS spoofingLayer 1 + Layer 2Large fraud ring (500+ partners) with fake GPSLayer 2 (ring detection) + Layer 4 (circuit breaker)New account fraud (no history)Layer 3 — behavioral baselineSustained low-volume fraud ringLayer 2 (graph density over time) + Layer 3
Defeating any single layer requires simultaneously defeating all others. A real fraud ring would need to spoof GPS with trajectory coherence (Layer 1), avoid device/IP/timing correlation with co-conspirators (Layer 2), build months of fake delivery history (Layer 3), and stay below zone-level statistical thresholds (Layer 4) — simultaneously. This is not operationally feasible at scale.

Hyperledger Fabric — Immutable Audit Layer
Every decision across all three phases is written to a permissioned Hyperledger Fabric ledger as an immutable transaction. Three organisations participate: GigZo (read/write), Worker (read-only, own records only), and IRDAI/Regulator (aggregated audit view, no PII).
EventData Written On-ChainPre-Engine predictionZone, confidence score, timestamp, data source hashesCoverage elevationPolicy ID, tier change, trigger reasonThreshold breachRaw API reading, threshold value, pass/fail, model versionFraud check resultScore, flags raised, decision (no PII)Payout stage issuedAmount, UPI reference, timestampRecovery predictionPredicted recovery time, confidence intervalBridge credit issuedAmount, repayment scheduleClaim rejectionReason code + exact data values that caused it
Workers scan a QR code in the app to view their complete, immutable claim history. No insurer can retroactively alter what the IMD said, what the threshold was, or why a decision was made. This is not a transparency feature — it is the mechanism that makes worker trust structurally possible rather than an ask.

e-Shram Integration
e-Shram is the Government of India's national database for unorganised workers with over 300 million registrations, all Aadhaar-verified and NPCI bank-linked. GigZo uses it as the primary onboarding channel.
When a worker enters their e-Shram UAN, GigZo automatically retrieves their Aadhaar-verified identity, occupation code (confirming gig worker status), primary work district (setting their default trigger zone), and NPCI-linked bank account (the payout destination). KYC is instant. No document uploads. No waiting period.
This matters beyond convenience. The UAN is Aadhaar-linked one-per-person — duplicate account fraud is structurally prevented at entry before any ML model runs. New Labour Codes effective April 2026 mandate e-Shram registration for gig workers seeking social security benefits, meaning GigZo's onboarding intercepts workers at the exact moment the government brings them into the formal system. And 500,000+ Common Service Centres across India become natural co-distribution points.

AI/ML Integration Plan
1. Dynamic Premium Calculation
Model: Gradient Boosted Trees (XGBoost) with Choquet integral pricing kernel
Inputs: Zone pin code, worker's active hours, historical claim frequency in zone, seasonal risk index, upcoming week's probabilistic forecast
Output: Personalised weekly premium (0.8× – 1.6× base tier price)
Retraining: Weekly using new weather, claim, and platform data
2. Disruption Forecasting (Pre-Engine)
Model: XGBoost + Facebook Prophet for seasonal patterns
Inputs: IMD ensemble forecast, GDELT keyword velocity, ECI political calendar, eCourts labour filing spikes, Shram Suvidha union activity, historical disruption patterns
Output: Disruption probability score (0–1), predicted window (days), confidence level, affected pin codes
3. Adaptive Payout Staging (Present-Engine)
Model: LSTM on 24-hour rolling time-series window
Inputs: Rainfall, temperature, wind, humidity, flood risk index (hourly)
Output: Remaining disruption duration estimate, severity index, recommended payout stage
4. Recovery Prediction (Post-Engine)
Model: Cox Proportional Hazards (Survival Analysis)
Inputs: Historical post-event order volumes, road clearance time, worker recovery history, adjacent zone density, disruption type and severity
Output: Time-to-full-income-recovery (hours), bridge credit amount
5. Fraud Detection
Models: Isolation Forest (anomaly detection) + Graph Neural Network (ring detection) + CNN-BiLSTM (GPS spoof detection) + rule-based layer
Signals: GPS trajectory physics, cell tower corroboration, IMU sensor fusion, claim timing patterns, network graph density, device fingerprint overlap, behavioral baseline deviation
Output: Fraud Risk Score (0–100). Score > 70 = manual review. Score > 90 = auto-reject.

Fraud Detection Summary
LayerMechanismHow It WorksGPS PhysicsTrajectory coherence + cell tower checkRoad geometry, speed limits, tower corroborationNetwork GraphRing detection via GNNTemporal clustering, device fingerprint overlap, registration signalsContinuous Sensor FusionCNN-BiLSTM on IMU dataValidates physical presence throughout event — not just at triggerActivity ContradictionDelivery activity checkNo payout if platform activity confirms deliveries during disruptionBehavioral BaselinePer-worker Trust ScoreLongitudinal profile; new accounts get heightened scrutinyDuplicate PreventionClaim deduplicationSame worker cannot claim two overlapping disruptionsAnomaly DetectionIsolation ForestFlags statistical outliers vs zone cohortVelocity CheckRate limitingMore than 3 claims/week triggers enhanced reviewCircuit BreakerZone-level rate monitoringZone claim spike → pause payouts, queue for reviewe-Shram BindingUAN → Aadhaar 1:1Structural duplicate prevention at onboarding

Platform & Tech Stack
We are building a Progressive Web App (PWA) — mobile-first for delivery partners, desktop-capable for the insurer admin dashboard — in a single React codebase.
LayerTechnologyWhyFrontendReact.js (PWA)Mobile-responsive, installable, no App Store overheadBackendNode.js + NestJSModular REST APIs, scalable microservice structureDatabasePostgreSQL + RedisRelational policy/claim data + job queues for trigger engineML ServicesPython + FastAPIXGBoost, LSTM, Cox PH, Isolation Forest, GNN, CNN-BiLSTMBlockchainHyperledger Fabric 2.x + Go chaincodePermissioned ledger, IRDAI-compliant, no token overheadPolicy AdminGuidewire PolicyCenter + APDWeekly product lifecycle, auto-generated REST APIsClaims AdminGuidewire ClaimCenterZero-touch straight-through processingWeather APIIMD + OpenWeatherMapDual-oracle rainfall, temperature, heat indexAQI APICPCB / WAQIReal-time air quality by districtSocial EventsGDELT Project APINLP-based curfew and strike detectionTrafficGoogle Maps Traffic APIRoad clearance time for post-engineIdentitye-Shram UAN APIInstant Aadhaar-verified KYCPaymentsRazorpay Test ModeSimulated UPI payouts and auto-repaymentHostingVercel (frontend) + Render (backend) + AWS SageMaker (ML)Free/low-cost tiers, fast deploysVersion ControlGitHubSingle mono-repo

Development Plan
Phase 1 (Weeks 1–2): Ideation & Foundation ✅

 Finalise persona and problem scope (food/quick-commerce delivery)
 Define parametric triggers and premium model
 Design Pre → Present → Post three-engine architecture
 Define Hyperledger audit layer and on-chain event schema
 Define adversarial defense — four-layer fraud architecture
 Write README and system design documentation
 Set up GitHub repo and project board
 Build basic React PWA shell and routing
 Create worker onboarding UI mockup (e-Shram UAN flow)
 Record 2-minute strategy video

Phase 2 (Weeks 3–4): Core Platform & Automation

 Worker registration + e-Shram UAN authentication flow
 Insurance policy creation with dynamic weekly premium
 Integrate IMD + OpenWeatherMap + CPCB/WAQI APIs
 Build claims management module
 Implement ML premium scoring (XGBoost + Choquet kernel)
 Build automated trigger monitoring service (Present-Engine)
 Implement GPS physics validation (Layer 1 fraud)
 Build network graph ring detection (Layer 2 fraud)
 Implement basic Hyperledger Fabric network (3 orgs)
 Deploy trigger audit log chaincode (Go)
 Record 2-minute demo video

Phase 3 (Weeks 5–6): Full Intelligence & Scale

 Pre-Engine: XGBoost + Prophet forecast layer with GDELT integration
 Present-Engine: LSTM adaptive payout staging
 Post-Engine: Cox PH recovery predictor + bridge credit automation
 Full fraud detection stack (Isolation Forest + GNN + CNN-BiLSTM)
 Per-worker Trust Score and behavioral baseline (Layer 3)
 Zone-level liquidity circuit breaker (Layer 4)
 Simulated instant payout via Razorpay test mode
 Worker dashboard (coverage status, forecast card, payout history, chain explorer QR)
 Insurer/admin dashboard (loss ratios, zone heatmap, fraud queue, predictive analytics)
 End-to-end disruption simulation demo (all three phases)
 Final pitch deck (PDF)
 Record 5-minute demo video
