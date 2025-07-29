%% 三级指标逻辑图（并列结构）
graph TD
    %% ---------- 一级目标 ----------
    Y["Y: Repayment Guarantee for Core Enterprises in the Supply Chain"]

    %% ---------- 二级维度 ----------
    A1["A1: Core Enterprise Profitability"]
    A2["A2: Core Enterprise Debt Repayment Ability"]
    A3["A3: Core Enterprise Credit Status"]
    A4["A4: Core Enterprise Quality"]
    C1["C1: Supply Chain Cooperation Quality"]

    %% ---------- 三级指标 ----------
    %% A1 下属
    A11["A11: Earnings per Share"]
    A12["A12: Return on Equity"]
    A13["A13: Net Profit Growth Rate"]
    A14["A14: Pre-interest and Post-tax Profit"]

    %% A2 下属
    A21["A21: Asset–Liability Ratio"]
    A22["A22: Total Assets"]
    A23["A23: Cash Ratio"]
    A24["A24: Quick Ratio"]
    A25["A25: External Guarantee Situation"]

    %% A3 下属
    A31["A31: Credit Status"]
    A32["A32: Financial Report Audit Opinion"]

    %% A4 下属
    A41["A41: Employee Quality"]
    A42["A42: Management Level"]
    A43["A43: Employee Loyalty"]

    %% C1 下属
    C11["C11: Concentration of Suppliers"]
    C12["C12: Supply Chain Concentration"]
    C13["C13: Degree of Information Sharing within the Supply Chain"]

    %% ---------- 连线关系 ----------
    %% 一级 → 二级
    Y --&gt; A1
    Y --&gt; A2
    Y --&gt; A3
    Y --&gt; A4
    Y --&gt; C1

    %% 二级 → 三级
    A1 --&gt; A11
    A1 --&gt; A12
    A1 --&gt; A13
    A1 --&gt; A14

    A2 --&gt; A21
    A2 --&gt; A22
    A2 --&gt; A23
    A2 --&gt; A24
    A2 --&gt; A25

    A3 --&gt; A31
    A3 --&gt; A32

    A4 --&gt; A41
    A4 --&gt; A42
    A4 --&gt; A43

    C1 --&gt; C11
    C1 --&gt; C12
    C1 --&gt; C13

    %% ---------- 视觉样式 ----------
    classDef level1 fill:#1E90FF,stroke:#000,stroke-width:2px,color:#fff
    classDef level2 fill:#FFD700,stroke:#000,stroke-width:1.5px,color:#000
    classDef level3 fill:#98FB98,stroke:#000,stroke-width:1px,color:#000

    class Y level1
    class A1,A2,A3,A4,C1 level2
    class A11,A12,A13,A14,A21,A22,A23,A24,A25,A31,A32,A41,A42,A43,C11,C12,C13 level3
