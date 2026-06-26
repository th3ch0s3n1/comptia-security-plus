# 📊 Section 18: Risk Analysis & Assessments

> Cornell Notes — CompTIA Security+ (SY0-701) | Maps to Domain 5.0 (Security Program Management and Oversight)

## ❓ Cue / Key Questions & Notes

| Question / Keyword | Answer |
| --- | --- |
| **🟢 Risk Assessment Frameworks** |  |
| 🔴 What is a risk assessment? | An ongoing or point-in-time process used to identify, analyze, and evaluate threats to organizational assets. |
| 🔴 Ad-hoc vs. Recurring assessments | Ad-hoc assessments are triggered by specific events (like system updates or breaches); recurring assessments run on a fixed schedule for continuous compliance. |
| 🔴 Qualitative vs. Quantitative | Qualitative uses subjective rankings (High/Medium/Low) based on human judgment; Quantitative uses concrete mathematical and financial values. |
| 🔴 What is a risk heat map? | A visual matrix that plots risks based on their **likelihood** of occurrence against their operational **impact**. |
| **🟢 Quantitative Risk Calculation** | ALE |
| 🔴 What is Asset Value (AV)? | The total financial or operational worth of a corporate resource or data set. |
| 🔴 What is the Exposure Factor (EF)? | The percentage of an asset's total value that is lost as a result of a specific security incident. |
| 🔴 What is Single Loss Expectancy (SLE)? | The financial loss expected each time a specific threat exploits a vulnerability. Formula: $SLE = AV \times EF$. |
| 🔴 What is Annualized Rate of Occurrence (ARO)? | An estimate of how many times a specific threat is expected to successfully exploit a vulnerability within a single year. |
| 🔴 What is Annualized Loss Expectancy (ALE)? | The total expected financial loss from a specific risk over an entire year. Formula: $ALE = SLE \times ARO$. |
| **🟢 Business Impact Analysis Metrics** | BIA |
| 🔴 What is Recovery Time Objective (RTO)? | The maximum acceptable duration of time that a system or business process can remain offline after a disaster before causing major harm. |
| 🔴 What is Recovery Point Objective (RPO)? | The maximum acceptable age of data that can be lost from storage backup systems when an unexpected failure occurs. |
| 🔴 MTBF vs. MTTR | Mean Time Between Failures (MTBF) measures hardware reliability by calculating average uptime; Mean Time to Repair (MTTR) tracks average time to fix a failed system. |
| **🟢 Risk Treatment Strategies** |  |
| 🔴 What is Risk Avoidance? | Choosing to eliminate a risk entirely by stopping the associated business activity or removing the vulnerable technology. |
| 🔴 What is Risk Transference? | Sharing or moving the financial burden of a risk to a third party, such as purchasing cybersecurity insurance or outsourcing to a vendor. |
| 🔴 What is Risk Mitigation? | Deploying technical or operational security controls to actively reduce the likelihood or overall impact of a threat. |
| 🔴 What is Risk Acceptance? | Acknowledging a risk exists but deciding to absorb any potential impact because the cost of mitigation outweighs the threat itself. |
| **🟢 Structural Evaluation & Testing** |  |
| 🔴 What are penetration testing boxes? | **Black Box**: Tester has zero prior knowledge of the target; **Grey Box**: Tester has partial or limited knowledge; **White Box**: Tester has full internal knowledge and source code access. |
| 🔴 What is a bug bounty program? | A crowdsourced initiative where independent ethical hackers are financially rewarded for discovering and responsibly reporting vulnerabilities. |

## 📝 Summary

**Risk analysis and assessments** allow organizations to effectively prioritize security budgets by evaluating threats through both qualitative and quantitative methodologies. Qualitative approaches prioritize events visually using a **likelihood vs. impact heat map**, whereas quantitative models analyze risk mathematically by assessing Asset Value (**AV**) and the Exposure Factor (**EF**) to determine the Single Loss Expectancy (**SLE**), which scales into the Annualized Loss Expectancy (**ALE**) when multiplied by the Annualized Rate of Occurrence (**ARO**).

When planning organizational resilience, a Business Impact Analysis (**BIA**) defines structural performance metrics, specifying the maximum tolerable data loss (**RPO**) and system downtime (**RTO**). Once evaluated, risks are addressed using one of four fundamental **risk treatment strategies**: **avoidance**, **transference** (such as buying cyber insurance), **mitigation** via security controls, or baseline **acceptance**. Finally, organizations validate these risk postures internally using a combination of crowdsourced **bug bounty programs** and tiered **penetration testing** exercises (spanning black, grey, and white box scenarios).
