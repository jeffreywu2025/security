Unit 5 Case Study: Reviewing an Assessment Reporting Template:

Introduction

This essay evaluates whether the PurpleSec Sample Vulnerability Assessment Report can be used as a baseline for future penetration testing in line with National Cyber Security Centre (NCSC) expectations, and it critically examines the report’s strengths, weaknesses and practical lessons in relation to vulnerability analysis and secure-system design. The discussion also links the evaluation to the learning outcomes of identifying and analysing vulnerabilities, selecting appropriate methodologies and tools, and critically appraising security solutions for managing risk (NCSC, 2024; NCSC, 2026a).

NCSC baseline expectations

NCSC presents penetration testing as one component of a broader assurance and vulnerability-management process rather than a standalone technical activity (NCSC, 2026a). Its guidance stresses the need to understand the systems in scope, clarify testing objectives, and use security testing to support wider risk management and improvement activities (NCSC, 2026a). In parallel, NCSC’s vulnerability-management guidance emphasises maintaining an inventory of systems, identifying the vulnerabilities that affect them, and measuring how effectively patching and configuration processes reduce exposure over time (NCSC, 2024).
Taken together, this means a useful baseline for later penetration testing should define scope and objectives, document the assets included, describe the methodology used, provide measurable indicators of current security posture, and establish a target control state against which later assessments can be compared (NCSC, 2024; NCSC, 2026a). A baseline is therefore more than a one-off scan result; it is a repeatable reference point for future testing and governance (NCSC, 2024).

Evaluation of the PurpleSec template

The PurpleSec template contains some valuable baseline elements. It states that the purpose of the assessment is to gather data on Windows and third-party software patch levels on specified hosts, identifies that 35 hosts were in scope and 32 were successfully scanned, and records the use of Nessus Professional v8.2.2 on a defined assessment date (PurpleSec, n.d.). These details help future assessors reproduce the technical conditions of the scan and compare broad changes in vulnerability counts over time.

The methodology section is also useful. It explains that the assessment was an internal credentialed patch audit, performed from inside the client environment with valid domain credentials, and that the scan proceeded through network discovery followed by vulnerability assessment (PurpleSec, n.d.). This is consistent with recognised good practice because credentialed internal scans provide deeper visibility into patch levels and configuration weaknesses than purely external or unauthenticated scans (NCSC, 2024).

The report also provides a clear summary of findings. It records 447 unique vulnerabilities across the scanned hosts, broken down into 44 critical, 309 high, 84 medium and 10 low vulnerabilities, and gives examples such as outdated Windows patches, outdated third-party applications, unsupported SQL Server versions and TLS/SSL weaknesses on HP switches (PurpleSec, n.d.). This creates a useful initial snapshot of risk exposure and demonstrates how technical findings can be prioritised through severity categories.

Despite these strengths, the report does not fully meet the NCSC expectation of a baseline that can act as a reference point for future penetration tests. The main weakness is that it does not define the expected control standard or target state. It lists missing patches and configuration problems, but it does not specify measurable requirements such as patching critical vulnerabilities within a defined number of days, prohibiting unsupported software in production, or enforcing modern encryption standards across management interfaces (PurpleSec, n.d.; NCSC, 2024). Without this target state, the report shows the presence of weaknesses but not the degree of deviation from an agreed baseline.

A second weakness is the limited business and asset context. The report counts hosts and notes that some are Windows systems and some are HP switches, but it does not include a structured asset register showing business criticality, system ownership, service role or data sensitivity (PurpleSec, n.d.). NCSC guidance highlights that prioritisation depends not only on technical severity but also on the importance of the affected system to business operations, so the absence of this information weakens the report’s usefulness for later scoping and prioritising penetration tests (NCSC, 2024).

A third weakness concerns the form of the metrics used. The template provides raw numbers of vulnerabilities and several pages of individual KB-level remediation tasks, but it does not translate these into governance-friendly indicators such as patch compliance rates, the percentage of hosts missing at least one critical update, or the number of unsupported systems still in use (PurpleSec, n.d.; NCSC, 2024). As a result, it is difficult to use the document to measure security improvement consistently across time. This limitation is important because contemporary cyber-risk research shows that organisations gain more value when technical security data is transformed into broader management indicators that support prioritisation and decision-making (Liu and Babar, 2026).

A final limitation is that the report does not clearly explain how this assessment will be reused in future penetration testing. Although it mentions that vulnerability scanning is only one tool for assessing security posture and references the possible value of red teaming or penetration testing, it does not define how later testers will use this snapshot to select targets, validate remediation or identify residual risk (PurpleSec, n.d.; NCSC, 2026a). For that reason, the report is better described as a useful technical vulnerability-scan report than a complete NCSC-style testing baseline.

Recommended amendments

