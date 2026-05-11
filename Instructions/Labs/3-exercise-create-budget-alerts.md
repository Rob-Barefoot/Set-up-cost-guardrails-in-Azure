---
lab:
    title: 'Exercise - Create budget and alerts'
    description: 'Exercise - Create budget and alerts'
    duration: '7 minutes'
    level: 300 <!-- 100 basic concepts, 200 foundations, 300 practical usage, 400 advanced scenarios, 500 expert design -->
    islab: true <!-- if not a lab, remove -->
---

This guided project consists of the following exercises:

 - Apply cost-tracking tags
 - **Create budget and alerts**
 - Assign and test Azure Policy

In this exercise, you create a budget with alert thresholds that notify you before spending exceeds your target. Budget alerts give you early warning so you can investigate and adjust before costs get out of control.

This exercise includes the following tasks:

 - Open Cost Management and start the budget
 - Configure and create the budget

**Outcome:** Budget thresholds configured with actionable notifications.

## Task 1: Open Cost Management and start the budget

Navigate to the Cost Management service where you define spend limits and alerts. This is the central place to monitor and control cloud spending across your subscription and resources.

1.  In the portal search bar, search for **Cost Management** and select **Cost Management**.
2.  In the left menu, under **Monitoring**, select **Budgets**.
3.  Select **+ Add**.

> [!NOTE]
> **Validation step:** Confirm Cost Management is open and you have selected your budget scope.

## Task 2: Configure and create the budget

Set up your budget parameters including amount, reset period, and alert thresholds. These alerts will notify you before you overspend, giving you time to investigate and adjust.

1. For **Name**, enter **gp-pilot-budget**.
2. For **Reset period**, select **Monthly**.
3. For **Amount**, enter a small test value such as **10** (USD or your billing currency).
4. Select **Next** to move to the alerts section.
5. For **Type**, select **Actual**.
6. For the threshold, enter **80** percent.
7. For **Type**, select **Actual cost**.
8. For the threshold, enter **100** percent.
9. In the **Alert recipients** field, enter the same email address.
10. Select **Create**.

> [!NOTE]
> **Validation step:** Confirm the **gp-pilot-budget** appears in the budgets list with two alert thresholds (80% and 100%).
