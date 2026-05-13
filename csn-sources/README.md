# SAP S/4HANA Cloud — CSN Data Product Reference

Auto-generated from official SAP CSN JSON files. English labels only.

One file per data product. Includes all entity fields with type, key, label, currency/UOM reference, FK association, and ECC/S4 compatibility flag.


## ECC / S4 Diff Flag Logic

| Flag | Meaning |
|---|---|
| `S/4 only entity (no ECC CDC mapping)` | Entity has no `@Analytics.dataExtraction` CDC mapping — it is native S/4 with no direct ECC table equivalent |
| `S/4 only — no ECC equivalent` | Named field (e.g. `SourceLedger`, `AmountInGlobalCurrency`) does not exist in ECC |
| `S/4 only — ECC BSEG lacks global currency` | Global currency amounts require FX derivation in ECC; native in S/4 ACDOCA |
| `ECC: BKPF.MONAT (unpadded '3'); S/4: zero-padded '003'` | `FiscalPeriod` stored differently between versions — handle in Bronze |


## Data Products

| File | Entities | ECC Source Tables |
|---|---|---|
| [ARBankStatement](./sap-s4com-ARBankStatement-v1.md) | `ARBankStatement`, `BankStmntItemReprocessReason`, `BankStmntItmReprocessRsnText` | — |
| [BillingDocument](./sap-s4com-BillingDocument-v1.md) | `BillingDocument`, `BillingDocumentItem` | vbrk, vbrp |
| [CashFlow](./sap-s4com-CashFlow-v1.md) | `CashFlow`, `CashFlowForecast` | — |
| [CnsldtnGLChartOfAccounts](./sap-s4com-CnsldtnGLChartOfAccounts-v1.md) | `CnsldtnGLChartOfAccounts`, `CnsldtnGLChartOfAccountsText` | — |
| [CompanyCode](./sap-s4com-CompanyCode-v1.md) | `CompanyCode`, `CompanyCodeCurrencyRole`, `CompanyCodeCurrencyTranslation`, `CompanyCodeHierarchy`, `CompanyCodeHierarchyNode`, `CompanyCodeHierarchyNodeText`, `CompanyCodeHierarchyText`, `CurrencyRole`, `CurrencyRoleText` | — |
| [ControllingArea](./sap-s4com-ControllingArea-v1.md) | `ControllingArea` | — |
| [CostCenter](./sap-s4com-CostCenter-v1.md) | `CostCenter`, `CostCenterCategory`, `CostCenterCategoryText`, `CostCenterHierarchy`, `CostCenterHierarchyNode`, `CostCenterHierarchyNodeText`, `CostCenterHierarchyText`, `CostCenterText` | — |
| [CostCenterActivityType](./sap-s4com-CostCenterActivityType-v1.md) | `CostCenterActivityType`, `CostCenterActivityTypeCatText`, `CostCenterActivityTypeCategory`, `CostCenterActivityTypeText`, `CostCtrActivityTypeHierNdeText`, `CostCtrActivityTypeHierNode`, `CostCtrActivityTypeHierText`, `CostCtrActivityTypeHierarchy` | — |
| [CostOriginGroup](./sap-s4com-CostOriginGroup-v1.md) | `CostOriginGroup`, `CostOriginGroupText` | — |
| [Customer](./sap-s4com-Customer-v1.md) | `Customer`, `CustomerCompanyCode`, `CustomerDunning`, `CustomerSalesArea`, `CustomerSalesAreaTax`, `CustomerUnloadingPoint`, `CustomerWithHoldingTax` | ADRC, KNA1, KNB1, KNB5 |
| [FinancialTransaction](./sap-s4com-FinancialTransaction-v1.md) | `FXFixingReferenceText`, `FinInstrActivityCategoryText`, `FinInstrProductTypeSupplement`, `FinInstrProductTypeText`, `FinInstrTransCategoryText`, `FinInstrTransactionCategory`, `FinInstrTransactionTypeText`, `FinInstrumentActivityCategory`, `FinTransNoticePeriodUnit`, `FinTransNoticePeriodUnitText`, `FinTransOptionExerciseType`, `FinTransOptionExerciseTypeText`, `FinTransOptionSettlementType`, `FinTransOptnSettlementTypeText`, `FinTransOptnUndrlgAllocation`, `FinTransReleaseStatus`, `FinTransReleaseStatusText`, `FinTransUnderlyingFlow`, `FinancialInstrTransactionType`, `FinancialInstrumentProductType`, `FinancialInstrumentStatus`, `FinancialInstrumentStatusText`, `FinancialTransaction`, `ForeignExchangeFixingReference`, `TradeFinanceCategory`, `TradeFinanceCategoryText`, `TreasuryContractType`, `TreasuryContractTypeText`, `TreasuryPortfolio`, `TreasuryPortfolioText`, `TreasuryProductCategory`, `TreasuryProductCategoryText`, `TreasuryReversalReason`, `TreasuryReversalReasonText` | — |
| [FiscalYear](./sap-s4com-FiscalYear-v1.md) | `FiscalYear`, `FiscalYearVariant`, `FiscalYearVariantText` | — |
| [FunctionalArea](./sap-s4com-FunctionalArea-v1.md) | `FunctionalArea`, `FunctionalAreaHierNodeText`, `FunctionalAreaHierarchy`, `FunctionalAreaHierarchyNode`, `FunctionalAreaHierarchyText`, `FunctionalAreaText` | — |
| [GeneralLedgerAccount](./sap-s4com-GeneralLedgerAccount-v1.md) | `ChartOfAccounts`, `ChartOfAccountsText`, `FinancialStatementHierNode`, `FinancialStatementHierNodeText`, `FinancialStatementHierText`, `FinancialStatementHierarchy`, `GLAccountHierNodeBySemanticTag`, `GLAccountHierarchyNode`, `GLAccountHierarchyNodeText`, `GLAccountHierarchyText`, `GLAccountTypeFlowType`, `GeneralLedgerAccount`, `GeneralLedgerAccountFlowType`, `GeneralLedgerAccountHierarchy`, `GeneralLedgerAccountLineItem`, `GeneralLedgerAccountText`, `GeneralLedgerAccountTypeText`, `OperatingGeneralLedgerAccount`, `SemanticTag`, `SemanticTagFunctionalArea`, `SemanticTagGeneralLedger`, `SemanticTagLeafNode`, `SemanticTagText` | — |
| [InvoiceList](./sap-s4com-InvoiceList-v1.md) | `InvoiceList`, `InvoiceListItem` | — |
| [JournalEntryCodes](./sap-s4com-JournalEntryCodes-v1.md) | `BusinessTransactionCategory`, `BusinessTransactionCategoryText`, `BusinessTransactionType`, `BusinessTransactionTypeText`, `FinancialTransactionType`, `FinancialTransactionTypeText`, `JournalEntryCategory`, `JournalEntryCategoryText`, `JournalEntryType`, `JournalEntryTypeText`, `ReferenceDocumentType`, `ReferenceDocumentTypeText` | — |
| [JournalEntryHeader](./sap-s4com-JournalEntryHeader-v1.md) | `JournalEntry`, `JournalEntryItemBillOfExchange` | BKPF |
| [JournalEntryItemCodes](./sap-s4com-JournalEntryItemCodes-v1.md) | `AssetAcctTransClassification`, `ControllingDebitCreditCode`, `ControllingDebitCreditCodeText`, `DebitCreditCode`, `DebitCreditCodeText`, `FinancialAccountType`, `FinancialAccountTypeText`, `GeneralLedgerRecordType`, `JournalEntryItemObsoleteReason`, `JrnlEntryItemObsltRsnText`, `MovementCategoryText`, `PostingKey`, `PostingKeyText`, `PostingKeyWithSpecialGLCode`, `PostingKeyWithSpecialGLCodeText`, `SpecialGeneralLedgerCode`, `SpecialGeneralLedgerCodeText`, `SubledgerAccountLineItemType`, `SubledgerAccountLineItemTypeText` | — |
| [Ledger](./sap-s4com-Ledger-v1.md) | `Ledger`, `LedgerCompanyCodeCurrencyRoles`, `LedgerSourceLedger`, `LedgerText` | — |
| [Plant](./sap-s4com-Plant-v1.md) | `Plant`, `PlantCategory` | — |
| [Product](./sap-s4com-Product-v1.md) | `ProdIntlTradeClassification`, `ProdWhseManagementStorageType`, `Product`, `ProductConsumption`, `ProductDescription`, `ProductGroup`, `ProductGroupText`, `ProductMRPArea`, `ProductPlant`, `ProductPlantCosting`, `ProductPlantForecast`, `ProductPlantInternationalTrade`, `ProductPlantProcurement`, `ProductPlantPurchaseTax`, `ProductPlantQualityManagement`, `ProductPlantStorage`, `ProductPlantSupplyPlanning`, `ProductPlantWorkScheduling`, `ProductProcurement`, `ProductQualityManagement`, `ProductSales`, `ProductSalesDelivery`, `ProductStorage`, `ProductUnitOfMeasure`, `ProductUnitOfMeasureEAN`, `ProductValuation`, `ProductValuationAccounting`, `ProductValuationCosting`, `ProductWarehouseManagement` | — |
| [ProfitCenter](./sap-s4com-ProfitCenter-v1.md) | `PrftCtrCompanyCodeAssignment`, `ProfitCenter`, `ProfitCenterHierarchy`, `ProfitCenterHierarchyNode`, `ProfitCenterHierarchyNodeText`, `ProfitCenterHierarchyText`, `ProfitCenterText` | — |
| [PurchaseOrder](./sap-s4com-PurchaseOrder-v1.md) | `PurOrdSupplierConfirmation`, `PurchaseOrder`, `PurchaseOrderAccountAssignment`, `PurchaseOrderItem`, `PurchaseOrderScheduleLine` | — |
| [SalesMasterDataConfiguration](./sap-s4com-SalesMasterDataConfiguration-v1.md) | `AdditionalCustomerGroup1`, `AdditionalCustomerGroup1Text`, `AdditionalCustomerGroup2`, `AdditionalCustomerGroup2Text`, `AdditionalCustomerGroup3`, `AdditionalCustomerGroup3Text`, `AdditionalCustomerGroup4`, `AdditionalCustomerGroup4Text`, `AdditionalCustomerGroup5`, `AdditionalCustomerGroup5Text`, `AdditionalProductGroup1`, `AdditionalProductGroup1Text`, `AdditionalProductGroup2`, `AdditionalProductGroup2Text`, `AdditionalProductGroup3`, `AdditionalProductGroup3Text`, `AdditionalProductGroup4`, `AdditionalProductGroup4Text`, `AdditionalProductGroup5`, `AdditionalProductGroup5Text`, `BillingBlockReason`, `BillingBlockReasonText`, `CustomerAccountAssignmentGroup`, `CustomerAccountAssignmentGroupText`, `CustomerGroup`, `CustomerGroupText`, `CustomerPriceGroup`, `CustomerPriceGroupText`, `DeliveryDateTypeRule`, `DeliveryDateTypeRuleText`, `IncotermsClassification`, `IncotermsClassificationText`, `IncotermsVersion`, `IncotermsVersionText`, `MaterialPricingGroup`, `MaterialPricingGroupText`, `ProductCommissionGroup`, `ProductCommissionGroupText`, `ProductItemCategoryGroup`, `ProductItemCategoryGroupText` | — |
| [SalesOrder](./sap-s4com-SalesOrder-v1.md) | `SalesOrder`, `SalesOrderItem` | vbak, vbap, vbkd, veda |
| [Supplier](./sap-s4com-Supplier-v1.md) | `Supplier`, `SupplierCompanyCode`, `SupplierPurchasingOrganization`, `SupplierWithHoldingTax` | ADRC, LFA1, LFM1, lfb1, t001 |
