# public.fa_fixedassetbudgetmaster_amendlog

## Description

## Columns

| Name | Type | Default | Nullable | Children | Parents | Comment |
| ---- | ---- | ------- | -------- | -------- | ------- | ------- |
| fixedassetbudgetamendmasterid | integer | nextval('fa_fixedassetbudgetmaster_ame_fixedassetbudgetamendmasterid_seq'::regclass) | false |  |  |  |
| fixedassetbudgetmasterid | integer |  | true |  |  |  |
| budgetno | varchar(200) |  | true |  |  |  |
| budgetdate | date |  | true |  |  |  |
| budgetamount | numeric(21,3) |  | true |  |  |  |
| remarks | text |  | true |  |  |  |
| finyearid | integer |  | true |  |  |  |
| branchid | integer |  | true |  |  |  |
| isauthorized | boolean | false | true |  |  |  |
| authorizedby | integer |  | true |  |  |  |
| authorizedon | timestamp(6) without time zone |  | true |  |  |  |
| createdby | integer |  | true |  |  |  |
| createdon | timestamp(6) without time zone | now() | true |  |  |  |
| editlog | text |  | true |  |  |  |
| headauthorizedby | integer |  | true |  |  |  |
| headauthorizedon | timestamp(6) without time zone |  | true |  |  |  |
| seriesno | integer |  | true |  |  |  |
| seriescode | varchar(20) |  | true |  |  |  |
| seriesid | integer |  | true |  |  |  |
| seriesvouchertype | integer |  | true |  |  |  |
| iscancelled | boolean |  | true |  |  |  |
| amendby | integer |  | true |  |  |  |
| amendon | timestamp(6) without time zone |  | true |  |  |  |
| amendreason | text |  | true |  |  |  |
| isamended | boolean | false | true |  |  |  |
| updatedby | integer |  | true |  |  |  |
| updatedon | timestamp(6) without time zone | NULL::timestamp without time zone | true |  |  |  |

## Constraints

| Name | Type | Definition |
| ---- | ---- | ---------- |
| fa_fixedassetbudgetmaster_amendlog_pkey | PRIMARY KEY | PRIMARY KEY (fixedassetbudgetamendmasterid) |

## Indexes

| Name | Definition |
| ---- | ---------- |
| fa_fixedassetbudgetmaster_amendlog_pkey | CREATE UNIQUE INDEX fa_fixedassetbudgetmaster_amendlog_pkey ON public.fa_fixedassetbudgetmaster_amendlog USING btree (fixedassetbudgetamendmasterid) |

## Relations

![er](public.fa_fixedassetbudgetmaster_amendlog.svg)

---

> Generated by [tbls](https://github.com/k1LoW/tbls)