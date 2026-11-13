
# Research Log: Tax Management System (TMS)

**Phase 0 – Step 3: Research the Problem**  
**Date:** 12 November 2026  
**Project:** Tax Management System (TMS)  
**Country of focus:** Rwanda

## 1. The Problem

Many businesses in Rwanda find it difficult to manage their tax obligations, remember payment deadlines and understand the penalties that may apply when they pay late. Without an organised way to track these responsibilities, businesses may miss deadlines, face penalties and have difficulties maintaining tax compliance.

The proposed Tax Management System (TMS) will help businesses record their tax obligations, monitor payment deadlines, track paid and unpaid taxes, estimate possible late-payment penalties, receive deadline reminders and generate tax compliance reports. The system will support businesses in managing their tax information. It will not replace the official tax declaration and payment services provided by the Rwanda Revenue Authority (RRA).

## 2. Research Sources

| # | Source (APA) | Type | Link | Key finding | Gap it shows |
|---|---|---|---|---|---|
| 1 | Mascagni, G., Nell, C., & Monkam, N. (2017). *One size does not fit all: A field experiment on the drivers of tax compliance and delivery methods in Rwanda* (ICTD Working Paper 58). International Centre for Tax and Development. | Research paper | [ICTD publication](https://ictd.ac/publication/ictd-wp58/) | The study examined messages sent by the Rwanda Revenue Authority during the 2016 tax filing period. It found that reminders and friendly messages could improve taxpayer compliance. It also showed that SMS and email were effective ways of reaching taxpayers. | The study focuses on communication from the tax authority. It does not provide a business-side system for organising different tax obligations, payment records and deadlines in one place. |
| 2 | Mascagni, G., Santoro, F., Mukama, D., Karangwa, J., & Hakizimana, N. (2022). Active ghosts: Nil-filing in Rwanda. *World Development, 152*, Article 105806. https://doi.org/10.1016/j.worlddev.2021.105806 | Research paper | [ScienceDirect](https://www.sciencedirect.com/science/article/pii/S0305750X21004216) | The research studied nil-filing among taxpayers in Rwanda using tax administration data and other research methods. It found that nil-filing was common, especially among small and young businesses. The study explains that confusion about tax obligations and the tax system can contribute to this behaviour. | The findings show that some businesses have difficulties understanding their tax responsibilities. The proposed TMS will help businesses organise their obligations and see the deadlines they need to follow. |
| 3 | Ntahondereye, A., & Ntakirutimana, E. (2023). Assessment of tax enforcement in selected small and medium enterprises (SMEs) in Kigali City, Rwanda. *East Africa Journal of Science and Technology, 13*(1), 15–29. | Research paper | [Full research paper](https://site.unilak.ac.rw/wp-content/uploads/2023/12/Elisonetal.pdf) | The researchers used questionnaires involving 99 SME owners in Kigali. The study found that taxpayers rated their understanding of the tax system at a moderate level and the training they received from RRA at a low level. Respondents also reported difficulties understanding and paying their tax liabilities. | The research identifies challenges related to tax knowledge and compliance among SMEs. It recommends improvements in taxpayer education but does not develop a software tool for tracking tax obligations and payment deadlines. |
| 4 | World Bank. (2020). *Doing Business 2020: Economy profile, Rwanda*. World Bank Group. | Report / statistics | [World Bank report](https://www.worldbank.org/content/dam/doingBusiness/country/r/rwanda/RWA.pdf) | The report indicates that Rwanda had 9 tax payments per year and 91 hours of tax compliance time for the standard business used in the study. It also reports a total tax and contribution rate of 33.2% of profit. | The figures show that tax compliance involves several payments and time. However, the report does not explain how individual businesses organise their tax deadlines and payment records. The figures represent a standard business, not every business in Rwanda. |
| 5 | Rwanda Revenue Authority. (n.d.). *Declare employment tax (PAYE).* | Existing system / official tax service | [RRA – Declare PAYE](https://www.rra.gov.rw/en/domestic-tax-services/employment-tax-paye/declare-paye) | RRA provides online tax declaration through E-Tax (MyRRA). Its PAYE page explains penalties for late declaration, late payment and late-payment interest. The penalties depend on the type of violation and the period of delay. | RRA provides official tax declaration services and penalty information. The proposed TMS will focus on helping a business organise and monitor its own tax obligations, deadlines and payment records. It will complement, not replace, RRA services. |
| 6 | National Institute of Statistics of Rwanda. (2024). *Rwanda Establishment Census 2023* (Reference ID: rwa-nisr-rec-2023-V0.1) [Data set]. NISR Microdata Catalog. | Dataset | [NISR dataset and data dictionary](https://microdata.statistics.gov.rw/index.php/catalog/112/datafile/F4) | The dataset contains 269,194 records and 68 variables. The variables include information about establishments, such as location, business size, registration and business characteristics. Some variables relate to tax registration and taxes paid by establishments. | The dataset can help understand the characteristics of Rwandan businesses and guide the design of the TMS. However, it does not provide actual tax payment deadlines, payment dates or penalty transactions. Those records will need to be created separately for the system. |
| 7 | Oracle. (n.d.). *Using the Scheduler*. In *Oracle Database Administrator's Guide (10g Release 2).* | Technical source / Oracle documentation | [Oracle Scheduler documentation](https://docs.oracle.com/cd/B19306_01/server.102/b14231/scheduse.htm) | Oracle Scheduler allows database jobs to run PL/SQL blocks or stored procedures at scheduled times. It supports recurring jobs, which can be used to perform regular database tasks. | Oracle Scheduler can support automatic checks for upcoming and overdue tax deadlines. However, the application must still define the correct tax deadlines, reminder conditions and penalty calculations using PL/SQL. This documentation is for Oracle 10g Release 2, so the implementation will be checked against the Oracle version used in the project. |

## 3. Research Gap

The reviewed sources discuss tax compliance, taxpayer communication, tax enforcement, tax compliance costs and official online tax declaration services in Rwanda.

The research shows that businesses can experience difficulties understanding their tax responsibilities and maintaining compliance. It also shows that reminders can help taxpayers remember their obligations.

RRA already provides official online tax services. However, the sources reviewed do not establish whether businesses have a single business-side tool that brings together their different tax obligations, payment deadlines, payment records, estimated penalties and compliance reports.

The proposed Tax Management System will address this area by providing a central place where businesses can organise and monitor their tax information. It will use Oracle PL/SQL to manage the database operations, calculate outstanding balances, estimate penalties based on verified rules and check upcoming deadlines.

## 4. Summary of Research Findings

The seven sources helped identify the following points:

1. **Tax reminders can improve compliance:** The Rwanda field experiment shows that reminders can encourage taxpayers to meet their obligations.
2. **Tax obligations can be difficult to understand:** The nil-filing research identifies confusion about tax responsibilities as one of the issues affecting taxpayers.
3. **SMEs face tax-related challenges:** The Kigali SME study reports difficulties related to tax understanding, training and payment.
4. **Tax compliance involves time and several payments:** The World Bank report provides evidence of the time and payments involved for its standard business.
5. **Official online tax services already exist:** RRA provides online declaration services and publishes information about tax penalties.
6. **Business data is available:** The NISR Establishment Census provides information about Rwandan businesses that can guide the system's design.
7. **Automatic database tasks are possible:** Oracle Scheduler can run scheduled PL/SQL procedures to check deadlines and create reminders.

## 5. Dataset Information

**Dataset name:** Rwanda Establishment Census 2023  
**Producer:** National Institute of Statistics of Rwanda (NISR)  
**Reference ID:** rwa-nisr-rec-2023-V0.1  
**Number of records:** 269,194  
**Number of variables:** 68  
**Dataset link:** https://microdata.statistics.gov.rw/index.php/catalog/112/datafile/F4

The dataset contains information about Rwandan establishments, including business characteristics, location, size and tax-related registration information.

The dataset will help guide the design of the business and tax-type information in the proposed system. It does not contain actual tax payment transactions, deadlines or penalty records. These will be represented using separately prepared sample records during system development.

**Access and usage note:** The NISR catalogue provides access information and a release policy. The microdata must be obtained and used according to the conditions stated by NISR. The data dictionary and catalogue information were reviewed for this research.

## 6. Conclusion

The research confirms that tax compliance and tax management are important issues for businesses in Rwanda. The reviewed studies identify challenges related to tax knowledge, reminders and compliance, while official sources show that online tax declaration and penalty information are already available.

Based on these findings, the proposed Tax Management System will focus on helping businesses organise their tax obligations, monitor payment deadlines, record payments, estimate possible penalties and generate reports. The system will use Oracle Database and PL/SQL to manage the main business rules and database operations.

## 7. References

1. Mascagni, G., Nell, C., & Monkam, N. (2017). *One size does not fit all: A field experiment on the drivers of tax compliance and delivery methods in Rwanda* (ICTD Working Paper 58). International Centre for Tax and Development. https://ictd.ac/publication/ictd-wp58/

2. Mascagni, G., Santoro, F., Mukama, D., Karangwa, J., & Hakizimana, N. (2022). Active ghosts: Nil-filing in Rwanda. *World Development, 152*, Article 105806. https://doi.org/10.1016/j.worlddev.2021.105806

3. Ntahondereye, A., & Ntakirutimana, E. (2023). Assessment of tax enforcement in selected small and medium enterprises (SMEs) in Kigali City, Rwanda. *East Africa Journal of Science and Technology, 13*(1), 15–29. https://site.unilak.ac.rw/wp-content/uploads/2023/12/Elisonetal.pdf

4. World Bank. (2020). *Doing Business 2020: Economy profile, Rwanda*. World Bank Group. https://www.worldbank.org/content/dam/doingBusiness/country/r/rwanda/RWA.pdf

5. Rwanda Revenue Authority. (n.d.). *Declare employment tax (PAYE).* https://www.rra.gov.rw/en/domestic-tax-services/employment-tax-paye/declare-paye

6. National Institute of Statistics of Rwanda. (2024). *Rwanda Establishment Census 2023* (Reference ID: rwa-nisr-rec-2023-V0.1) [Data set]. NISR Microdata Catalog. https://microdata.statistics.gov.rw/index.php/catalog/112/datafile/F4

7. Oracle. (n.d.). *Using the Scheduler*. In *Oracle Database Administrator's Guide (10g Release 2).* https://docs.oracle.com/cd/B19306_01/server.102/b14231/scheduse.htm