Several amendments would make the template more suitable as a formal baseline. First, it should include a dedicated “Baseline Scope and Objectives” section near the beginning of the document. This section should identify the business services in scope, the rationale for testing, the environment type, the frequency of reassessment and the intended use of the baseline in future penetration testing (NCSC, 2024; NCSC, 2026a).
Second, the report should add an asset and criticality register. This should list each host or device, its operating system and version, system role, owner, business criticality and whether it stores or supports sensitive data (NCSC, 2024). It should also explicitly identify excluded or unscanned systems and explain the reason for exclusion, since the current report notes that some hosts were offline or could not be authenticated but does not fully address the risk this creates for assurance coverage (PurpleSec, n.d.).
Third, the template should define measurable control targets. For example, it could state that no unsupported operating systems or database platforms are permitted in production, that all critical vulnerabilities should be remediated within a specified timeframe, and that internal remote management services such as RDP must require Network Level Authentication and strong transport security (NCSC, 2024; Cyber Essentials, 2023). Findings should then be mapped against those targets so the report measures compliance with an agreed security standard rather than merely listing defects.
Fourth, the remediation section should be redesigned. The current report includes many pages of individual KB references, which may be useful operationally but are not effective for management analysis (PurpleSec, n.d.). A better approach would be to summarise remediation at a higher level, such as upgrading unsupported SQL Server instances, standardising Windows patching on the latest cumulative update, or removing obsolete software such as Adobe Flash, while leaving detailed scanner output in an appendix (NCSC, 2024).
Fifth, the report should include a section explaining how the baseline will support future penetration testing. This should clarify which unresolved high-risk findings are likely to become testing priorities, how rescans will validate remediation, and how trend data will support broader assurance decisions (NCSC, 2024; NCSC, 2026a). Adding this section would create a clearer bridge between vulnerability assessment and later exploit-based testing.

Two strongest lessons from the report

One of the best lessons in the report is the value of credentialed internal scanning. The methodology explicitly states that domain credentials were used from within the network perimeter to gather detailed information about patch levels and configuration, showing that the assessment was designed to reveal weaknesses that a surface-level external scan might miss (PurpleSec, n.d.). This is a strong example of selecting an appropriate methodology and tool for identifying security vulnerabilities in network systems, which directly supports the module learning outcome on analysis of threats and vulnerabilities (NCSC, 2024).
The second strong lesson is the report’s risk-based remediation logic. The remediation section shows that actions across nine hosts would resolve 20 per cent of the vulnerabilities on the network, illustrating that security teams should focus first on shared components and common weaknesses that deliver the greatest reduction in exposure (PurpleSec, n.d.). This demonstrates how vulnerability data can be turned into practical, prioritised action, supporting the learning outcome about designing and appraising solutions that manage and audit security risk (NCSC, 2024).

Two weaker elements

One weaker element is the excessive amount of low-level remediation detail in the main body of the report. The long list of individual KB patches makes the report harder to interpret strategically and obscures broader patterns such as legacy operating systems, outdated browsers or ineffective patch cycles (PurpleSec, n.d.). A grouped, control-focused summary would be more effective for decision-making and for establishing a reusable baseline (NCSC, 2024).
Another weaker element is the generic password-policy guidance. The final section includes recommendations on password history, password length and account lockout settings, but these are not linked to evidence gathered during the assessment and are therefore analytically weaker than the report’s core vulnerability findings (PurpleSec, n.d.). Policy recommendations should ideally be supported by observed misconfigurations or by a clear comparison against recognised baseline standards so that they contribute directly to risk analysis rather than appearing as a generic best-practice appendix (Cyber Essentials, 2023; NCSC, 2024).
Use of wider sources

Recent peer-reviewed research supports the argument that vulnerability assessments should feed a broader, evidence-based process of cyber-risk management. Liu and Babar (2026) argue that organisations gain more value when technical vulnerability data is converted into governance-level indicators that support prioritisation, investment decisions and continuous improvement. Murthy, Verma and Singh (2024) similarly show that systematic analysis of breach patterns over time helps identify recurring weaknesses and improves proactive defence, reinforcing the need for baselines that can be revisited and compared rather than treated as static, one-off reports.
These sources strengthen the critique of the PurpleSec template. The report is useful as a technical scan output, but it would become more effective if it transformed raw findings into metrics, trend indicators and service-level risk insights that could support long-term assurance and targeted penetration testing (Liu and Babar, 2026; Murthy, Verma and Singh, 2024).

Reflection

This activity involved several challenges. One challenge was distinguishing between a technically competent vulnerability-scan report and a complete NCSC-style baseline for future penetration testing, because the two are related but not identical (NCSC, 2024; NCSC, 2026a). Another challenge was translating a large amount of technical detail into a critical academic evaluation that addressed both industry guidance and module learning outcomes.
These challenges were overcome by comparing the PurpleSec report structure against NCSC guidance on penetration testing and vulnerability management, and by using recent peer-reviewed literature to frame the discussion around governance, metrics and systematic analysis rather than only technical findings (NCSC, 2024; NCSC, 2026a; Liu and Babar, 2026). This approach helped show that the template is useful but incomplete, and that a stronger baseline would include clearer scope, asset context, measurable targets and links to future testing.
This will affect the final report positively because it highlights the importance of designing a vulnerability assessment that is repeatable, measurable and aligned with business risk. A final submission informed by this reflection would include explicit baseline metrics, an asset register, evidence-based recommendations and a clear explanation of how assessment results support later penetration testing and ongoing cyber-risk management (NCSC, 2024; Liu and Babar, 2026).

References

Cyber Essentials (2023) Cyber Essentials requirements for IT infrastructure. 

Liu, C. and Babar, M.A. (2026) ‘Corporate cybersecurity risk and data breaches: A systematic review of empirical research’, Australian Journal of Management, 51(1), pp. 62-92.

Murthy, A.S.R.C., Verma, P. and Singh, R. (2024) ‘An in-depth analysis of contemporary security breaches using time series analysis’, in Proceedings of ICCIET 2024. Paris: Atlantis Press, pp. 701-709.

National Cyber Security Centre (NCSC) (2024) Vulnerability management. 

National Cyber Security Centre (NCSC) (2026a) Penetration testing. 

National Cyber Security Centre (NCSC) (2026b) CHECK penetration testing. 

PurpleSec (n.d.) Sample Vulnerability Assessment Report – Example Institute. PDF file provided as course material.


