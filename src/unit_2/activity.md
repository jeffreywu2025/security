Unit2: Vulnerability Analysis – Literature Review Activity
----------------
Based on the information identified about your assigned websites, carry out a literature search/ audit on software sites and the national vulnerabilities database to create a baseline audit on potential vulnerabilities with websites.

1. Introduction
   
Web applications continue to represent one of the most significant attack surfaces within modern information systems due to their exposure to the internet, dependence on user interaction and integration with backend databases and authentication mechanisms. As organisations increasingly rely on online platforms for financial transactions, communication and data storage, cybercriminals continue to target web applications through a variety of attacks including SQL injection, cross-site scripting and authentication bypass techniques. Consequently, vulnerability assessment has become an essential component of information security management and risk mitigation.

The purpose of this report is to conduct a baseline vulnerability audit and assessment of the Zero WebApp Security training application. The assessment focuses on identifying potential web application vulnerabilities through manual inspection, literature review and analysis of publicly available vulnerability intelligence sources. The report evaluates the possible security risks associated with common web application weaknesses and examines how such vulnerabilities may affect the confidentiality, integrity and availability of information systems.

The Zero WebApp Security application is intentionally designed as a vulnerable web application training environment for educational purposes. This makes the platform suitable for studying common web security weaknesses and understanding how vulnerabilities may be identified and analysed within a controlled environment. The assessment was conducted ethically and remained limited to passive inspection and vulnerability research activities. No exploitative or destructive testing was performed during the audit.
The report additionally incorporates findings from academic literature, the National Vulnerability Database (NVD), Common Vulnerabilities and Exposures (CVE) records and the OWASP Top 10 framework in order to establish an evidence-based vulnerability analysis. The combination of academic research and practical observation provides a structured methodology for evaluating security risks and recommending mitigation strategies.

2. Aim and Objectives
   
The aim of this assessment is to perform a baseline vulnerability audit of the Zero WebApp Security training application in order to identify potential security weaknesses and analyse the associated risks affecting web application security.
The objectives of the assessment are to identify common web application vulnerabilities within the assigned website, analyse the potential impact of identified weaknesses, evaluate vulnerability information gathered from academic and professional sources, examine recognised vulnerability databases and recommend appropriate mitigation strategies and security controls. The assessment also aims to demonstrate an understanding of vulnerability assessment methodologies and professional security reporting practices.

3. Scope of Assessment
4. 
The scope of the assessment was limited to passive inspection and vulnerability research activities conducted against the Zero WebApp Security training environment. The assessment focused on analysing publicly accessible functionality including authentication pages, search functionality, account management features and transaction-related components that may present potential security weaknesses.
The assessment specifically considered vulnerabilities associated with web application input validation, authentication controls, access control mechanisms, information disclosure and general web application misconfiguration. The methodology involved manual navigation of the application and comparison of observed features against known vulnerability categories identified within academic literature and industry security guidance.

No exploitative penetration testing, denial-of-service activity, password brute-forcing or destructive scanning was conducted during the assessment. The audit was performed solely for academic and educational purposes within an authorised training environment.

4. Methodology
5. 
The vulnerability assessment was conducted using a structured methodology designed to support baseline web application security analysis. The methodology combined manual website inspection, literature review and vulnerability intelligence analysis.
The first stage of the assessment involved manual inspection of the Zero WebApp Security application in order to identify visible functionality, user interaction points and application features that may present security risks. Particular attention was given to login systems, search forms, URL parameters and transaction-based functionality because these areas commonly present vulnerabilities within web applications.

The second stage involved a literature review of recent peer-reviewed academic studies relating to web application security vulnerabilities. Academic databases and scholarly publications were used to identify current research regarding SQL injection, cross-site scripting, vulnerability assessment methodologies and web application risk management.
The third stage involved the analysis of recognised vulnerability intelligence sources including the National Vulnerability Database, Common Vulnerabilities and Exposures records and OWASP security guidance. These sources were used to examine common vulnerability categories, attack techniques and mitigation approaches relevant to modern web applications.

The final stage of the assessment involved analysing identified weaknesses according to potential exploitability, business impact and security implications. Appropriate mitigation strategies and best practice security controls were then recommended based on academic research and recognised industry guidance.

5. Vulnerability Analysis and Literature Review
   
