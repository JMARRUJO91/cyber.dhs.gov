---
layout: base
title: Vulnerability Disclosure Policy Template
permalink: /bod/20-01/vdp-template/
redirect_to: https://www.cisa.gov/vulnerability-disclosure-policy-template

---
This page contains a web-friendly version of the Cybersecurity and Infrastructure Security Agency's Binding Operational Directive 20-01 VDP template. See also the [.docx template]({{ site.baseurl }}/assets/report/bod-20-01-vdp-template.docx) and an [example of what a basic web form](https://forms.office.com/Pages/ResponsePage.aspx?id=bOfNPG2UEkq7evydCEI1SqHke9Gh6wJEl3kQ5EjWUKlUMk82UEZET043WFFCUDlUNFI0Q1I5UjM5US4u) to accept submissions looks like.

<span style="color:red">*This template is intended to assist your agency in the creation of a vulnerability disclosure policy (VDP) that aligns with [Binding Operational Directive (BOD) 20-01](https://cyber.dhs.gov/bod/20-01/).*</span>

-   <span style="color:red">*Instructions for how to use the template and some example text are provided throughout the document in red and italic text. These should be changed and removed from your published policy.*</span>

-   <span style="color:red">*You are encouraged to modify the template to suit your needs, but your policy must address all actions required by the Directive. It is **strongly recommended** that you use the template's language for the Authorization section.*</span>

-   <span style="color:red">*CISA recommends that you review the [implementation guidance](https://cyber.dhs.gov/bod/20-01/#compliance-guide) maintained in support of this directive, particularly the section [Consider prior art](https://cyber.dhs.gov/bod/20-01/#consider-prior-art).*</span>

-  <span style="color:red">*Your policy must be published as a public web page in plain text or HTML at the "/vulnerability-disclosure-policy" path of your agency\'s primary .gov website.*</span>

<span style="color:red">*The primary sources for this template were the General Services Administration's [Technology Transformation Services' VDP](https://18f.gsa.gov/vulnerability-disclosure-policy/), the [Department of Defense's VDP](https://hackerone.com/deptofdefense), and a VDP template from a 2016 working group of the [National Telecommunications and Information Administration](https://www.ntia.doc.gov/files/ntia/publications/ntia_vuln_disclosure_early_stage_template.pdf). It has been written to align with the Department of Justice's [Framework for a Vulnerability Disclosure Program for Online Systems](https://www.justice.gov/criminal-ccips/page/file/983996/download).*
</span>

## Vulnerability Disclosure Policy
<span style="color:red">*AGENCY NAME*

<span style="color:red">_Month Day, Year_

### Introduction

<span style="color:red">*An introductory section that provides background information about your organization and your VDP. It should take a committed, concerned, and receptive tone.*

*AGENCY NAME* is committed to ensuring the security of the American public by protecting their information. This policy is intended to give security researchers clear guidelines for conducting vulnerability discovery activities and to convey our preferences in how to submit discovered vulnerabilities to us.

This policy describes **what systems and types of research** are covered under this policy, **how to send us** vulnerability reports, and **how
long** we ask security researchers to wait before publicly disclosing vulnerabilities.

We encourage you to contact us to report potential vulnerabilities in our systems.

### Authorization

<span style="color:red">*This section reflects your commitment to not take legal action against anyone in the general public for security research activities that represent a good faith effort to follow the policy.*</span>

<span style="color:red">*CISA **strongly encourages** keeping this language as-is. The language is designed to be as welcoming to researchers as possible and to avoid "legalese" or other unnecessarily intimidating language.*</span>

**If you make a good faith effort to comply with this policy during your security research, we will consider your research to be authorized we will work with you to understand and resolve the issue quickly, and *AGENCY NAME* will not recommend or pursue legal action related to your research. Should legal action be initiated by a third party against you for activities that were conducted in accordance with this policy, we will make this authorization known.**

### Guidelines

Under this policy, "research" means activities in which you:

-   Notify us as soon as possible after you discover a real or potential security issue.

-   Make every effort to avoid privacy violations, degradation of user experience, disruption to production systems, and destruction or manipulation of data.

-   Only use exploits to the extent necessary to confirm a vulnerability's presence. Do not use an exploit to compromise or exfiltrate data, establish persistent command line access, or use the exploit to pivot to other systems.

-   Provide us a reasonable amount of time to resolve the issue before you disclose it publicly.

-   Do not submit a high volume of low-quality reports.

Once you've established that a vulnerability exists or encounter any sensitive data (including personally identifiable information, financial information, or proprietary information or trade secrets of any party), **you must stop your test, notify us immediately, and not disclose this data to anyone else**.

### Test methods

The following test methods are not authorized:

-   Network denial of service (DoS or DDoS) tests or other tests that impair access to or damage a system or data

-   Physical testing (e.g. office access, open doors, tailgating), social engineering (e.g. phishing, vishing), or any other non-technical vulnerability testing

### Scope

<span style="color:red">*This section defines which internet-accessible systems or services are in scope of your policy. Your first published VDP must contain at least one production system or service, and it must also describe the types of tests that are allowed (or specifically not authorized).*</span>

<span style="color:red">*Alternatively, instead of an **allowlist** that enumerates which systems or services are in scope, you may choose to use a **denylist** to describe which are out of scope.*</span>

*Before adding a system or service to the scope, ensure you are permitted to authorize security testing on the system or service. Specifically, if you, e.g., use a managed service provider or software as a service, confirm whether the vendor has explicitly authorized such testing, such as in your agency's contract with the provider or their publicly available policy. If not, you should work with the vendor to obtain authorization. **If it is not possible to obtain the vendor's authorization, you may not include those systems or services in scope of your policy.***

<span style="color:red">*Note:*</span>

-   <span style="color:red">*After your policy's publication, all newly launched Internet-accessible systems or services must be included* implicitly *in the scope (e.g., by indicating a wildcard \[\*\] on a domain's scope) or* explicitly *by updating the policy to account for these systems.*</span>

-   <span style="color:red">*At 2 years after the issuance of this directive, all internet-accessible systems or services must be in scope of your policy.*</span>

This policy applies to the following systems and services:

-   <span style="color:red">`*.agency-brand.gov`

-   <span style="color:red">`agency-form.gov`

-   <span style="color:red">`agency-service.gov`, and the following hostnames:

    -   <span style="color:red">`alpaca.agency-service.gov`

    -   <span style="color:red">`buffalo.agency-service.gov`

    -   <span style="color:red">`cassowary.agency-service.gov`

    -   <span style="color:red">`dormouse.agency-service.gov`

    -   <span style="color:red">Any other subdomain of `agency-service.gov` and all customer applications are excluded from this policy (`*.app.agency-service.gov` is specifically excluded, except for `*.service-proxy.app.agency-service.gov`.)

-   <span style="color:red">Source code at [https://github.com/agency-example/repo](https://github.com/agency-example/repo)</span>

**Any service not expressly listed above, such as any connected services, are excluded from scope** and are not authorized for testing. Additionally, vulnerabilities found in systems from our vendors fall outside of this policy's scope and should be reported directly to the vendor according to their disclosure policy (if any). If you aren't sure whether a system is in scope or not, contact us at <span style="color:red">security@agency.gov before starting your research (or at the security contact for the system's domain name listed in the [.gov WHOIS](https://domains.dotgov.gov/dotgov-web/registration/whois.xhtml))</span>.

Though we develop and maintain other internet-accessible systems or services, we ask that *active research and testing* only be conducted on the systems and services covered by the scope of this document. If there is a particular system not in scope that you think merits testing, please contact us to discuss it first. We will increase the scope of this policy over time.

<span style="color:red">*If you operate a bug bounty program, you may consider referencing that in your VDP. For example, you could use language such as: "A subset of our systems may be eligible for bounties. Check out \[hyperlink\] for the current list of bounty-eligible systems."*</span>

### Reporting a vulnerability

<span style="color:red">*This section describes communication mechanisms and processes for submitting vulnerabilities. It must include instructions on where reports should be sent (e.g., a web form, email address), and a request for the information your agency needs to find and analyze the vulnerability (e.g., a description of the vulnerability, its location and potential impact; technical information needed to reproduce; any proof of concept code; etc.).*</span>

<span style="color:red">*You must allow vulnerability reporters to submit anonymously: you must not require the submission of personally identifiable information, although you may request the reporter voluntarily provide contact information.*</span>

<span style="color:red">*This is also a good place to pledge your agency to be as transparent as possible about what steps you are taking during the remediation process, as well as set expectations for when the reporter can anticipate acknowledgement of their report.*</span>

*Information submitted under this policy will be used for defensive purposes only -- to mitigate or remediate vulnerabilities. If your findings include newly discovered vulnerabilities that affect all users of a product or service and not solely* Agency Name*, we may share your report with the Cybersecurity and Infrastructure Security Agency, where it will be handled under their [coordinated vulnerability disclosure process](https://www.cisa.gov/coordinated-vulnerability-disclosure-process). We will not share your name or contact information without express permission.*

**We accept vulnerability reports at <span style="color:red">this form</span> or via <span style="color:red">security@agency.gov</span>**. Reports may be submitted anonymously. If you share contact information, we will acknowledge receipt of your report within 3 business days.

We do not support PGP-encrypted emails. For particularly sensitive information, submit through our <span style="color:red">HTTPS web form</span>.

<span style="color:red">*Make sure that any web form you use has a strong HTTPS configuration. Reporters who are concerned about the sensitivity of their report may take steps to verify the HTTPS configuration first, and could be discouraged or alarmed if weak or compromised protocols or ciphers are in use.*</span>

<span style="color:red">*You may consider including the following statement in your VDP and/or by the submission button if you use a webform: "By submitting a vulnerability, you acknowledge that you have no expectation of payment and that you expressly waive any future pay claims against the U.S. Government related to your submission."*</span>

#### What we would like to see from you

In order to help us triage and prioritize submissions, we recommend that your reports:

-   Describe the location the vulnerability was discovered and the potential impact of exploitation.

-   Offer a detailed description of the steps needed to reproduce the vulnerability (proof of concept scripts or screenshots are helpful).

-   Be in English, if possible.

#### What you can expect from us

When you choose to share your contact information with us, we commit to coordinating with you as openly and as quickly as possible.

-   Within 3 business days, we will acknowledge that your report has been received.

-   To the best of our ability, we will confirm the existence of the vulnerability to you and be as transparent as possible about what steps we are taking during the remediation process, including on issues or challenges that may delay resolution.

-   We will maintain an open dialogue to discuss issues.

### Questions
Questions regarding this policy may be sent to <span style="color:red">security@agency.gov</span>. We also invite you to contact us with suggestions for improving this policy.

### Document change history

  | **Version** | **Date** | **Description** |
  | ----------- | -------- | ---------------- |
  | 1.0 | *Month Day, Year* | First issuance. |
