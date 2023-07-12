# Cost Management Power BI samples

The following Power BI reports are very simple starter kits to collect feedback. They all use the Cost Management Power BI connector, which is limited to only Enterprise Agreement billing accounts and Microsoft Customer Agreement billing profiles. If you'd like to see anything, please [submit an issue](https://github.com/flanakin/cost-management-powerbi/issues/new).

Reports:

- [FOCUS](#focus)
- [Cost summary](#cost-summary)
- [Commitment discounts](#commitment-discounts)
- [Cost Management template app](#cost-management-template-app) (Enterprise Agreement only)

To connect to your account, see [Connect reports to your account](#connect-reports-to-your-account)

<br>

> ℹ️ _If you find these reports useful, you might also be interested in [FinOps hubs](https://aka.ms/finops/hubs). FinOps hubs enable you to:_
> 
> - _Connect Power BI to subscriptions, resource groups, and other scopes._
> - _Connect Power BI to Azure Government and Microsoft Online Services Aagreement accounts._
> - _Report on multiple subscriptions, resource groups, or billing accounts._
> - _Coming soon: Ingest data from subscriptions in multiple tenants into a single storage account._
> - _Coming soon: Normalize cost data across account types._
> - _Coming soon: Ingest data into Azure Data Explorer._

<br>

---

<br>

## FOCUS

The **FOCUS report** provides an example of the [FinOps Open Cost and Usage Specification (FOCUS)](https://focus.finops.org) for Azure cost details. The report merges billed (actual) and amortized cost details into a single normalized dataset aligned to the FOCUS schema.

This report comes with sample data to demonstrate the FOCUS schema and collect feedback. You can explore this dataset without connecting to your own account. I encourage anyone who works with cloud cost and usage data to check it out and share feedback about the schema to help improve it for everyone. To learn more about how to contribute to FOCUS, visit [focus.finops.org](https://focus.finops.org).

![Screenshot of the raw data page in the FOCUS sample report](https://github.com/flanakin/cost-management-powerbi/assets/399533/fb48a5b0-5353-4d0c-aad1-458845f702ef)

[Download FOCUS.pbix](https://github.com/flanakin/cost-management-powerbi/raw/main/FOCUS.pbix) and [create an issue](https://github.com/flanakin/cost-management-powerbi/issues/new) to share feedback!

<br>

## Cost summary

The **Cost summary report** provides an overview of amortized costs with a few common breakdowns that enable you to:

- Identify the top cost contributors.
- Review changes in cost over time.
- Build a chargeback report.
- Summarize cost savings from negotiated and commitment-based discounts.

![Screenshot of the summary page in the Cost summary report](https://user-images.githubusercontent.com/399533/216882658-45f026f1-c895-48ca-81e2-35765af8e29e.png)

[Download CostSummary.pbix](https://github.com/flanakin/cost-management-powerbi/raw/main/CostSummary.pbix) and [create an issue](https://github.com/flanakin/cost-management-powerbi/issues/new) to share feedback!

<br>

## Commitment discounts

The **Commitment discounts report** summarizes existing and potential savings from commitment-based discounts, like reservations and savings plans. This report enables you to:

- Review Azure Hybrid Benefit usage.
- Identify and resolve any under-utilized commitments (aka utilization).
- Identify opportunity to save with more commitment-based discounts (aka coverage).
- Determine which resources used commitment-based discounts (aka chargeback).
- Summarize cost savings from commitment-based discounts.

![Screenshot of the utilization page in the Commitment discounts report](https://user-images.githubusercontent.com/399533/216882916-bb7ecfa3-d092-4ae2-88e1-7a0425c14dca.png)

[Download CommitmentDiscounts.pbix](https://github.com/flanakin/cost-management-powerbi/raw/main/CommitmentDiscounts.pbix) and [create an issue](https://github.com/flanakin/cost-management-powerbi/issues/new) to share feedback!

<br>

## Cost Management template app

> ⚠️ _The Cost Management template app is designed to work for **Enterprise Agreement billing accounts only** and will **not** work for Microsoft Customer Agreement billing profiles._

The **Cost Management template app** is the PBIX version of the official [Cost Management app](https://appsource.microsoft.com/product/power-bi/costmanagement.azurecostmanagementapp). Details are covered in [Cost Management documentation](https://learn.microsoft.com/azure/cost-management-billing/costs/analyze-cost-data-azure-cost-management-power-bi-template-app).

Please keep in mind that I am not maintaining this. I am simply making it available for download. If you would like to see something from here incorporated into one of the reports above or you would like to see a new report covering a different area, please [create an issue](https://github.com/flanakin/cost-management-powerbi/issues/new) to share feedback.

[Download CostManagementTemplateApp.pbix](https://github.com/flanakin/cost-management-powerbi/raw/main/CostManagementTemplateApp.pbix).

<br>

---

<br>

## Connect reports to your account

1. Download and open the report in Power BI.
2. Select **Transform data** in the toolbar.
3. Select **Queries** > **Setup** > **Start here** and follow the instructions.
   - If connecting an EA account, set the Billing Account ID to your EA enrollment number.
   - If connecting an MCA account, set the Billing Account ID to your MCA billing account ID and optionally set the Billing Profile ID.
   - Billing profile is optional for cost data, but required for MCA reservation recommendations.
   - Leverage the troubleshooting messages to ensure everything is setup correctly.
4. Select **Close & Apply** in the toolbar and allow Power BI to refresh to see your data.

![Screenshot of the Billing Account ID parameter in Power BI Desktop](https://github.com/flanakin/cost-management-powerbi/assets/399533/766f2a70-abcb-434b-8c1b-b7365afcd68b)

For more details, see [Create to the Azure Cost Management connector in Power BI Desktop](https://learn.microsoft.com/power-bi/connect-data/desktop-connect-azure-cost-management).