Web applications remain one of the most frequently targeted areas within cyber security due to their accessibility, complexity and reliance on user-generated input. According to Aslan et al. (2023), modern cyber-attacks continue to exploit weaknesses in software configuration, coding practices and network-connected services, resulting in substantial financial and operational damage to organisations. The increasing sophistication of cyber threats has therefore made vulnerability assessment an essential security process for organisations seeking to identify and mitigate security weaknesses before exploitation occurs.

Current literature suggests that vulnerability assessment should involve a layered and systematic methodology rather than relying exclusively on automated tools. Bennouk et al. (2024) argue that effective vulnerability assessment combines manual inspection, automated scanning, penetration testing methodologies and vulnerability intelligence gathered from recognised databases. This supports the approach adopted within the current assessment, where manual website inspection was combined with academic research and vulnerability database analysis.

One of the most significant vulnerabilities affecting web applications is SQL injection. SQL injection occurs when user input is improperly validated and incorporated directly into backend database queries, potentially allowing attackers to manipulate database commands and retrieve unauthorised information. Paul et al. (2024) explain that SQL injection vulnerabilities continue to affect modern applications because many systems still fail to implement secure coding practices and parameterised query structures. Choi et al. (2025) further note that SQL injection attacks may result in authentication bypass, database compromise and unauthorised disclosure of sensitive information.

Within the Zero WebApp Security application, several user input fields and transactional components appear capable of accepting dynamic user input, indicating the potential for injection-based vulnerabilities if backend validation mechanisms are insufficient. Search functionality, login forms and account-related parameters may therefore represent possible SQL injection attack surfaces. The OWASP Top 10 framework also identifies injection vulnerabilities as one of the most critical web application security risks (OWASP, 2025).

Cross-site scripting represents another major web application security concern identified within recent academic research. Alhamyani et al. (2024) describe cross-site scripting as a vulnerability that enables attackers to inject malicious client-side scripts into trusted web pages. When executed within a victim’s browser, these scripts may compromise session information, manipulate user interactions or redirect users to malicious resources. Younas et al. (2024) additionally explain that reflected and stored XSS vulnerabilities continue to present significant risks to applications containing interactive user functionality.

The Zero WebApp Security application includes multiple user interaction features involving search forms, account messaging and data input mechanisms. Such functionality may potentially allow malicious scripts to be reflected or stored within application responses if output encoding and input sanitisation controls are not properly implemented. The impact of successful cross-site scripting attacks may include session hijacking, credential theft and compromise of user trust.

Authentication weaknesses also remain highly significant within modern web application security. Weak authentication controls, insecure password policies and insufficient session management mechanisms may allow attackers to gain unauthorised access to user accounts and sensitive information. Research by Tanveer et al. (2025) highlights the growing prevalence of broken authentication and access control weaknesses within modern web applications and APIs.

The Zero WebApp Security training application intentionally demonstrates insecure authentication mechanisms for educational purposes. Observations from the assessment indicate that the application may expose weak account protection controls and insufficient authentication safeguards. Such weaknesses increase the likelihood of unauthorised account access and privilege escalation if exploited by malicious actors.

Information disclosure vulnerabilities also represent a significant security concern because attackers frequently rely on publicly accessible information during reconnaissance activities. Information disclosure may occur through verbose error messages, exposed directories, server information leakage or publicly accessible configuration files. According to Li et al. (2023), vulnerability intelligence databases demonstrate that information leakage frequently contributes to successful attack planning and exploitation.
During the assessment, publicly accessible application information and visible error-handling behaviour suggested the potential for information disclosure risks within the training environment. Such weaknesses may assist attackers in identifying technologies, frameworks and application structures that could later be targeted through more advanced attacks.

Recent research additionally highlights both the value and limitations of automated vulnerability scanning technologies. Seara et al. (2024) explain that automated scanners improve vulnerability detection efficiency by rapidly identifying known weaknesses and configuration issues. However, Kaya (2025) argues that automated scanners may produce false positives or fail to identify complex vulnerabilities requiring contextual analysis and human interpretation. This demonstrates the importance of combining automated analysis with professional judgement and manual assessment.

The OWASP Top 10 framework remains one of the most widely recognised industry standards for web application security analysis. The framework identifies critical categories including injection attacks, broken access control, security misconfiguration and cryptographic failures (OWASP, 2025). Although OWASP guidance is not peer-reviewed academic literature, it provides a practical and widely accepted benchmark for vulnerability classification and risk analysis.

