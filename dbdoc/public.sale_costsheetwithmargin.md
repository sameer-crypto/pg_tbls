# public.sale_costsheetwithmargin

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| transactionid | integer | nextval('sale_costsheetwithmargin_transactionid_seq'::regclass) | false |  |  |  |
| transactionno | text |  | true |  |  |  |
| transactiondate | date |  | true |  |  |  |
| projectcode | text |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| isauthorized | boolean | false | false |  |  |  |
| createdby | integer |  | false |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp(6) without time zone |  | true |  |  |  |
| seriescode | varchar(50) |  | true |  |  |  |
| seriesno | integer |  | true |  |  |  |
| createdon | timestamp(6) without time zone | now() | true |  |  |  |
| seriesvouchertype | smallint | 0 | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| iscancelled | boolean | false | true |  |  |  |
| editlog | text |  | true |  |  |  |
| cancellationreason | text |  | true |  |  |  |
| cancellationdate | date |  | true |  |  |  |
| cancelledby | integer |  | true |  |  |  |
| amendreason | text |  | true |  |  |  |
| amendby | integer |  | true |  |  |  |
| amendon | timestamp(6) without time zone |  | true |  |  |  |

## Relations

![er](public.sale_costsheetwithmargin.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)
