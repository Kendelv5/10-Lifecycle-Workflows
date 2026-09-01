# Lab 10: Microsoft Entra ID Lifecycle Workflows

## 🎯 Objective
Configure automated cloud-native identity lifecycle orchestration using Microsoft Entra ID Lifecycle Workflows to execute scheduled deprovisioning, session revocation, and offboarding tasks.

---

## 🏗️ Architecture & Scenario
Manual offboarding processes introduce severe security risks, including orphaned accounts and lingering active sessions. Modern identity governance utilizes automated workflow engines to execute timed lifecycle actions without administrative intervention. This lab establishes an automated offboarding pipeline:
1. **Workflow Template Selection:** Utilized native Microsoft Entra governance templates tailored for employee termination and offboarding.
2. **Execution Scoping:** Targeted designated test groups and user objects for automated evaluation.
3. **Task Orchestration:** Configured automated actions to disable user accounts, revoke active authentication sessions, and purge group memberships systematically upon trigger conditions.

---

## ⚙️ Configuration Steps

### 1. Workflow Initialization
* Navigated to **Microsoft Entra admin center** > **Identity governance** > **Lifecycle workflows** > **+ Create workflow**.
* Selected a pre-configured offboarding template and named the workflow `Automated-Leaver-Offboarding`.

### 2. Scoping & Timing Parameters
* Configured target user scopes to evaluate specific test groupings.
* Defined execution schedules and validated underlying task components (Account disabling, session teardown).

---

## 🧪 Validation & Testing
* **Workflow Deployment:** Verified that the custom lifecycle workflow is successfully created, scheduled, and monitoring designated object scopes within the Entra governance plane.

---

## 💡 Key Takeaways & Challenges
* **Automated Offboarding Hygiene:** Learned how cloud-native orchestration engines mitigate insider threat vectors and administrative drag by automating day-two lifecycle operations.
* **Multi-Vendor Orchestration:** Contrasted native Microsoft lifecycle automation workflows with Okta-based state rules, broadening enterprise identity operations capabilities.