Overall, the literature strongly supports the use of a layered and evidence-based vulnerability assessment methodology. The combination of manual inspection, vulnerability database analysis, academic research and security frameworks provides an effective foundation for baseline vulnerability assessment and risk evaluation.

6. Findings and Analysis
   
The findings identified during the assessment were evaluated according to their potential impact on the confidentiality, integrity and availability of information systems. This approach supports the CIA triad model, which remains a fundamental principle within information security risk management. Vulnerabilities capable of exposing sensitive information primarily affect confidentiality, while vulnerabilities enabling unauthorised modification of information threaten system integrity. Authentication weaknesses and denial of service risks may additionally affect system availability.

Manual inspection of the Zero WebApp Security application identified several visible attack surfaces including login functionality, dynamic search fields, account management features and URL parameter handling mechanisms. These components increase the application’s exposure to common web application attacks because they rely heavily on user-controlled input and backend processing. The assessment therefore focused on analysing how these exposed functionalities may contribute to injection-based attacks, access control weaknesses and information disclosure risks.
The assessment identified several potential vulnerabilities commonly associated with web applications and recognised within modern cyber security literature. Although no exploitative testing was conducted, manual inspection and literature-supported analysis suggest that the Zero WebApp Security application contains several areas that may expose security risks.
One of the most significant findings relates to potential SQL injection exposure. The application contains multiple dynamic input fields associated with authentication and transactional functionality. Such components may present injection risks if backend database queries fail to implement parameterised input handling and secure validation controls. SQL injection vulnerabilities may allow attackers to manipulate database operations, retrieve confidential information or bypass authentication systems. Given the prevalence of SQL injection attacks within modern web applications, this vulnerability category represents a high-risk concern.
Potential cross-site scripting vulnerabilities were also identified during the assessment. User-controlled input functionality and dynamic content generation mechanisms may permit malicious client-side script execution if appropriate sanitisation and output encoding procedures are absent. Successful exploitation of XSS vulnerabilities may result in session compromise, credential theft and malicious content injection. The presence of interactive user functionality within the application increases the relevance of this vulnerability category.

The assessment additionally identified concerns relating to authentication security and access control mechanisms. The training environment intentionally demonstrates weak authentication practices for educational purposes, including simplified login processes and reduced account protection mechanisms. Weak authentication controls increase the likelihood of unauthorised account access and privilege escalation. Furthermore, broken access control vulnerabilities may allow users to access restricted functionality or manipulate account-related parameters beyond their authorised permissions.

Information disclosure risks were also identified within the application environment. Publicly visible application behaviour and error handling mechanisms may expose technical information regarding application structure, server configuration or underlying technologies. Such information may assist attackers during reconnaissance activities and contribute to future exploitation attempts.
The findings collectively demonstrate that modern web applications remain exposed to a range of common security vulnerabilities when secure coding practices, input validation controls and authentication mechanisms are insufficiently implemented. The assessment additionally highlights the importance of continuous vulnerability management and secure application development practices.

7. Recommendations
8. 
The findings of the assessment indicate that multiple security controls should be implemented in order to reduce the likelihood of successful exploitation and improve the overall security posture of the application.

Input validation mechanisms should be strengthened through the implementation of parameterised database queries and secure server-side validation processes. Parameterised queries significantly reduce the likelihood of SQL injection vulnerabilities by preventing malicious user input from being interpreted as executable database commands.

Cross-site scripting risks may be mitigated through comprehensive output encoding, input sanitisation and content security policies. Applications should ensure that user-generated content is properly validated and encoded before being rendered within browser environments.

Authentication security should be improved through the implementation of strong password policies, multi-factor authentication and secure session management controls. Account lockout mechanisms and secure credential storage practices should additionally be implemented to reduce the likelihood of brute-force attacks and credential compromise.
Information disclosure risks may be reduced through secure error handling procedures and the removal of unnecessary technical information from publicly accessible application responses. Generic error messages should replace verbose system-generated responses that may reveal sensitive implementation details.

Regular vulnerability assessments and security reviews should be conducted in order to identify newly emerging threats and maintain an effective security posture. Organisations should additionally implement continuous monitoring, patch management and secure software development lifecycle practices in order to support long-term vulnerability management.

8. Conclusion
9. 
This report presented a baseline vulnerability audit and assessment of the Zero WebApp Security training application. The assessment identified several common web application vulnerabilities including potential SQL injection exposure, cross-site scripting risks, authentication weaknesses, access control concerns and information disclosure issues.

