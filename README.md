# Cost Management Power BI samples

These are very simple starter kits used to collect feedback. If you'd like to see anything, please [submit an issue](https://github.com/flanakin/cost-management-powerbi/issues/new).

Reports:

- [Cost summary](#cost-summary)
- [Commitment discounts](#commitment-discounts)

To connect to your account, see [Connect reports to your account](#connect-reports-to-your-account)

<br>

---

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

---

<br>

## Connect reports to your account

1. Download and open the report in Power BI.
2. Select **Transform data** in the toolbar.
3. Select **Queries** > **BillingProfileOrEnrollmentNumber** and update the value to your EA enrollment number of MCA billing profile ID.
4. If using MCA, select **Queries** > **Scope** and change the value to `Billing Profile Id`.
5. Select **Close & Apply** in the toolbar and allow Power BI to refresh to see your data.

![Screenshot of the BillingProfileOrEnrollmentNumber parameter in Power BI Desktop](https://user-images.githubusercontent.com/399533/217879504-e874f66d-0ac5-49f1-a1fc-010be407679c.png)

For more details, see [Create to the Azure Cost Management connector in Power BI Desktop](https://learn.microsoft.com/power-bi/connect-data/desktop-connect-azure-cost-management).
