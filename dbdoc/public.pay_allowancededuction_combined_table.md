# public.pay_allowancededuction_combined_table

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| headid | integer | nextval('pay_allowancededuction_combined_table_headid_seq'::regclass) | false |  |  |  |
| monthid | integer |  | false |  |  |  |
| yearid | integer |  | true |  |  |  |
| payperiodid | integer |  | true |  |  |  |
| employeeid | integer |  | true |  |  |  |
| pay_headid | integer |  | true |  |  |  |
| amount | numeric(18,2) |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |

## Relations

![er](public.pay_allowancededuction_combined_table.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