The findings of the assessment demonstrate that web applications remain vulnerable to a variety of cyber threats when secure coding practices, authentication controls and vulnerability management procedures are insufficiently implemented. The assessment also highlights the importance of combining manual inspection, academic research and vulnerability intelligence sources when conducting security analysis.

The literature review demonstrated that vulnerabilities such as SQL injection and cross-site scripting continue to represent significant threats within modern web environments. Academic research additionally supports the use of layered security methodologies involving vulnerability assessment, secure coding practices and continuous security monitoring.

Overall, the assessment demonstrates that vulnerability management remains a critical component of information security governance. Implementing secure coding standards, strong authentication controls and continuous vulnerability assessment procedures significantly improves organisational resilience against modern cyber threats.

9. Reflection
    
One of the primary challenges encountered during this activity involved understanding the large volume of technical information available within vulnerability databases such as the National Vulnerability Database and CVE records. Many vulnerability entries contained complex technical terminology, exploit descriptions and vulnerability scoring mechanisms that were initially difficult to interpret. As a result, distinguishing between theoretical vulnerabilities and vulnerabilities directly relevant to the assigned website required additional research and analysis.

Another challenge involved evaluating the reliability and relevance of available security information sources. Some publicly available vulnerability discussions and security articles contained inconsistent or conflicting information regarding vulnerability severity and exploitability. This created difficulty when attempting to determine which sources were academically appropriate and sufficiently credible for inclusion within the report.

These challenges were overcome through the use of multiple academic and professional sources in order to cross-reference vulnerability information and improve understanding of common web application security weaknesses. Peer-reviewed journal articles provided valuable theoretical explanations regarding vulnerability categories and security risks, while OWASP guidance offered practical classification frameworks for analysing web application vulnerabilities. Additional research into CVSS scoring systems and vulnerability management methodologies also improved the ability to evaluate vulnerability severity and prioritisation.

The challenges experienced during the assessment positively influenced the quality of the final report by encouraging a more analytical and evidence-based approach to vulnerability assessment. The process improved understanding of vulnerability research methodologies, web application security concepts and professional security reporting standards. The experience also highlighted the importance of critically evaluating security information sources and combining multiple forms of evidence when conducting cyber security analysis.
Overall, the activity significantly improved understanding of vulnerability assessment processes and demonstrated the importance of structured security analysis within modern information security management.

10. References
    
Alhamyani, R., Alotaibi, A., Alshamrani, A. et al. (2024) ‘Machine learning-driven detection of cross-site scripting attacks’, Information, 15(7), p. 420.

Aslan, Ö., Aktuğ, S.S., Ozkan-Okay, M., Yilmaz, A.A. and Akin, E. (2023) ‘A comprehensive review of cyber security vulnerabilities, threats, attacks, and solutions’, Electronics, 12(6), p. 1333.

Bennouk, K., Ait Aali, N., El Bouzekri El Idrissi, Y., Sebai, B., Faroukhi, A.Z. and Mahouachi, D. (2024) ‘A comprehensive review and assessment of cybersecurity vulnerability detection methodologies’, Journal of Cybersecurity and Privacy, 4(4), pp. 853–908.

Choi, J. et al. (2025) ‘Comparative analysis of SQL injection defence mechanisms’, Applied Sciences, 15(23), p. 12351.

Kaya, M. (2025) ‘Evaluation of automated web vulnerability scanning technologies’, Cyber Security and Applications, 3, pp. 44–58.

Li, X. et al. (2023) ‘The anatomy of a vulnerability database: A systematic mapping study’, Information and Software Technology, 163.

Open Worldwide Application Security Project (OWASP) (2025) OWASP Top 10: The ten most critical web application security risks. Available at: OWASP Top 10 (Accessed: 9 May 2026).

Paul, A. et al. (2024) ‘SQL injection attack: Detection, prioritization and prevention’, Journal of Information Security and Applications.

Seara, J.P. et al. (2024) ‘Automation of system security vulnerabilities detection’, Electronics, 13(5), p. 873.

Tanveer, F. et al. (2025) ‘A survey on RESTful API vulnerability detection’, Computer Standards and Interfaces.

Younas, F. et al. (2024) ‘An efficient artificial intelligence approach for early detection of cross-site scripting attacks’, Intelligent Systems with Applications.

