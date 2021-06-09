# Banking Marketing Prediction

## Dataset
The dataset contains information about direct marketing campaign (phone calls) of a Portuguese banking institution.

Disclamer: Dataset is based on publicly available Bank Marketing dataset (link)

## Attributes
### Clients' data
  - age (numeric)
  - job: type of job (categorical: "admin.", "blue-collar", "entrepreneur", "housemaid", "management", "retired", "self-employed", "services", "student", "technician", "unemployed", "unknown")
  - marital: marital status (categorical: "divorced","married","single","unknown"; note: "divorced" means divorced or widowed)
  - education (categorical: "basic.4y", "basic.6y", "basic.9y", "high.school","illiterate", "professional.course", "university.degree", "unknown")
  - default: has credit in default? (categorical: "no","yes","unknown")
  - housing: has housing loan? (categorical: "no","yes","unknown")
  - loan: has personal loan? (categorical: "no","yes","unknown")

### Target data
  - test_control_flag: contains information if the person was part of the campaign ("campaign group") or control group ("control group"). Campaign group was called (details on the contact below) and offered term deposit. All customers could subscribe to the deposit (also control group)  
  - y: has the client subscribed a term deposit? (binary: "yes","no")

### Data related with the last contact of the current campaign
  - contact: contact communication type (categorical: "cellular","telephone")
  - month: last contact month of year (categorical: "jan", "feb", "mar", ..., "nov", "dec")
  - day_of_week: last contact day of the week (categorical: "mon","tue","wed","thu","fri")
  - duration: last contact duration, in seconds (numeric)
  - campaign: total number of contacts performed during this campaign and for this client (numeric, includes last contact)

### Data about previous campaigns
  - pdays: number of days that passed by after the client was last contacted from a previous campaign (numeric; 999 means client was not previously contacted)
  - previous: number of contacts performed before this campaign and for this client (numeric)
  - poutcome: outcome of the previous marketing campaign (categorical: "failure","nonexistent","success")

### Social and economic context attributes
Data gathered for the day the day of subscription to the term deposit.

  - emp.var.rate: employment variation rate - quarterly indicator (numeric)
  - cons.price.idx: consumer price index - monthly indicator (numeric)
  - cons.conf.idx: consumer confidence index - monthly indicator (numeric)
  - euribor3m: euribor 3 month rate - daily indicator (numeric)
  - nr.employed: number of employees - quarterly indicator (numeric)
