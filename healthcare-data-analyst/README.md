## Reliance eHealth Collaborative HDA Technical Exercise

The [NPPES NPI Registry](https://npiregistry.cms.hhs.gov/) is a free directory of all active National Provider Identifier (NPI) records. Healthcare providers acquire their unique 10-digit NPIs to identify themselves in a standard way throughout their industry. Provider NPI numbers often occur in healthcare records and claims, and they supply another method of identification in addition to names.

The NPPES NPI Registry also maintains an [API](https://npiregistry.cms.hhs.gov/registry/help-api) in order to allow users to programmatically interface with the registry.

For this technical exercise, we have provided a [flat file](https://github.com/scotttse-rhie/recruiting/blob/master/Healthcare%20Data%20Analyst/data/provider_npi_list.tsv) of provider NPIs pulled from Reliance claims records.  These claims are all from providers that have ordered Lab results on their patients from commercial labs. The schema of the data in the flat file is:

*laboratory*: name of the lab that performed the result in the claim  
*provider_npi*: unique NPI number of the provider  
*claim_id_count*: number of claims for that provider ordered from the laboratory in this row  

We would like you to utilize the NPPES API to answer the following questions:

1) How many claims are there for each lab?
2) Who are the top 25 ordering providers (by NPI number and name)?
3) Of these top 25 providers, what are their addresses?
4) BONUS (OPTIONAL): for the top 25 providers, what are the names of their clinics/facilities (NOTE: to answer this, you will likely need to source data outside of NPPES)?

Please write up your approach in a Python 3.x Jupyter Notebook (1-2 pages) and utilize the Pandas and/or Numpy libraries. You are also welcome and encouraged to use other python libraries that support your analysis. Please explain your work!
